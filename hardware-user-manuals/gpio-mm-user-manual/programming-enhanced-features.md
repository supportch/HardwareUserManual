---
description: EEPROM Programming
---

# Programming Enhanced Features

The EEPROM provides non-volatile memory for storing application data. 

Program the EEPROM using the following steps. Repeat these steps for each data byte. 

1. Write the data byte to the EEPROM Data Register \(08h\).        
2. Specify the EEPROM address \(0-256\) where the data is to be written by writing the address to the EEPROM Address Register \(09h\).
3. Set the data transfer direction to write by resetting the EE\_RW bit in the EEPROM Control and Status Register \(0Ah\).                                                   
4. Set the EE\_EN bit in the EEPROM Control and Status Register \(0Ah\) to initiate the write operation. 

To read stored EEPROM data, use the following steps. Repeat these steps for each data byte.      

1. Specify the EEPROM address \(0-256\) where the data is to be read from by writing the address to the EEPROM Address Register \(09h\). 
2. Set the data transfer direction to read by setting the EE\_RW bit in the EEPROM Control and Status Register \(0Ah\).                                                   
3. Reset the EE\_EN bit in the EEPROM Control and Status Register \(0Ah\) to initiate the read operation.                                                                        
4. Test the EEPROM Control and Status Register \(0Ah\) EEBUSY bit to determine that the data transfer has completed. When EEBUSY is zero, a valid data byte is available and the next byte may be read.

