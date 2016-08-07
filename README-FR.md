[![English](http://upload.wikimedia.org/wikipedia/commons/e/e1/Union_Jack_22x16.png "English")](README.md)
[![Italiano](http://upload.wikimedia.org/wikipedia/commons/7/70/Flag_of_italy.png "Italiano")](README-IT.md) 
[![Français](http://upload.wikimedia.org/wikipedia/commons/1/14/Flag_of_france.png "Française")](README-FR.md)
[![Deutsch](http://upload.wikimedia.org/wikipedia/commons/4/4b/Flag_of_germany.png "Deutsch")](README-DE.md)
[![Portugues](http://upload.wikimedia.org/wikipedia/commons/a/aa/Flag_of_Portugal_icon.png "Portugues")](README-PT.md)
[![Español](http://upload.wikimedia.org/wikipedia/commons/3/30/Flag_of_spain.png "Español")](README-ES.md)
[![Türkçe](https://upload.wikimedia.org/wikipedia/commons/thumb/b/b4/Flag_of_Turkey.svg/24px-Flag_of_Turkey.svg.png "Türkçe")](README-TR.md)
****
# recalbox-os
**Nouveauté : v3.2.11 Correction du bug des contrôleurs ayant le même nom, ajout du thème zoid**

**Nouveauté : v3.2.4 Nouveau fichier recalbox.conf, nouveau système de démarrage.**

**Nouveauté : v3.2.3 Correction de bugs, stick analogique et L2/R2 ajouté dans la configuration du joystick**

**Nouveauté : recalboxOS est maintenant compatible avec le RPi2 !**

**Nouveauté : retrouvez toutes les informations à propos de recalbox-os sur le [WIKI](https://github.com/digitalLumberjack/recalbox-os/wiki)**

Le super repo pour recalbox.

Le principe de ce repo est de rassembler tous les projets tournant autour de recalbox en un seul à des fins de clarification et pour rendre la compilation du système plus aisée.

## Présentation
recalboxOS est un système d'exploitation embarqué crée pour être léger et tourner sur RaspberryPi et RaspberryPI 2.

Avec, vous pouvez transformer votre RaspberryPi en plate-forme d'émulation supportant jusqu'à 32 machines différentes.


## Fonctionnalités 
- Support ce Atari 2600, Atari 7800, NES, Game Boy, Game Boy color, Game Boy Advance, Super Nintendo, Famicom Disk System, Master System, Megadrive (Genesis), Gamegear, Game and Watch, Lynx, NeoGeo, NeoGeo Pocket, FBA (subset), iMame4all (subset), PCEngine, Supergrafx, MSX1/2, PSX, Sega Cd, Sega 32X, Sega SG1000, Playstation, ScummVM, Vectrex, VirtualBoy, Wonderswan
- Compilé avec buildroot, de cette façon l'OS ne pèse que 100MB une fois compressé.
- Système de restauration basé sur NOOBS : vous pouvez le réinstaller directement depuis la carte SD ou récupérer la dernière version depuis internet.
- Mises à jour via internet
- Accès par le réseau aux dossiers des ROMs, des captures d'écran et des sauvegardes.
- Partition des ROMs en FAT32: compatibilité inter systèmes garantie !
- Configuration des manettes dans l'interface : configurez une fois, jouez partout !
- Musique d'ambiance dans l'interface
- Support inclus des normes Bluetooth PS3 et Shanwan (branchement d'une manette, débranchez et jouez)
- Français, Anglais, Portugais (merci à mgoulart), Espagnol, Allemand, Italien et d'autres si vous participez à la traduction du projet.
- Interface basée sur la géniale EmulationStation2 par Aloshi
- FBA optimisé jusqu'à 4 joueurs
- Possibilité d'utiliser les ports GPIO du RaspberryPi pour la manette


## Projets
**recalboxOS** est le principal projet, regroupant les 3 sous projets qui composent le système

- **recalbox-buildroot** : 
https://github.com/digitalLumberjack/recalbox-buildroot (branch recalbox)  
Le projet recalbox-buildroot est celui qui crée le Linux qui tourne sur la recalbox.
Vous pouvez compiler ce projet, puis copiez le résultat sur une carte SD que vous avez formaté pour la mettre dans un RPi. Mais il existe une meilleure solution, appelée recalbox-rescue.

- **recalbox-rescue** : 
https://github.com/digitalLumberjack/recalbox-rescue (branch recalbox)  
A l'instar de NOOBS de l'équipe du Raspberry Pi, recalbox-rescue vous permet d'installer facilement retroboxOS et d'avoir une partition de secours sur votre carte SD. C'est un autre système d'exploitation très léger qui va télécharger recalboxOS, formater votre carte SD et l'installer pour vous, tout en vérifiant sur internet si une version plus récente est disponible avant l'installation.

- **recalbox-emulationstation** : 
https://github.com/digitalLumberjack/recalbox-emulationstation/tree/recalbox-buildroot  
Basée sur la géniale EmulationStation2 par Aloshi, l'interface graphique a été quelque peu modifiée pour inclure une musique de fond au format ogg, la sélection du langage, la configuration des manettes et une fonction de mise à jour
