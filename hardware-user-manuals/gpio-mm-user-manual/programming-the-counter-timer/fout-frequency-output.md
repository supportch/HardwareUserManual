# FOUT Frequency Output

A programmable frequency generator circuit is provided for the counter/timer, and is described in the 9513 datasheet. It has an input source, a multi-stage decimal or BCD divider, and a user-programmable divider. All options are programmed through the Master Mode Register. The FOUT circuit of the 9513-1 is available on the FOUT pin on the GPIO-MM board’s I/O header. Its source can be the input or gate from counters 1-5 or any of the five internal frequency dividers built into the chip and driven by the clock. The FOUT circuit of the 9513-2 is not available externally.

