# Base Address Selection

Jumper J10, positions 2-5, is used to configure the base address of the DIO \(8255\) registers. The 8255 register map occupies 8 bytes of I/O address space, as described in Section 5, I/O Map. Jumper positions 6-9, is used to configure the base address of the counter/timer I/O \(9513\) registers and the enhanced features registers. The 9513 register map occupies 16 bytes of I/O address space, as described in Section 5, I/O Map. Jumper the locations as shown to set the 8255 and 9513 base addresses.

![](../../../.gitbook/assets/4%20%283%29.png)

#### NOTE: Different address must be selected for the DIO and counter/timer functions. 

The example, below, selects a DIO base address of 0040h.

![Figure 2: Example - Set DIO Base Address to 0040h](../../../.gitbook/assets/5%20%281%29.png)

The following example selects a counter/timer base address of 0100h.

![Figure 3: Example - Set Counter/Timer Base Address to 0100h](../../../.gitbook/assets/6%20%283%29.png)



