# Counter/Timer and Enhanced Feature Programming

Sixteen registers are used for counter/timer and enhanced feature programming.

| Offset | Description |
| :--- | :--- |
| 00h | 9513-1 command and status data register. Transfers command and status data to/from the register pointed to at base+01h. |
| 01h | 9513-1 command and status data register pointer. Address of the command and status registers for transferring the 8-bit data located at base+00h. |
| 02h | 8-bit DIO data. Set or read the 9513 DIO lines. |
| 03h | Shadow register of base+02h. |
| 04h | 9513-2 command and status data register. Transfers command and status data to/from the register pointed to at base+05h. |
| 05h | 9513-2 command and status data register pointer. Address of the command and status registers for transferring the 8-bit data located at base+04h |
| 06h | Interrupt control. Enable and reset counter/timer interrupts. |
| 07h | Shadow register of base+06h. |
| 08h | EEPROM data. Data written to and read from the EEPROM. |
| 09h | EEPROM address. The EEPROM location for reading or writing data. |
| 0Ah | EEPROM control and status register. Initiate EEPROM data transfer and set the data transfer direction. Also, indicates when valid data is available from EEPROM during a read operation. |
| 0Bh | FPGA revision code and clock source select register. Get the on-board FPGA program revision level. Select 4MHz or 20MHz clock source. |
| 0Ch | Interrupt source selection. Specify the interrupt source for IRQA/IRQB. |
| 0Dh | Interrupt control and status. Enable, disable and clear IRQA/IRQB interrupts and gets the IRQA/IRQB interrupt status. |
| 0Eh | Auxiliary DIO control and status. Set the state of the auxiliary DIO lines and read the current DIO line state. |
| 0Fh | Board reset and board ID code. Reset the board or get the FPGA personality ID code |

