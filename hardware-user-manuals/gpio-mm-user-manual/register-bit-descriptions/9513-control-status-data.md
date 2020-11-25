# 9513 Control/Status Data

**Base+00h \(9513-1\)/Base+04h \(9513-2\) \(Read/Write\)**

![](../../../.gitbook/assets/13%20%282%29.png)

|  |  |
| :--- | :--- |
| D7-D0 | 9513-1 and 9513-2 counter/timer control and status data registers. Control data written to these registers will be written to the 9513 location specified by the Control/Status Pointer register, below. Status data is read from these registers, also, from the location specified by the Control/Status Pointer register. Refer to the 9513 data sheet, referenced in the Additional Information section of this document, for a description of the contents of this register and how to use this register with the Control/Status Pointer register. \(Register Base+00h is associated with the Base+01h pointer register, and register Base+04h is associated with the Base+05h pointer register.\) |



