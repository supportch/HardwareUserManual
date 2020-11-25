# Digital I/O Header Pin-out

Connector \(J4\) is the 50-pin general-purpose DIO interface. The connector connects directly to the FPGA, which implements the functionality of two 82C55A PPI chips. This gives a total of 48 bidirectional DIO lines. The J4 pins can be configured to pull-up to +5V or pull-down to ground using jumper J11, as described in Section 4, Board Configuration, Line Pull-up/pull-down Selection.

![](../../../.gitbook/assets/image%20%2895%29.png)

#### NOTE: The connector is labeled “Port 2,” which should not be confused with DIO ports A, B and C and the fixed-direction TTL ports.

| Signal | Description |
| :--- | :--- |
| Port 1A0-Port 1A7 | 8255-1 Port A, bits 0-7 |
| Port 1B0-Port 1B7 | 8255-1 Port B, bits 0-7 |
| Port 1C0-Port 1C7 | 8255-1 Port C, bits 0-7 |
| Port 2A0-Port 2A7 | 8255-2 Port A, bits 0-7 |
| Port 2B0-Port 2B7 | 8255-2 Port B, bits 0-7 |
| Port 2C0-Port 2C7 | 8255-2 Port C, bits 0-7 |
| +5V | +5 volt DC from the PC/104 bus. |
| Ground | Digital ground from the PC/104 bus. |

