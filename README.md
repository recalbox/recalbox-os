# retrobox-os
The super repository for retrobox.

This repository purpose is the regroup the differents retrobox projects in one to clarify and make it more easy to compile the system.

## Presentation
retroboxOS is a light embedded system created to run on the raspberryPi.

You can transform your rpi in an emulation platform, supporting up to 12 systems !
The retrobox is designed to work with a PS3 or Shanwan controller, or USB controllers. You cannot play with a keyboard for now.


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
- French and English, maybe other to come if you participate.
- Frontend based on Aloshi great EmulationStation2
- FBA optimized version with 4 player support (yeah Dungeons and Dragons)

## Installation ##
You can install the retroboxOS on a fat32 formatted sd card.
Download retroboxOS.zip from https://github.com/digitalLumberjack/retrobox-os/releases and copy all unzipped files to your sd.

Then boot your rpi and install the retroboxOS !

## Usage ##
On first boot, you will have a message specifying that no game has been found. Just copy your roms from your local network, or unplug the SD and put it in your card reader. A share partition is available with a rom folder, where you must put your files.

Check the manuals :

French : https://docs.google.com/document/d/1DyJmmb4YhigGI3po764lMO25ertI2ER3CPNk0jsikW0/edit?usp=sharing

English (very sorry for the translation) : https://docs.google.com/document/d/1Ksqhg56HF7nzS8k8Vy_7j2gqw6tCUgcWWGaTBmEh70c/edit?usp=sharing

Do not hesitate to correct me by commenting.

## Compilation ##

You have 3 projects composing the whole system :
- *retrobox-emulationstation* : 
https://github.com/digitalLumberjack/retrobox-emulationstation (branch retrobox-buildroot)
Based on the Aloshi awesome emulationstation 2, the frontend has been  modified to have ogg bg music, language selection, update support and controller configuration. 

- *retrobox-buildroot* : 
https://github.com/digitalLumberjack/retrobox-buildroot (branch retrobox)
Based on the rmaz awesome emulator-buildroot, the retrobox system can be build from sources from the above url. 
The fact that it is based on buildroot make the system very light and optimized. 

- *retrobox-rescue* : 
https://github.com/digitalLumberjack/retrobox-rescue (branch retrobox)
Based on the awesome NOOBS from rpi team, the retrobox rescue allows you to easily install retroboxOS and have a rescue partition, just in case :)
If you wire an ethernet cable, it will check if a new version is available from the net.

So how it works basically :

- The **retrobox-buildroot** create a fully functional system. This system is configured to run on a SD partitioned with 3 partition : 
  - boot (200MB) : fat32 partition containing boot files and kernel
  - root (2GB): ext2/4 partition containing the system
  - share (MAXIMUM SIZE) : fat32 partition on which all roms and save are placed.

  So if you want to install the system without retrobox-rescue, you will have to create your partitions and copy manually binary files created by retrobox-buildroot compilation on the SD (not recommended)

- The **retrobox-rescue** create a minimal system that will boot on rpi and install the retrobox-buildroot, either from the sd card or from the net.
It create many partitions and allow you to install other systems in dual boot !


You can make it easy by downloading `createRetroboxOS.sh` form the last release https://github.com/digitalLumberjack/retrobox-os/releases and launch it from a terminal (you will have to edit package installation if you are not on a debian based distribution)
It will compile retrobox-buildroot, retrobox-rescue, and create all necessary files in a folder called SDCONTENT.
Then copy all the files in SDCONTENT to your sd card.


