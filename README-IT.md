[![Italiano](http://upload.wikimedia.org/wikipedia/commons/7/70/Flag_of_italy.png "Italiano")](README-IT.md) [![English](http://upload.wikimedia.org/wikipedia/commons/e/e1/Union_Jack_22x16.png "English")](README.md)
[![Française](http://upload.wikimedia.org/wikipedia/commons/1/14/Flag_of_france.png "Française")](README-FR.md)  [![Espagnol](http://upload.wikimedia.org/wikipedia/commons/3/30/Flag_of_spain.png "Espagnol")](README-ES.md)
* * *
# recalbox-os
**Novità : v3.2.11 Corretti alcuni errori nei nomi dei controller, aggiunto tema zoid**

**Novità : v3.2.4 Nuovo file di configurazione recalbox.conf, nuovo sistema di avvio.**

**Novità : v3.2.3 Correzioni di errori vari, joystick analogico e L2/R2 aggiunti nellla configurazione joystick**

**Novità : recalboxOS è ora compatibile con RPi2 !**

**Novità : Tutte le informazioni su recalbox-os nella [WIKI IT](https://github.com/digitalLumberjack/recalbox-os/wiki/Home-%28IT%29)**

il super repository per recalbox.

La finalità di questo repository è di raggruppare i differenti progetti recalbox in uno, per fare ordine e rendere
piu' facile la compilazione del sistema.

## Presentazione
recalboxOS è un sistema integrato molto leggero, creato per essere eseguito su raspberryPi e raspberryPI 2.
 
Puoi trasformare il tuo raspberryPi in una piattaforma di emulatori (arcade game platform), con supporto per 16 sistemi differenti!

## Caratteristiche 
- Supporta Atari 2600, NES, Game Boy, Game Boy color, Game Boy Advance, Super Nintendo, Master System, Megadrive (Genesis), FBA, iMame4all, PCEngine, MSX1/2, PSX, SegaCD, Sega 32x, Sega SG1000, Famicom Disk System.
- Creato con buildroot, cosi il file di sistema pesa solamente 100MB compressi.
- Sistema di ripristino basato su NOOBS : rReinstalla direttamente dalla tua carta SD o recupera l'ultima versione via internet.
- Aggiornamenti online.
- Accesso da rete ai folder delle rom, degli screenshots e delle partite salvate.
- Partizione della rom in fat32 : compatibile con tutti i sistemi di gioco.
- Configurazione dei controller direttamente dall'interfaccia visuale : Configuri una volta solo e giochi ad ogni gioco.
- Musica di sottofondo nell'interfaccia visuale.
- Supporto integrato per controller Bluetooth PS3 e Shanwan (inserisci il controller, de-inserisci e gioca)
- Francese, inglese, Portoghese, Spagnolo, Tedesco e italiano e forse altre lingue supportate in futuro...se ci aiuti e partecipi pure tu.
- fantastica interfaccia EmulationStation2 basata su Aloshi 
- Versione ottimizzata di FBA con supporto per 4 giocatori 
- Puoi usare RPi GPIOs come controller

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

