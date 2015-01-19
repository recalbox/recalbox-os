# retrobox-os
**New : get all infos on retrobox-os on the [WIKI](https://github.com/digitalLumberjack/retrobox-os/wiki)**

The super repository for retrobox.

This repository purpose is the regroup the differents retrobox projects in one to clarify and make it more easy to compile the system.

## Presentation
retroboxOS is a light embedded system created to run on the raspberryPi.

You can transform your rpi in an emulation platform, supporting up to 12 systems !


## Features 
- Supports Atari 2600, NES, Game Boy, Game Boy color, Game Boy Advance, Super Nintendo, Master System, Megadrive (Genesis), FBA, iMame4all, PCEngine, MSX1/2, PSX (not so much right now)
- Build with buildroot, so the root file system is only 70MB compressed.
- Rescue system based on NOOBS : reinstall directly from your sd card or get the last version from the net
- Online update
- Network access to rom folder, screenshots, saves.
- fat32 rom partition : compatible with all systems
- Controller configuration in the frontend : configure once, play everywhere.
- Background frontend music
- PS3 and Shanwan Bluetooth built-in support (plug a controller, unplug and play)
- French, English, Portugues (thanks to mgoulart) and maybe other to come if you participate.
- Frontend based on Aloshi great EmulationStation2
- FBA optimized version with 4 player support (yeah Dungeons and Dragons)

## Projects
**retroboxOS** is the main project, that aggregate the 3 sub-projects composing the system :

- **retrobox-buildroot** : 
https://github.com/digitalLumberjack/retrobox-buildroot (branch retrobox)  
The retrobox-buildroot project is the buildroot system. It create the whole linux os that will run on the retrobox.
You could compile this project, then copy output files to a manually formatted SD card to run the system on a raspberryPi. But there is a better way, called retrobox-rescue.

- **retrobox-rescue** : 
https://github.com/digitalLumberjack/retrobox-rescue (branch retrobox)  
Based on the awesome NOOBS from rpi team, the retrobox rescue allows you to easily install retroboxOS and have a rescue partition on your SD card. It's an other minimal OS, that will download retroboxOS, format your SD card, and install the system for you.  
It will check if a new version is available from the net, before installing SD card version. 

- **retrobox-emulationstation** : 
https://github.com/digitalLumberjack/retrobox-emulationstation/tree/retrobox-buildroot  
Based on the Aloshi awesome emulationstation 2, the frontend has been a little modified to have ogg bg music, language selection, update support and controller configuration.

