# C256 FMX

The C256 FMX (Foenix Music eXpansion) includes all of the standard features, plus the following:

* 4MB System RAM
* 4MB Video RAM
* MIDI in/out
* YM2151 Sound
* YM6212 Sound
* 2x 9-wire RS232 ports
* EPP parallel port
* 1.44 MB floppy drive
* Two additional joystick ports

The FMX further supports either the ESID (2x SID + ethernet) or EVID (2nd video + ethernet) expansion cards.

## Memory Map
| Start Address | End Address | Descrtiption |
|---------------|-------------|---------------|
| $00:0000      | $00:00FF    | RAM (Reserved by Kernel) |
| $00:0100      | $00:0107    | 16Bits Unsigned Multiplication (FIXED MATH CORE) |
| $00:0108      | $00:010F    | 16Bits Signed Multiplication (FIXED MATH CORE) |
| $00:0110      | $00:0117    | 16Bits Unsigned Division (FIXED MATH CORE) |
| $00:0118      | $00:011F    | 16Bits Sgned Division (FIXED MATH CORE) |
| $00:0120      | $00:012F    | 32Bits Addition/Substraction (FIXED MATH CORE) |
| $00:0140      | $00:015F    | Interrupt Controller |
| $00:0160      | $00:017F    | Timers |
| $00:0180      | $00:01FF    | SDMA (System DMA) |
| $00:0200      | $00:0FFF    | RAM (Reserved by Kernel) |
| $00:1000      | $3F:FFFF    | RAM |
| $AE:0000      | $AE:FFFF    | Expansion Chip Select |
| $AF:0000      | $AF:00FF    | VICKY II Control Registers |
| $AF:0100      | $AF:013F    | Tiles Control Registers |
| $AF:0140      | $AF:014F    | Bitmap Control Registers |
| $AF:0200      | $AF:03FF    | Sprites Control Registers |
| $AF:0400      | $AF:04FF    | VDMA Control Registers |
| $AF:0500      | $AF:06FF    | Mouse Pointer Graphic Mem |
| $AF:0700      | $AF:0707    | Mouse Pointer Control Registers |
| $AF:070B      | $AF:070F    | C256 FPGA Version and date |
| $AF:0800      | $AF:080F    | RTC |
| $AF:1000      | $AF:13FF    | SuperIO (Floppy/LPT/COM1/COM2/MPU) (FMX Only) |
| $AF:1F00      | $AF:173F    | Text Mode Color Palette (Foreground) |
| $AF:1F40      | $AF:1F7F    | Text Mode Color Palette (Background) |
| $AF:2000      | $AF:23FF    | Graphic Mode Color Palette0 |
| $AF:2400      | $AF:27FF    | Graphic Mode Color Palette1 |
| $AF:2800      | $AF:2BFF    | Graphic Mode Color Palette2 |
| $AF:2C00      | $AF:2FFF    | Graphic Mode Color Palette3 |
| $AF:3000      | $AF:33FF    | Graphic Mode Color Palette4 |
| $AF:3400      | $AF:37FF    | Graphic Mode Color Palette5 |
| $AF:3800      | $AF:3BFF    | Graphic Mode Color Palette6 |
| $AF:3C00      | $AF:3FFF    | Graphic Mode Color Palette7 |
| $AF:4000      | $AF:40FF    | GAMMA Correction - Blue Channel |
| $AF:4100      | $AF:41FF    | GAMMA Correction - Green Channel |
| $AF:4200      | $AF:42FF    | GAMMA Correction - Red Channel |
| $AF:4000      | $AF:7FFF    | Tile Map Memory |
| $AF:8000      | $AF:87FF    | FONT Set Memory |
| $AF:A000      | $AF:BFFF    | Text Display Memory |
| $AF:C000      | $AF:DFFF    | Text Color Memory |
| $AF:E200      | $AF:E2FF    | FLOAT MATH CORE |
| $AF:E400      | $AF:E4FF    | FPGA SID (3 Channels for Now) |
| $AF:E600      | $AF:E7FF    | OPL3 (YMF262) |
| $AF:E800      | $AF:E81F    | Trinity CHIP (Joystick and DIP switches) |
| $AF:E830      | $AF:E83F    | UNITY CHIP (IDE) |
| $AF:E840      | $AF:E87F    | RESERVED (TBD) |
| $AF:E880      | $AF:E887    | GABE Control Registers (LED, Buzzer, Etc) |
| $AF:E900      | $AF:E9FF    | CODEC |
| $AF:EA00      | $AF:EAFF    | SDCARD Controller |
| $AF:EC00      | $AF:EDFF    | RESERVED (TBD) |
| $AF:EE00      | $AF:EFFF    | RESERVED (TBD) |
| $AF:F000      | $AF:F0FF    | OPM (YM2151) (FMX Only) |
| $AF:F100      | $AF:F1FF    | PSG (SN76489) |
| $AF:F200      | $AF:F3FF    | OPN2 (YM2612) (FMX Only) |
| $B0:0000      | $EF:FFFF    | VICKY II Video Memory |
| $F8:0000      | $FF:FFFF    | KERNEL FLASH (not CPU Accessible) |