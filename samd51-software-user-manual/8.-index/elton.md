# Elton

### Overview <a id="overview"></a>

Elton™ utilizes the NVIDIA® Jetson™ AGX Xavier™ embedded computer module to deliver unmatched performance for AI, machine learning, image processing, and other compute-intensive tasks. 

Elton provides numerous sockets for I/O expansion. An industry-standard camera module socket supports the attachment of up to 8 CSI cameras \(up to 4 cameras with 4K resolution\). An M.2 socket supports the use of PCIe x4 NVMe flash storage up to 256GB. An LTE module socket supports the use of NimbeLink SkyWire cellular modems, featuring a broad range of solutions with worldwide compatibility. Most notably, a full PCI/104- Express expansion socket enables the use of PCI-104 and PCIe/104 expansion modules with up to PCIe x8 bandwidth. 

All I/O is provided on pin headers that are compatible with both common non-latching and rugged latching mating cables, making Elton ideal for applications in environments subject to high shock and vibration.

### Features <a id="features"></a>

* Supports A/D channels 0-5\(single ended\), 0-2\(differential ended\) and 12 -15\(on-board voltage\)
* Supports A/D single ended and differential ended.
* Supports D/A conversion.
* Supports port A: 0-7\(8 bits\) and port B: 0-4\(5 bits\)
* Supports serial port \(1 & 2, 3 & 4\) configuration.
* Supports temperature read.
* Supports WLAN, LTE, FAN control & User Led.
* Supports 2 cameras.

### Pin out diagram

![](../../.gitbook/assets/elton.png)

### Analog Input <a id="analog-input"></a>

<table>
  <thead>
    <tr>
      <th style="text-align:left">&#x200B;</th>
      <th style="text-align:left">&#x200B;</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">Max Input Channels:</td>
      <td style="text-align:left">
        <p>0 to 5 (Single ended)</p>
        <p>0 to 2 (Differential ended)</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">A/D Resolution:</td>
      <td style="text-align:left">No oversampling : 12 bit</td>
    </tr>
    <tr>
      <td style="text-align:left">&#x200B;</td>
      <td style="text-align:left">Oversampling: 14 bit, 15 bit, 16 bit</td>
    </tr>
    <tr>
      <td style="text-align:left">Data range:</td>
      <td style="text-align:left">Single ended: 0 to 4095</td>
    </tr>
    <tr>
      <td style="text-align:left">&#x200B;</td>
      <td style="text-align:left">Differential ended: -2048 to 2047</td>
    </tr>
    <tr>
      <td style="text-align:left">Supported Conversion Triggers:</td>
      <td style="text-align:left">Software initiated A/D conversion</td>
    </tr>
    <tr>
      <td style="text-align:left">A/D Reference</td>
      <td style="text-align:left">External reference(3.3 V)</td>
    </tr>
  </tbody>
</table>

### Analog Output <a id="analog-output"></a>

| ​ | ​ |
| :--- | :--- |
| Max Output Channels: | 2 |
| D/A Resolution: | 12 bits |
| Data range: | 0 to 4095 |

### Digital I/O <a id="digital-i-o"></a>

<table>
  <thead>
    <tr>
      <th style="text-align:left">&#x200B;</th>
      <th style="text-align:left">&#x200B;</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">Max Ports:</td>
      <td style="text-align:left">
        <p>Supports 2 DIO ports namely Port A &amp; Port B</p>
        <p>(Port A - 0 to 7 bits, Port B - 0 to 4 bits)</p>
      </td>
    </tr>
  </tbody>
</table>

### Elton SAMD51 Functions <a id="jethro-samd51-functions"></a>

* [​DSCSAM\_ADSample\(\) ​](../9.-samd51-apis/dscsam_adsample.md)
* ​[DSCSAM\_ADScan\(\) ​](../9.-samd51-apis/dscsam_adscan.md)
* ​[DSCSAM\_ADSetSettings\(\)](../9.-samd51-apis/dscsam_adsetsettings.md) ​
* ​[DSCSAM\_CAMERAControl\(\)](../9.-samd51-apis/dscsam_cameracontrol.md) ​
* ​[DSCSAM\_DAConvert\(\) ​](../9.-samd51-apis/dscsam_daconvert.md)
* ​[DSCSAM\_DIOBitConfig\(\)](../9.-samd51-apis/dscsam_diobitconfig.md) ​
* ​[DSCSAM\_DIOConfig\(\) ​](../9.-samd51-apis/dscsam_dioconfig.md)
* ​[DSCSAM\_DIOConfigAll\(\)](../9.-samd51-apis/dscsam_dioconfigall.md) ​
* ​[DSCSAM\_DIOInputBit\(\)](../9.-samd51-apis/dscsam_dioinputbit.md) ​
* ​[DSCSAM\_DIOInputByte\(\) ](../9.-samd51-apis/dscsam_dioinputbyte.md)​
* ​[DSCSAM\_DIOOutputBit\(\)](../9.-samd51-apis/dscsam_diooutputbit.md) ​
* [​DSCSAM\_DIOOutputByte\(\) ​](../9.-samd51-apis/dscsam_diooutputbyte.md)
* ​[DSCSAM\_FANControl\(\) ](../9.-samd51-apis/dscsam_fancontrol.md)​
* ​[DSCSAM\_FLASHRead\(\) ](../9.-samd51-apis/dscsam_flashread.md)​
* ​[DSCSAM\_FLASHWrite\(\) ](../9.-samd51-apis/dscsam_flashwrite.md)​
* ​[DSCSAM\_LEDControl\(\)](../9.-samd51-apis/dscsam_ledcontrol.md) ​
* ​[DSCSAM\_LTEControl\(\)](../9.-samd51-apis/dscsam_ltecontrol.md) ​
* [​DSCSAM\_SerialPortConfig\(\) ](../9.-samd51-apis/dscsam_serialportconfig.md)​
* ​[DSCSAM\_TemperatureSensorRead\(\)](../9.-samd51-apis/dscsam_temperaturesensorread.md) ​
* ​[DSCSAM\_WLANControl\(\)​](../9.-samd51-apis/dscsam_wlancontrol.md)

