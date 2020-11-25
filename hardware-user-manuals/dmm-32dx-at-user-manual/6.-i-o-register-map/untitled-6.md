# 6.5 Page 1: 82C55 Digital I/O Circuit

This section is included as a reference to the page 1 82C55-like digital I/O registers. More info on the behavior of these digital I/O signals can be found later in this document.

**Page 1, Base + 12**       **Read/Write**     **Digital I/O Port A**

![](../../../.gitbook/assets/23%20%282%29.png)

A7-0    Port A data

**Page 1, Base + 13**      **Read/Write**      **Digital I/O Port B**

![](../../../.gitbook/assets/24%20%283%29.png)

B7-0    Port B data

**Page 1, Base + 14**     **Read/Write**      **Digital I/O Port C**

![](../../../.gitbook/assets/25%20%283%29.png)

**Page 1, Base + 15**    **Read/Write**        **Digital I/O Control Register**

![](../../../.gitbook/assets/26%20%282%29.png)

|  |  |
| :--- | :--- |
| 1 | Bit 7 must be set to 1. This indicates port configure mode in the 8255 \(as opposed to bit set mode which is not supported\). |
| ModeA-C | Mode configuration bits. These must be set to 0. |
| DIRA, DIRB, DIRCH, DIRCL | Direction control bits. On ports A and b, all the bits in each port must be the same direction. On port C, the upper half C7 – C4 can have a different direction than the lower half C3 – C0. |
| 0 | Output |
| 1 | Input |

