[![Italiano](http://upload.wikimedia.org/wikipedia/commons/7/70/Flag_of_italy.png "Italiano")] [![English](http://upload.wikimedia.org/wikipedia/commons/e/e1/Union_Jack_22x16.png "English")](README.md)
[![Française](http://upload.wikimedia.org/wikipedia/commons/1/14/Flag_of_france.png "Française")](README-FR.md)  [![Espagnol](http://upload.wikimedia.org/wikipedia/commons/3/30/Flag_of_spain.png "Espagnol")](README-ES.md)
* * *
# recalbox-os
**Novità : v3.2.11 Corrected same name controller bug, aggiunto tema zoid**

**Novità : v3.2.4 New recalbox.conf system, new boot system.**

**Novità : v3.2.3 Bug corrections, Analog joystick and L2/R2 added in joystick config**

**Novità : recalboxOS is now compatible with RPi2 !**

**Novità : get all infos on recalbox-os on the [WIKI](https://github.com/digitalLumberjack/recalbox-os/wiki)**

il super repository per recalbox.

La finalità di questo repository è di raggruppare i differenti progetti recalbox in uno, per fare ordine e rendere
piu' facile la compilazione del sistema.

## Presentazione
recalboxOS is a light embedded system created to run on the raspberryPi and raspberryPI 2.

You can transform your rpi in an emulation platform, supporting up to 16 systems !


## Caratteristiche 
- Supports Atari 2600, NES, Game Boy, Game Boy color, Game Boy Advance, Super Nintendo, Master System, Megadrive (Genesis), FBA, iMame4all, PCEngine, MSX1/2, PSX, SegaCD, Sega 32x, Sega SG1000, Famicom Disk System.
- Build with buildroot, so the root file system is only 100MB compressed.
- Rescue system based on NOOBS : reinstall directly from your sd card or get the last version from the net
- Online update
- Network access to rom folder, screenshots, saves.
- fat32 rom partition : compatible with all systems
- Controller configuration in the frontend : configure once, play everywhere.
- Background frontend music
- PS3 and Shanwan Bluetooth built-in support (plug a controller, unplug and play)
- French, English, Portugues (thanks to mgoulart), Spanish, German, italiano and maybe other to come if you participate.
- Frontend based on Aloshi great EmulationStation2
- FBA optimized version with 4 player support (yeah Dungeons and Dragons)
- Use RPi GPIOs as controllers

## Progetti
**recalboxOS** è il porgetto principale, aggrega i 3 sotto-progetti che compongono il sistema :

- **recalbox-buildroot** : 
https://github.com/digitalLumberjack/recalbox-buildroot (branch recalbox)  
The recalbox-buildroot project is the buildroot system. It create the whole linux os that will run on the recalbox.
You could compile this project, then copy output files to a manually formatted SD card to run the system on a raspberryPi. But there is a better way, called recalbox-rescue.

- **recalbox-rescue** : 
https://github.com/digitalLumberjack/recalbox-rescue (branch recalbox)  
Based on the awesome NOOBS from rpi team, the recalbox rescue allows you to easily install retroboxOS and have a rescue partition on your SD card. It's an other minimal OS, that will download retroboxOS, format your SD card, and install the system for you.  
It will check if a new version is available from the net, before installing SD card version. 

- **recalbox-emulationstation** : 
https://github.com/digitalLumberjack/recalbox-emulationstation/tree/recalbox-buildroot  
Based on the Aloshi awesome emulationstation 2, the frontend has been a little modified to have ogg bg music, language selection, update support and controller configuration.

