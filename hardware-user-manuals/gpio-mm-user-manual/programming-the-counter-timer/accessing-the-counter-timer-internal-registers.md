# Accessing the Counter/Timer Internal Registers

The chip contains many internal registers. To minimize the I/O memory footprint, a data pointer scheme is used to access these registers. This scheme is reflected in the GPIO-MM board’s I/O map \(Section 5, I/O Map\). The data pointer values are shown in the 9513 datasheet on page 8, Table 4. The appropriate data pointer value is written to the data pointer register for the chip \(Base + 1 for chip no. 1 and Base + 5 for chip no. 2\). Then the register is accessed through the data register \(Base + 0 for chip no. 1 and Base + 4 for chip no. 2\).

