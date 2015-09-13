[![English](http://upload.wikimedia.org/wikipedia/commons/e/e1/Union_Jack_22x16.png "English")](README.md)
[![Italiano](http://upload.wikimedia.org/wikipedia/commons/7/70/Flag_of_italy.png "Italiano")](README-IT.md) 
[![Français](http://upload.wikimedia.org/wikipedia/commons/1/14/Flag_of_france.png "Française")](README-FR.md)
[![Deutsch](http://www.flagsoftheworld.eu/images/2/flag-of-germany.png "Deutsch")](README-DE.md)
[![Portugues](http://www.flagsoftheworld.eu/images/2/flag-of-portugal.png "Portugues")](README-PT.md)
[![Español](http://upload.wikimedia.org/wikipedia/commons/3/30/Flag_of_spain.png "Español")](README-ES.md)
****
# recalbox-os
**Neu : V3.2.11 - Fehler mit "gleicher Controller Name" wurde korrigiert, Zoid Theme hinzugefügt**

**Neu : V3.2.4  - Neues recalbox.conf System, neues Boot-System**

**Neu : V3.2.3  - Fehlerkorrekturen, Analog Joystick und L2/R2 zu Joystick-Konfiguration hinzugefügt**

**Neu : recalboxOS ist jetzt kompatibel mit RPi2!**

**Neu : Alle Informationen zum recalbox-os im [WIKI](https://github.com/digitalLumberjack/recalbox-os/wiki)**

Das Super "Repository" für recalbox.

Ziel dieses "Repository" ist die Neu-Gruppierung der verschiedenen recalbox-Projekte zu einem Ganzen und die 
Vereinfachung das System zu kompilieren.
## Vorstellung
recalboxOS ist ein leichtes, integriertes System, entwickelt für RaspberryPi und RaspberryPI 2.

Du kannst Deinen RPI in eine Emulations Plattform verwandeln, es werden bis zu 16 Systeme unterstützt!

## Eigenschaften
- Unterstützung für Atari 2600, NES, Game Boy, Game Boy Color, Game Boy Advance, Super Nintendo, Master System, Megadrive (Genesis), FBA, iMame4all, PCEngine, MSX1/2, PSX, SegaCD, Sega 32x, Sega SG1000, Famicom Disk System
- Erstellt mit "buildroot", dadurch ist das Haupt-Datei-System auf nur 100MB komprimiert
- Rettungssystem basierend auf NOOBS : Neuinstallation direkt von Deiner SD-Karte oder hole Dir die letzte Version aus dem Netz
- Online-Aktualisierung
- Netzwerk-Zugriff auf ROM-Verzeichnis, Screenshots, Saves, etc.
- Fat32 ROM-Partition : Mit allen Systemen kompatibel
- Controller-Konfiguration im Front-End : Einmalige Konfiguration, überall spielen
- Hintergrundmusik im Front-End
- Integrierte PS3 und ShanWan Bluetooth Unterstützung (Einen Controller anschliessen, wieder entfernen und spielen)
- Französisch, Englisch, Portugiesisch (Dank an mgoulart), Spanisch, Deutsch und mit Unterstützung vielleicht noch mehr
- Front-End basierend auf dem großartigen EmulationStation2 von Aloshi
- FBA optimierte Version mit Unterstützung für bis zu 4 Spieler (Yeah Dungeons and Dragons)
- Benutze RPI GPIOs als Contoller

## Projekte
**recalboxOS** ist das Haupt-Projekt, bestehend aus 3 Unter-Projekten, die das System bilden :

- **recalbox-buildroot** :
https://github.com/digitalLumberjack/recalbox-buildroot (branch recalbox)                                                   
Das recalbox-buildroot Projekt ist ein "buildroot" System. Es erstellt ein komplettes Linux Betriebssystem, dass auf recalbox lauffähig ist.
Du kannst dieses Projekt kompilieren, dann die Ausgabe-Dateien auf eine manuell formartierte SD-Karte kopieren, um das System auf einem RaspberryPi zu starten. 
Es gibt aber noch einen besseren Weg, das recalbox-rescue System.

- **recalbox-rescue** : 
https://github.com/digitalLumberjack/recalbox-rescue (branch recalbox)                                                      
Basierend auf dem grandiosen NOOBS vom RPI Team, ermöglicht Dir das recalbox-rescue System eine einfache Installation von RecalboxOS und einer Rettungs-Partition auf Deiner SD-Karte. 
Es ist ein anderes, kleines Betriebssystem, welches retroboxOS runterlädt, Deine SD-Karte formatiert und das System für Dich installiert.  
Bevor die SD-Karten Version installiert wird, wird überprüft, ob eine neue Version im Internet verfügbar ist.

- **recalbox-emulationstation** :
https://github.com/digitalLumberjack/recalbox-emulationstation/tree/recalbox-buildroot
Basierend auf dem grandiosen EmulationStation2 von Aloshi, wurde das Front-End ein wenig modifiziert, 
um ogg Hintergrundmusik, Sprachauswahl, Update Unterstützung und Controller-Konfiguration zu ermöglichen.
