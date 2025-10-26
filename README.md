# zlib_aos
zlib for AmigaOS m68k and WarpOS.

version 1.3.1, January 22nd, 2024
Copyright (C) 1995-2024 Jean-loup Gailly and Mark Adler

## Building 
To build the `z.lib` linker library simply go the `amiga` folder and do `make -f Makefile.vbccWOS` or `make -f Makefile.vbcc68K`

## Notes
I had to patch `zconf.h` becuase vbcc defines `SEEK_SET`, `SEEK_CUR` and `SEEK_END` a little differently than the zlib expects. There is probably a better but it works. 