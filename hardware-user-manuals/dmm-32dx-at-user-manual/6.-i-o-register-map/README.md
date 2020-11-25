# 6. I/O REGISTER MAP

Diamond-MM-32DX-AT occupies 16 bytes in the system I/O address space. Direct register access is not required if you are using the Universal Driver™ software that ships with the board. The driver handles all board access and provides a high-level set of functions to simplify programming. The information presented here and in the next chapter is intended to provide a detailed description of the board’s features and operation, as well as for programmers who are not using the Universal Driver software. The DMM-32DX-AT FPGA I/O register map, while remaining backwards compatible with the DMM-32-AT, offers more features to the user. New features that did not exist in the DMM-32-AT are marked boldface,or noted as an enhanced feature. Registers 12 – 15 provide a window into several pages for access to additional registers without requiring additional I/O address space. Page selection is done via control bits in register 8.

[ ](6.11-page-7-d-a-output-channel-control.md)

