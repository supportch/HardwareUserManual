# Auxiliary DIO Status

**Base+0Eh \(Read\)**

![](../../../.gitbook/assets/27%20%287%29.png)

|  |  |
| :--- | :--- |
| AUXnIN | Auxiliary DIO line. Read the respective AUXnIN bit to determine the auxiliary DIO line state.                                                                     0 = low level                                                                                                                      1 = high level                                                                                                                If the line is currently set to output mode, according to the AUXnDIR bit, below, the read value corresponds to the current output level.  |
| AUXnDIR | Auxiliary line I/O direction and state. Read the bit to determine the current I/O mode.                                                                                0 = output mode                                                                                                            1 = input mode |

     

       

