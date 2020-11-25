# 9. PERFORMING AN A/D CONVERSION

This chapter describes the steps involved in performing an A/D conversion on a selected input channel using direct programming \(not with the driver software\).

**The A/D FIFO** 

All A/D conversions are stored in an on-board FIFO \(first in first out memory\). The FIFO can hold up to 1024 samples. Each time an A/D conversion is finished, the data is stored in the FIFO, and the FIFO counter increments by 1. Each time you read A/D data, you are actually reading it out of the FIFO, and the FIFO counter decrements by 1. When the FIFO is empty the data read from it is undefined – you may continue to read the last sample, or you may read all 1s. 

You can read each A/D sample as soon as it is ready, or you can wait until you take a collection of samples \(up to 1024 maximum\) and then read them all out at once. 

To be sure that you are getting only current A/D data, be sure to reset the FIFO each time before you start any A/D operation. This will prevent errors caused by leaving data in from a previous operation. To reset the FIFO, write a 1 to bit 2 of register 7 \(see page 20\). This bit is not a real register bit; instead it triggers a command in the board’s controller chip. Therefore you do not need to write a 1 and then a 0, just write a 1. However writing to the FIFORST bit affects the values of other bits in this register as well: 

**outp\(Base+7, 0x02\); // resets the FIFO and clears SCANEN and FIFOEN** 

#### outp\(Base+7, 0x0A\); // resets the FIFO and SCANEN but leaves FIFOEN set 

Note that this register also contains a FIFO enable bit, FIFOEN. 

This bit only has meaning during A/D interrupt operations. The FIFO is always enabled and is always in use during A/D conversions. 

There are seven steps involved in performing an A/D conversion: 

[      1. Select the input channel or input channel range ](9.1-select-the-input-channel-or-input-channel-range.md)

[      2. Select the analog input range ](9.2-select-the-analog-input-range.md)

[      3. Wait for the analog circuit to settle ](9.3-wait-for-the-analog-circuit-to-settle.md)

[      4. Start an A/D conversion on the current channel ](9.4-start-an-a-d-conversion-on-the-current-channel.md)

[      5. Wait for the conversion to finish ](9.5-wait-for-the-conversion-to-finish.md)

[      6. Read the A/D data ](9.6-read-the-a-d-data.md)

[      7. Convert the numerical data to a meaningful value](9.7-convert-the-numerical-data-to-a-meaningful-value.md)

If you are going to sample the same channel multiple times or sample multiple consecutive channels with the same input range, you only need to perform steps 1-3 once, and then you can repeat steps 4-6 or 4-7 as many times as desired. 

Diamond Systems also provides sample register level code, downloadable at [http://diamondsystems.com/files/binaries/SourceCodeExamples.zip](http://diamondsystems.com/files/binaries/SourceCodeExamples.zip)



