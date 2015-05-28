[![English](http://upload.wikimedia.org/wikipedia/commons/e/e1/Union_Jack_22x16.png "English")](README.md)
[![Italiano](http://upload.wikimedia.org/wikipedia/commons/7/70/Flag_of_italy.png "Italiano")](README-IT.md)
[![Français](http://upload.wikimedia.org/wikipedia/commons/1/14/Flag_of_france.png "Française")](README-FR.md)
[![Portugues](http://www.flagsoftheworld.eu/images/2/flag-of-portugal.png "Portugues")](README-PT.md)
[![Espagnol](http://upload.wikimedia.org/wikipedia/commons/3/30/Flag_of_spain.png "Espagnol")](README-ES.md)
* * *
# recalbox-os
#### Piattaforma di emualzione arcade per raspberryPi!
**Novità : v3.2.11 Corretti alcuni errori nei nomi dei controller, aggiunto tema zoid**

**Novità : v3.2.4 Nuovo file di configurazione recalbox.conf, nuovo sistema di avvio.**

**Novità : v3.2.3 Correzioni di errori vari, joystick analogico e L2/R2 aggiunti nellla configurazione joystick**

**Novità : recalboxOS è ora compatibile con RPi2 !**

**Novità : Tutte le informazioni su recalbox-os nella [WIKI IT](https://github.com/digitalLumberjack/recalbox-os/wiki/Home-%28IT%29)**

###il super repository per recalbox.

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
- Fantastica interfaccia EmulationStation2 basata su Aloshi 
- Versione ottimizzata di FBA con supporto per 4 giocatori 
- Puoi usare RPi GPIOs come controller

## Progetti
**recalboxOS** è il porgetto principale, aggrega i 3 sotto-progetti che compongono il sistema :

- **recalbox-buildroot** : 
https://github.com/digitalLumberjack/recalbox-buildroot (branch recalbox)  
Il progetto recalbox-buildroot è il sistema di buildroot. 
Crea l'intero sistema operativo Linux OS che lancia e supporta la recalbox. Puoi compilare questo progetto, poi copiare i file creati in una SD card formattata e lanciare il ssitema su un raspberryPi.
Attenzione! C'è un modo migliore per fare tutto cio, esso è chiamato recalbox-rescue.

- **recalbox-rescue** : 
https://github.com/digitalLumberjack/recalbox-rescue (branch recalbox)  
Basato sul fantastico NOOBS del team tpi, la recalbox rescue ti permette di installare retroboxOS in modo semplice e veloce permettendoti di avere una partizione di ripristino sulla tua carta SD. E' un altro OS molto leggero che scarica retroboxOS, formatta la tua carta SD e installa il ssitema al tuo posto.
Automaticamente controlla se una nuova versione è presente via internet prima di intallarla sulla tua carta SD.

- **recalbox-emulationstation** : 
https://github.com/digitalLumberjack/recalbox-emulationstation/tree/recalbox-buildroot  
Basato sulla fantastica emulationstation 2 Aloshi, l'interfaccia grafica è stata leggermente adattata per avere una musica di sottofondo (.ogg), selezione multilingua, supporto per aggiornamenti e configurazione dei controlle via interfaccia visuale.

