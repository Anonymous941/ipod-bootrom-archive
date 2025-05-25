# iPod Classic BootROM archive
This is an archive of iPod Classic/Nano (non-touch) BootROMs. This is very incomplete, so if you have a non-touch iPod running Rockbox, I would appreciate if you could dump it and open a PR! (or send it another way if you prefer)

These files are *not* device-specific meaning they don't contain any identifying information such as the serial number. `internal_eeprom.bin` does, so it won't be archived in this repository.

For more information, see https://www.rockbox.org/wiki/IpodFlash.html and https://freemyipod.org/wiki/Bootrom

### Dumping guide
1. Install Rockbox if you haven't already using [Rockbox Utility](https://www.rockbox.org/wiki/RockboxUtility#Download)  
It can be uninstalled right after, and only "bootloader" and "rockbox" need to be checked
2. From the main menu, go to "System > Debug (Keep Out!) > Dump ROM contents"
3. Plug your iPod into your computer and copy the file starting with either `internal_rom_` or `flash_rom_` (for example `internal_rom_000000-1FFFFF.bin`)

### Status
Archived:
 - A1238 - iPod 5th Generation (Video)

Not archived:
 - Everything else
