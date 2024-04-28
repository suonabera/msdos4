# MS-DOS 4.00
On April 25, 2024, Microsoft released the source code to MS-DOS 4.00 along their previous releases of 1.25 and 2.00. (https://github.com/microsoft/MS-DOS)

The MS-DOS 4.00 release provided by Microsoft is in a crude state. To summarize, all source files have kept their Unix line endings, which causes errors in Microsoft's tools (For example, NOSRVBUILD will refuse to create .CL* files if the .SKL file has UNIX line endings. There's also the issue of SETENV.BAT not having the right paths for INCLUDE and LIB, among other problems, which were also related to the usage of extended ASCII characters in source code.

This repository provides a source tree which can be compiled, but no substantial analysis has been made on this code.

## Top level tree overview
``BIOS``: IO.SYS sources

``BOOT``: Floppy MBR sources

``CMD``: Userspace programs (COMMAND.COM et al) sources

``DEV``: Driver sources (printers, display adapters..)

``DOS``: MSDOS.SYS Sources

``H``: System related C headers

``INC``: System related ASM Includes

``LIB``: LIB.EXE binary

``MAPPER``: MAPPER.LIB sources

``MEMM``: Early EMM386 sources

``MESSAGES``: Internationalized strings for MSDOS.SYS

``SELECT``: SELECT (System installer) sources

``TOOLS``: MS C compiler 5.10, MASM 5.11, LINK 3.65, NMAKE 1.00.05 and other system development tools, along with their Assembly include files and their C headers.
