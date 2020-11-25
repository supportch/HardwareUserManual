# EEPROM Data

**Base+08h \(Read/Write\)**

![](../../../.gitbook/assets/18%20%283%29.png)

|  |  |
| :--- | :--- |
| D7-D0 | Writing to this register writes data to the EEPROM at the address specified by the EEPROM Address Register \(Base+09h\). Reading from this register returns the EEPROM data at the EEPROM Address Register \(Base+09h\) location; read data is valid when EEBUSY = 0 in the EEPROM Status Register \(Base+0Ah\). |



