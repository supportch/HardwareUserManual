# Interrupt Control

**Base+0Dh \(Write\)**

![](../../../.gitbook/assets/26%20%283%29.png)

|  |  |
| :--- | :--- |
| IRQACLR | IRQA interrupt status and reset. Write a value of 1 to this bit to clear the interrupt. |
| IRQADIS  | IRQA interrupt disable. Write a value of 1 to this bit to disable the IRQA interrupt. This is equivalent to the INTE bit of the Interrupt Control Register \(Base+0Dh\).  |
| IRQAEN | IRQA interrupt enable. Write a value of 1 to this bit to enable the IRQA interrupt. This is equivalent to the INTE bit of the Interrupt Control Register \(Base+0Dh\).  |
| IRQBCLR | IRQB interrupt status and reset. Write a value of 1 to this bit to clear the interrupt.  |
| IRQBDIS  |  IRQB interrupt disable. Write a value of 1 to this bit to disable the IRQB interrupt. This is equivalent to the INTE bit of the Interrupt Control Register \(Base+0Dh\).  |
| IRQBEN  |  IRQB interrupt enable. Write a value of 1 to this bit to enable the IRQB interrupt. This is equivalent to the INTE bit of the Interrupt Control Register \(Base+0Dh\). |

   

