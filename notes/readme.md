#### Preview, my scribbing to put in final Dev Docs, discard them

Computer starts:

1. BIOS copied from ROM to RAM
2. BIOS start code execution:
   - initialize hardware
   - runs some tests (POST = power-on self test)
3. BIOS searchers for an OS to start
4. BIOS loads and start OS

TWO WAYs:

1. Legacy booting

   - BIOS loads first sector of each bootable device into memory ( at location 0x7C00)
   - BIOS checks for 0xAA55 signature
   - If found, it start code execution

2. EFI
   - BIOS looks into special EFI partitions
   - Operating system must be compiled as an EFI program
