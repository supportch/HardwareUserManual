# 2. INTRODUCTION

Helios is an embedded single board computer in the PC/104 small form factor based on the DMP Vortex86DX family of all-in-one 486 processors. Helios integrates a complete embedded PC plus a full analog and digital data acquisition circuit into a single board. It is available in several models with different features:

| Model | Processor Speed | Memory | Math Coprocessor | Digital IO | Analog IO |
| :--- | :--- | :--- | :--- | :--- | :--- |
| HLV1000-256AV | 1GHz | 256MB | Yes | 40lines | Yes |
| HLV1000-256DV | 1GHz | 256MB | Yes | 16lines | No |
| HLV800-256AV | 800MHz | 256MB | Yes | 40lines | Yes |
| HLV800-256DV | 800MHz | 256MB | Yes | 16lines | No |

The board includes the following key system and data acquisition features:

_**Processor and Memory**_

* 1GHz or 800MHz Vortex86DX CPU 
* Integrated North Bridge/South Bridge, 10/100 Ethernet MAC/PHY, quad UART, and flash memory with embedded BIOS 
* 256MB DDR2 RAM system memory

_**Video Features**_

* PCI interface XGI Volari Z9S chip 
* Dedicated 32MB video memory 
* High performance 2D accelerator 
* 18-bit LVDS LCD interface, up to 1600 x 1200 
* CRT up to 1600 x 1200

_**Ethernet**_

* 10/100Mbps Ethernet circuit integrated into the Vortex processor chip 
* On-board transformer and termination network for direct connection to Ethernet cabling

_**Standard Peripheral Interfaces**_

* 4 16550-compatible RS-232 ports \(2 have RS-422/485 capability\) 
* 4 USB 2.0 ports 
* PS/2 keyboard and mouse ports _._ The BIOS supports a USB keyboard during BIOS initialization, and it also supports legacy keyboard emulation via USB for DOS. The USB ports can be used for keyboard and mouse at the same time that the PS/2 keyboard and mouse are connected.

_**Mass Storage**_

* 44-pin IDE connector for connection to UDMA-100 hard drive or solid state flashdisk module 
* Mounting spacer for rugged mounting of flashdisk in harsh environment applications 
* On-board 1.5MB virtual floppy drive in flash memory with FreeDOS pre-installed

_**Analog I/O**_

* 16 single-ended or 8 differential analog voltage inputs, 16-bit resolution 
* ±1.25V, ±2.5V, ±5V, ±10V, 0-1.25V, 0-2.5V, 0-5V, and 0-10V input ranges 
* 250KHz maximum aggregate A/D sampling rate 
* Programmable input ranges 
* Both bipolar and unipolar input ranges 
* Internal and external A/D triggering 
* 2048-sample A/D FIFO with programmable threshold 
* Auto-calibration of both A/D and D/A circuits 
* Four analog voltage outputs, 12-bit resolution 
* ±2.5V, ±5V, ±10V 0-5V, and 0-10V output ranges programmable in software

_**Digital I/O**_

* Up to 40 programmable digital I/O lines 
* Enhanced output current capability: +64mA maximum

_**Counter/Timers**_

* One 24-bit counter/timer for A/D sampling rate control 
* One 16-bit counter/timer for user counting and timing functions 
* Programmable gate and count enable 
* Internal \(10MHz\) or external clock source

_**Bus Interfaces**_

The Vortex86DX processor generates both PCI and ISA buses for I/O expansion. The 33MHz 32-bit PCI bus is used internally for the Ethernet circuit and is not brought out to a PCI-104 expansion connector. The 8MHz 16-bit ISA bus is brought out to a standard PC/104 stackthrough connector, enabling 16-bit and 8-bit modules to be installed either above or below the board. Interrupt and DMA performance is supported on the ISA bus. Up to 4 I/O boards can be installed on the ISA bus on Helios, depending on the loading characteristics of the add-on modules.

_**Battery Backup**_ 

Helios contains a backup battery for the real-time clock and BIOS settings. The battery is directly soldered to the board and provides a minimum 7 year backup lifetime at 25°C. For longer lifetime an external battery of 3.3V +/-10% may be attached to the board.

_**Watchdog Timer**_ 

Helios contains a watchdog timer \(WDT\) circuit with a software-programmable timer. The time delay can be programmed, and the timer can be retriggered with an I/O write command. When the timer times out, it will trigger an IRQ or system reset depending on the user configuration. 

_**Power Supply**_ 

Helios requires only +5V +/-5% for operation. The input power connector provides connections for optional provision of +/-12V and -5V for pass through to the ISA bus if needed for attached I/O modules.

