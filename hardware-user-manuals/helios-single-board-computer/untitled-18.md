# 17. A/D SCAN, INTERRUPT AND FIFO OPERATION

The control bits SCANEN \(scan enable\) and AINTE \(A/D interrupt enable\) in conjunction with the FIFO determine the behavior of the board during A/D conversions and interrupts. 

#### FIFO Operation 

A FIFO integrated into the FPGA design provides a temporary buffer for storing A/D conversions before the application program reads them. The main purpose of the FIFO is to reduce the interrupt rate in order to reduce the software load on the processor during high speed sampling.

 On power-up or reset, the FIFO is set to basic mode, with depth 48 with threshold 16 for backward compatibility with older Diamond products. When EXFIFO=1 \(expanded FIFO mode is set\), the FIFO is set to depth 2048 with threshold 1024. At the end of an AD conversion, the 16-bit A/D data is latched into the FIFO. A/D Data is read out of the FIFO with 2 read operations, first Base + 0 \(LSB\) and then Base + 1 \(MSB\). The A/D FIFO depth register FDn:0 keeps track of the number of A/D samples in the FIFO. Each time an A/D conversion completes, data is written into the FIFO and the depth register increments by 1. When the MSB of the A/D data is read, the FIFO depth counter will decrement by 1 sample. 

If the FIFO reaches its limit \(48 samples in basic mode, 2048 samples in enhanced mode\), then the next time an A/D conversion occurs the Overflow flag OF will be set. In this case the FIFO will not accept any more data, and its contents will be preserved and may be read out. In order to clear the overflow condition, the program must reset the FIFO by writing to the RSTFIFO bit in Base + 1, or a hardware reset must occur. 

#### Scan operation 

When SCANEN = 1, each time an A/D trigger occurs, the board will perform an A/D conversion on all channels in the channel range programmed in Base + 2. When SCANEN = 0, each time an A/D trigger occurs, the board will perform a single A/D conversion and then advance to the next channel and wait for the next trigger. The total sample rate of the board is equal to the scan rate \(A/D trigger rate\) times the number of channels in the scan \(scan size\). The total sample rate cannot exceed the board’s limit of 250KHz. 

#### Interrupt operation 

When AINTE=1 \(base+4 bit 0\), once the FIFO depth equals or exceeds the programmed depth value, an interrupt request will occur. If AINTE = 0, the FIFO threshold is ignored and the FIFO continues to fill up. 

To detect if an interrupt has occurred, the AINT status bit can be read \(base+7 bit 4\). To clear the interrupt, write a 1 to the CLRA bit \(base+0 bit 0\) or disable analog interrupts by setting AINTE=0. 

When an interrupt is pending, the IRQ line will be driven high. When no interrupt is pending, the board will release the IRQ line and it will be pulled low by the pull-down resistor configured with J21. It is possible for Helios to generate interrupts from up to 3 sources simultaneously. Thus clearing one interrupt will not necessarily cause the IRQ line to go low. It will only go low when all 3 circuits are inactive or have no interrupts pending. 

In Scan mode \(SCANEN = 1\), the FIFO threshold should be set to a number at least equal to the scan size and in all cases equal to an integral number of scans. For example if the scan size is 8 channels, the FIFO threshold should be set to 8, 16, 24, 32, … but not less than 8. This way the interrupt will occur at the end of the scan, and the interrupt routine can read in a complete scan or set of scans each time it runs. 

In non-scan mode \(SCANEN = 0\), the FIFO threshold should be set to a level that minimizes the interrupt rate but leaves enough time for the interrupt routine to respond before the FIFO fills up. No A/D data is available to the application program until the interrupt occurs, so if the threshold is high but the rate is slow, the delay to receive A/D data may be longer than acceptable. Therefore for slow sample rates the FIFO threshold should be small. If the sample rate is high, the FIFO threshold should be high to reduce the interrupt rate. However remember that the remaining space in the FIFO determines the time the interrupt routine has to respond to the interrupt request. If the FIFO threshold is too high, the FIFO may overflow before the interrupt routine responds. A good rule of thumb is to set the FIFO threshold so as to limit the interrupt rate to no more than 1,000-2,000 per second in Windows and Linux or 10,000 per second in DOS.

Here are some general guidelines for FIFO thresholds. Experimentation may be necessary to determine the optimum FIFO threshold for each application. Total sample rate means sample rate for sample \(non-scan\) mode and scan rate times scan size for scan mode. In general, the FIFO should always be used in enhanced mode unless the sample rate is very slow and you want to have a very low FIFO threshold to receive interrupts on every sample or every scan.

| If total sample rate is:  | Set FIFO threshold to \(non-scan\):  |  Set FIFO threshold to \(scan\): |
| :--- | :--- | :--- |
| 0 to 100Hz  | 1 | scan size |
| &gt;100Hz upto 1KHz | 1-10 | 1 – 10 times scan size |
| &gt;1Khz upto 10KHz | 10-100 | 10 – 100 times scan size |
| &gt;10KHz upto 100KHz | 512-1500 | Multiple of scan size within range 512-1500 |

#### Function Modes 

The table below describes the board’s behavior for each of the 4 possible cases of AINTE and SCANEN \(interrupt operation and scan operation\). The interrupt software behavior given in the table describes the operation of the Diamond Systems Universal Driver software. If you write your own software or interrupt routine you should conform to the described behavior for optimum results.

<table>
  <thead>
    <tr>
      <th style="text-align:left">AINTE Base+4 bit 0</th>
      <th style="text-align:left">SCANEN Base+2 bit 1</th>
      <th style="text-align:left">Operation</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">0</td>
      <td style="text-align:left">0</td>
      <td style="text-align:left">
        <p><b>Software-triggered A/D samples </b>
        </p>
        <p>Single A/D conversions are triggered by write to ADSTART bit at base+0.</p>
        <p>ADBUSY stays high during the A/D conversion.</p>
        <p>No interrupt occurs.</p>
        <p>The user program monitors ADBUSY (Base+3, bit 7) and reads A/D data when
          ADBUSY goes low.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">0</td>
      <td style="text-align:left">1</td>
      <td style="text-align:left">
        <p><b>Software-triggered A/D scans </b>
        </p>
        <p>A/D scans are triggered by write to ADSTART bit at base+0.</p>
        <p>All channels between LOW and HIGH are sampled once on each scan.</p>
        <p>ADBUSY stays high during the entire scan (multiple A/D conversions).</p>
        <p>No interrupt occurs.</p>
        <p>The user program monitors ADBUSY (</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">1</td>
      <td style="text-align:left">0</td>
      <td style="text-align:left">
        <p><b>Clock-triggered A/D samples with interrupts </b>
        </p>
        <p>Single A/D conversions are triggered by the source selected with ADCLK
          (Base+4, bit 4).</p>
        <p>ADBUSY stays high during the A/D conversion.</p>
        <p>A/D interrupt occurs when the FIFO reaches its programmed threshold.</p>
        <p>The interrupt routine reads the number of samples equal to the programmed
          FIFO threshold.</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">1</td>
      <td style="text-align:left">1</td>
      <td style="text-align:left">
        <p><b>Clock-triggered A/D scans with interrupts </b>
        </p>
        <p>A/D scans are triggered by the source selected with ADCLK (Base+4, bit
          4).</p>
        <p>ADBUSY stays high during the entire scan (multiple A/D conversions).</p>
        <p>A/D interrupt occurs when the FIFO reaches its programmed threshold.</p>
        <p>The interrupt routine reads the number of samples equal to the programmed
          FIFO threshold.</p>
      </td>
    </tr>
  </tbody>
</table>

