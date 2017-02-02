[![English](http://upload.wikimedia.org/wikipedia/commons/e/e1/Union_Jack_22x16.png "English")](README.md)
[![Italiano](http://upload.wikimedia.org/wikipedia/commons/7/70/Flag_of_italy.png "Italiano")](README-IT.md) 
[![Français](http://upload.wikimedia.org/wikipedia/commons/1/14/Flag_of_france.png "Française")](README-FR.md)
[![Deutsch](http://upload.wikimedia.org/wikipedia/commons/4/4b/Flag_of_germany.png "Deutsch")](README-DE.md)
[![Portugues](http://upload.wikimedia.org/wikipedia/commons/a/aa/Flag_of_Portugal_icon.png "Portugues")](README-PT.md)
[![Español](http://upload.wikimedia.org/wikipedia/commons/3/30/Flag_of_spain.png "Español")](README-ES.md)
[![Türkçe](https://upload.wikimedia.org/wikipedia/commons/thumb/b/b4/Flag_of_Turkey.svg/24px-Flag_of_Turkey.svg.png "Türkçe")](README-TR.md)
****
# recalboxOs
  
Das Super "Repository" für recalbox.

**Alle Anleitungen zu recalboxOs gibt es im [WIKI](https://github.com/digitalLumberjack/recalbox-os/wiki)**
  
**Weitere Hilfe sowie Inspiration findest du im [FORUM](https://forum.recalbox.com)**

Ziel dieses "Repository" ist die Neu-Gruppierung der verschiedenen recalbox-Projekte zu einem Ganzen und die 
Vereinfachung das System zu kompilieren.
  
## Vorstellung
recalboxOS ist ein leichtes, integriertes System, welches für folgende Plattformen entwickelt wird:  
  
* Raspberry Pi 1
* Raspberry Pi 2
* Raspberry Pi 3
* Odroid XU4
* PC (x86)
* PC (x86_64)

Du kannst deine Hardware in eine Retro-Gamekonsole verwandeln, die mehr als 40 verschiedene Systeme unterstützt.

## Eigenschaften
Momentan werden Emulatoren für folgende Systeme unterstützt:  
  
- Arcade
- Arcade Classic
- NES (Nintendo Entertainment System)
- FDS (Famicom Disk System)
- SNES (Super Nintendo Entertainment System)
- Nintendo 64
- Game Boy
- Game Boy Color
- Game Boy Advance
- Nintendo Game and Watch
- Nintendo Virtual Boy
- Play Station 1
- Atari 2600
- Atari 7800
- Atari ST
- Atari Lynx
- NEC PC Engine (TurboGrafx 16)
- NEC Supergrafx
- Sega Master System
- Sega Megadrive (Genesis)
- Sega SG1000
- Sega 32x
- Sega CD
- Sega Game Gear
- MSX 1
- MSX 2
- MSX 2+
- ScummVM
- PRBOOM
- Vectrex
- Wonderswan Color
- NeoGeo Pocket Color
- NeoGeo/NeoGeo CD
- Philips Odyssey 2 Videopac
- Amstrad CPC
- Sinclair ZX81
- Sinclair ZX Spectrum
- Moonlight   
  
Das System wird laufend durch neue Emulatoren erweitert (je nach Rechenleistung der verwendeten und kompatiblen Hardware).   
   
- Erstellt mit "buildroot". Dadurch ist das Haupt-Dateisystem nur 150MB groß
- Rettungssystem basierend auf NOOBS: Neuinstallation direkt von der SD-Karte, oder lade die neueste Version von recalbox.com herunter.
- WiFi Unterstützung (Mit Dongle oder beim Raspberry Pi 3 intern)
- Online-Systemaktualisierung
- Netzwerkzugriff auf das ROM-Verzeichnis, auf Screenshots, Spielstände, etc.
- KODI Media Center
- Controllerkonfiguration im Frontend: Einmalige Konfiguration, für jedes System nutzbar
- Eingebaute PS3, Xbox360, 8Bitdo und Bluetooth (Dongle) Unterstützung (Controller anschliessen und spielen)
- In mehreren Sprachen verfügbar: Deutsch, Englisch, Französisch, Portugiesisch, Spanisch, Schwedisch, Italienisch, Türkisch, Chinesisch und bei Unterstützung durch die Community vielleicht auch bald noch mehr
- Frontend basiert auf dem großartigen EmulationStation2 von Aloshi
- Hintergrundmusik im Frontend
- FBA-Optimierte Version mit Unterstützung für bis zu 4 Spieler
- GPIO Treiber für Arcade, original NES, SNES, Megadrive, PSX oder XinMo Controller
- Lieblingsspiele als Favoriten abspeichern.
- [Miroof's Virtual Gamepad] (https://github.com/miroof/node-virtual-gamepads) Unterstützung (Smartphone als Controller benutzen)

## Projekte
**recalboxOS** ist das Haupt-Projekt, bestehend aus 3 Unter-Projekten, die das System bilden:

- **recalbox-buildroot**:
https://github.com/digitalLumberjack/recalbox-buildroot (branch recalbox)                                                   
Das recalbox-buildroot Projekt ist ein "buildroot" System. Es erstellt ein komplettes Linux Betriebssystem, dass auf recalbox lauffähig ist.
Du kannst dieses Projekt kompilieren, dann die Ausgabe-Dateien auf eine manuell formartierte SD-Karte kopieren, um das System auf einem Raspberry Pi oder kompatibler Hardware zu starten. 
Es gibt aber noch einen besseren Weg, das recalbox-rescue System.

- **recalbox-rescue**: 
https://github.com/digitalLumberjack/recalbox-rescue (branch recalbox)                                                      
Basierend auf dem grandiosen NOOBS vom RPI Team, ermöglicht Dir das recalbox-rescue System eine einfache Installation von RecalboxOS und einer Rettungs-Partition auf Deiner SD-Karte. 
Es ist ein anderes, kleines Betriebssystem, welches retroboxOS runterlädt, Deine SD-Karte formatiert und das System für Dich installiert.  
Bevor die SD-Karten Version installiert wird, wird überprüft, ob eine neue Version im Internet verfügbar ist.

- **recalbox-emulationstation**:
https://github.com/digitalLumberjack/recalbox-emulationstation/tree/recalbox-buildroot
Basierend auf dem grandiosen EmulationStation2 von Aloshi, wurde das Front-End ein wenig modifiziert, 
um _ogg_ Hintergrundmusik, Sprachauswahl, Update Unterstützung und Controller-Konfiguration zu ermöglichen.
