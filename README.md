# MS-DOS 4.00
On April 25, 2024, Microsoft released the source code to MS-DOS 4.00 along their previous releases of 1.25 and 2.00. (https://github.com/microsoft/MS-DOS)

The MS-DOS 4.00 release provided is in a crude state. To summarize, all source files have kept their Unix line endings, which causes errors in Microsoft's tools. There's also the issue of GETMSG.ASM having some weird comment which halts MASM, and SETENV.BAT not having the right paths for INCLUDE and LIB.

This repository provides a source tree which can be compiled, but no more analysis on this has been made.
