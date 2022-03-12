# Overview

The C256 machines (U, U+, and FMX) are based on the 65816 running at 14.318 MHz.

## Standard FLASH
* The C256 Kernal
* BASIC816
* MONITOR

## Languages
* C: The [WDC C compiler](https://www.westerndesigncenter.com/wdc/tools.php) is available for the 65816
* C: The [Calypsi C compiler](https://www.calypsi.cc) for 65816 by hth313
* TRSE: [TRSE](https://lemonspawn.com/turbo-rascal-syntax-error-expected-but-begin/) is being used to create games; see the 'c256-game-dev' channel on the discord.
* FORTH: [OF816](https://github.com/aniou/of816/tree/C256/platforms/C256) and [RetroForth](https://github.com/aniou/retro816) have both been ported.
* BASIC: all 65816 platforms include a brand new, clean-room BASIC for the 65816 Using [Foenix BASIC816](https://github.com/pweingar/BASIC816).
* Smalltalk: A full-blown Smalltalk-like environment is in development for the 65816. See Gadget's channel on Discord.
* Assembler: folks are using a variety of assemblers, tho 64tass appears to be the most popular.

## Operating Systems
For the more adventurous, several operating systems and desktop environments are in the works:

* CLI -- A platform agnostic kernel and CLI is in development for use across the entire Foenix line.
* FX/OS -- A Clean-Room GUI for the Foenix, written in C and presently compiling for the 65816.
* TinyCore -- A distributed Smalltalk-like environment being ported to the 65816.

## Music
The Foenix machines are an 8-bit musician's dream! All models include a TI SN76489, a Yamaha OPL3 (Sound Blaster), two Gideon FPGA SIDs, and a 16-bit CODEC. The FMX model further include MIDI ports, a Yamaha OPM, and a Yamaha OPN. You can also add two additional SIDs to any model. Turn your Foenix into the ultimate chip-tune machine, use it as a sound-module containing every classic FM-synth you every wanted, or directly implement your own MIDI transformations without having to wade through 30 years of operating system baggage!

Once again, Daniel Tremblay is here to get you started: [C256 VGM Player](https://github.com/dtremblay/c256-vgm-player)