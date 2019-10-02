Building the Commander X16 Emulator
===================================

The emulator itself is dependent only on SDL2. However, to run the emulated system you will also need a compatible `rom.bin` ROM image. This will be
loaded from the directory containing the emulator binary, or you can use the `-rom .../path/to/rom.bin` option.

> __WARNING:__ Older versions of the ROM might not work in newer versions of the emulator, and vice versa.

You can build a ROM image yourself using the [build instructions][x16-build] in the [x16-rom] repo. The `rom.bin` included in the [_latest_ release][releases] of the emulator may also work with the HEAD of this repo, but this is not guaranteed.


Emulator Build
---------------

### Linux

The SDL2 development package is available as a distribution package with most major versions of Linux:
- Red Hat: `yum install SDL2-devel`
- Debian: `apt-get install libsdl2-dev`

Type `make` to build the source. The output will be `x16emu` in the current directory.

### WebAssembly

Steps for compiling WebAssembly/HTML5 can be found [here][webassembly].



<!-------------------------------------------------------------------->
[cc65]: https://cc65.github.io/
[releases]: https://github.com/commanderx16/x16-emulator/releases
[x16-build]: https://github.com/commanderx16/x16-rom#releases-and-building
[x16-rom]: https://github.com/commanderx16/x16-rom
[webassembly]: webassembly/WebAssembly.md
