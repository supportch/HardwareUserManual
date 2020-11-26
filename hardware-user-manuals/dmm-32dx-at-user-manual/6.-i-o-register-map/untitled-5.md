# 6.4 Page 0: 82C54 Counter/Timer Access

This section is included as a reference to the page 0 counter/timer registers. Behavior of these registers should be identical to the 82C54 counter/timer chip. Please read reference \[12\], the 82C54 datasheet, for this behavior. More info on counter/timer signals can be found later in this document.

**Page 0, Base + 12**       **Read/Write**     **Counter 0 data**

![](../../../.gitbook/assets/19%20%283%29.png)

CTR0D7-0    Counter 0 data

**Page 0, Base + 13**      **Read/Write**      **Counter 1 data**

![](../../../.gitbook/assets/20%20%283%29.png)

CTR1D7-0    Counter 1 data

**Page 0, Base + 14**      **Read/Write**      **Counter 2 data**

![](../../../.gitbook/assets/21%20%285%29.png)

**Page 0, Base + 15**      **Read/Write**      **Counter/timer Control Register**

![](../../../.gitbook/assets/22%20%283%29.png)

|  |  |
| :--- | :--- |
| SC1-0 | Counter Select |
| RW1-0 | Read/Write Mode |
| M2-0 | Timer Mode |
| BCD | Binary Coded Decimal Count |

For more information see the 82C54 Datasheet

