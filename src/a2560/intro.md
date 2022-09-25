# Overview

The A2560 machines (A2560U, A2560K) are 680x0 based machines. The A2560U uses a 68000 running at 20MHz; the A2560K uses a 68040 running at 40MHz.

The 68k based machines are quite new, so not as much exists for them yet, but the 68k enjoys a huge body of pre-existing software that will easily port to the Foenix!

## Standard FLASH

* The C based "MCP" Kernel
* A simple DOS-like CLI

## Languages

### C
[Calypsi](https://www.calypsi.cc/) - Håkan Thörngren has created a modern C compiler suite for the Foenix line of computers, called Calypsi. Calypsi is the best option for the Foenix as it can make use of its math-copro and supports processors used by other computers of the product line. The development of Calypsi is active, and documentation is excellent. You can find out more on the "ht313-channel" of the Foenix Retro Systems [Discord](https://discord.gg/gZrcCqqY) server.

[VBCC](http://www.compilers.de/vbcc.html) - Dr Volker Barthelmann's C compiler is also used by the community. Dashewie maintains a [VBCC target](https://github.com/daschewie/Foenix_vbcc_target).

The FoenixMCP has an Elf loader so in principle it is possible to use "any" compiler producing ELF, like GCC. For example, [Thorsten Otto](http://tho-otto.de/crossmint.php) produces m68k [GCC](https://gcc.gnu.org/) suites for the Atari ST which might be used.

### BASIC
BASIC: a port of MMBASIC is in progress.

## Operating Systems
For the more adventurous, several operating systems and desktop environments are in the works.

### FoenixMCP


* CLI -- A simple DOS-like CLI is included
* A port of EmuTOS is in progress, see the Discord for daily updates!