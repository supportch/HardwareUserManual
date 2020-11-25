# 16-bit Fixed Direction\(9513\)

Connector J3 has 8 fixed TTL inputs and 8 fixed TTL outputs. The outputs are set by writing to base+2 or 3. \(See 9513 DIO Data Registers\). Write an 8-bit value to the register at base+2 \(or base+3\) to immediately output the value to the 8 output lines. When reading register base+2 \(or base+3\), the FPGA returns the logic state of the 8 input lines.

