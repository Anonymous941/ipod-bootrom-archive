# iPod Classic BootROM archive
This is an archive of iPod Classic/Nano (non-touch) BootROMs. This is very incomplete, so if you have a non-touch iPod running Rockbox, I would appreciate if you could dump it and open a PR! (or send it another way if you prefer)

These files are *not* device-specific, meaning they don't contain any identifying information such as the serial number. `internal_eeprom.bin` does, so it won't be archived in this repository.

For more information, see https://www.rockbox.org/wiki/IpodFlash.html and https://freemyipod.org/wiki/Bootrom

### Credits
Here are the people who helped make this possible by dumping:
 - [Alex](https://alex-s-camera.neocities.org/): A1040, A1051 (January 2004), A1099
 - [Anonymous941](https://github.com/Anonymous941) (me): A1238

### Dumping guide
1. Install Rockbox if you haven't already using [Rockbox Utility](https://www.rockbox.org/wiki/RockboxUtility#Download)  
It can be uninstalled right after, and only "bootloader" and "rockbox" need to be checked
2. From the main menu, go to "System > Debug (Keep Out!) > Dump ROM contents"
3. Plug your iPod into your computer and copy the file starting with either `internal_rom_` or `flash_rom_` (for example `internal_rom_000000-1FFFFF.bin`)

### Status
Archived:
 - A1040 - iPod 3rd Generation
 - A1051 - iPod Mini (1st generation)
 - A1099 - iPod 4th Generation (Photo)
 - A1238 - iPod 5th Generation (Video)

Not archived:
 - Everything else

### Extracting
The individual files can be extracted from [`flashsplit.c`](https://github.com/Rockbox/rockbox/blob/efefe143bdfbf96095fd7b03efb6eb4af682c5d7/utils/ipod/flashsplit/flashsplit.c).  Despite it being part of Rockbox's git, you don't need to compile it with Rockbox, just download the single C file and compile it with `gcc flashsplit.c -o flashsplit`
