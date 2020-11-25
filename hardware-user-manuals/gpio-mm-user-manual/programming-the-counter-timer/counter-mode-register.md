# Counter Mode Register

Each chip contains five Counter Mode Registers; one for each counter. This register is used to program the operating mode of the counter, including input source, gating method, output type, load/reload behavior and count direction. Note that in the Gate description, Gate N means the gate for the counter being programmed, and Gate N-1 means the gate for the previous counter. Gate N-1 is not valid for counter 1 \(or counter 6 on GPIO-MM, since that corresponds to counter 1 on the second chip\).

