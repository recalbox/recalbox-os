[![English](http://upload.wikimedia.org/wikipedia/commons/e/e1/Union_Jack_22x16.png "English")](README.md)
[![Italiano](http://upload.wikimedia.org/wikipedia/commons/7/70/Flag_of_italy.png "Italiano")](README-IT.md)
[![Français](http://upload.wikimedia.org/wikipedia/commons/1/14/Flag_of_france.png "Française")](README-FR.md)
[![Portugues](http://www.flagsoftheworld.eu/images/2/flag-of-portugal.png "Portugues")](README-PT.md)
[![Espagnol](http://upload.wikimedia.org/wikipedia/commons/3/30/Flag_of_spain.png "Espagnol")](README-ES.md)
****
# recalbox-os

Novidade : v3.2.11 Correção no bug dos controles com mesmo nome, tema zoid adicionado.

Novidade : v3.2.4 Novo arquivo de configuração recalbox.conf, novo sistema de boot.

Novidade : v3.2.3 Correções de bugs, mapeamento dos analógicose L2/R2 adicionadas nas configurações dos controles.

Novidade : recalboxOS agora é compatível com RPi2 !

Novidade : Busque todas as informações em recalbox-os através do WIKI

O super repositório para recalbox.

O objetivo desse repositório é agrupar os diferentes projetos do recalbox num único como forma de simplificar e facilitar a compilação do sistema.

Apresentação

recalboxOS é um sistema leve criado para rodar no Raspberry Pi e Raspberry Pi 2.

Voce pode transformar seu RPi numa plataforma de emulação, com suporta para 16 sistemas!

Características

Suporte à Atari 2600, NES, Game Boy, Game Boy color, Game Boy Advance, Super Nintendo, Master System, Megadrive (Genesis), FBA, iMame4all, PCEngine, MSX1/2, PSX, SegaCD, Sega 32x, Sega SG1000, Famicom Disk System.
Desenvolvido com buildroot, dessa forma o sistema de arquivos root possui apenas 100MB.
Sistema de recuperação baseado no NOOBS : reinstale diretamente de um cartão SD ou baixe a última versão pela internet
Atualização online
Acesso em rede para a pasta de roms, screenshots e savestates.
Partição rom em fat32 : Compatível com todos os sistemas
Configuração de controles no EmulationStation : Umav vez configurado, todos os emuladores serão configurados.
Trilhas sonoras no EmulationStation
Suporte à controles de PS3 e Shanwan Bluetooth (conecte o controle, desconecte e jogue)
Sistema traduzido para Francês, Inglês, Português (agradeço ao mgoulart), Espanhol, Alemão e talvez em outros idiomas case queira participar.
Interface baseado no EmulationStation2, desenvolvido pelo Aloshi.
FBA otimizado com suporte à quatro jogadores (Dungeons and Dragons!!!)
Suporte à controles GPIO

Projetos

recalboxOS é o projeto principal, que agrega três subprojetos que compõe o sistema:

recalbox-buildroot : https://github.com/digitalLumberjack/recalbox-buildroot (branch recalbox)
O projeto recalbox-buildroot é o sistema buildroot. Ele cria todo o sistema operacional linux que rodará no recalbox. Voce pode compilar esse projeto, e então copiar os arquivos de saída para um cartão SD formatado para rodar num RPi. Porém existe um caminho mais fácil chamado recalbox-rescue.

recalbox-rescue : https://github.com/digitalLumberjack/recalbox-rescue (branch recalbox)
Baseado no incrível sistema NOOBS do time de desenvolvedores do rpi, o recalbox rescue permite que voce instale facilmente o recalboxOS e tenha uma partição de recuperação no seu cartão SD. Ele é um outro mini sistema operacional, que baixará o recalboxOS, formatar seu cartão SD, e instalar o sistema para voce.
Ele checará se uma nova versão está disponível na internet, antes de instalar o sistema no cartão SD.

recalbox-emulationstation : https://github.com/digitalLumberjack/recalbox-emulationstation/tree/recalbox-buildroot
Baseado no incrível EmulationStation 2 (desenvolvide pelo Aloshi), a interface foi modificada para ter suporte a trilhas sonoras, seleção de idiomas, suporte a atualização e configuração de controles.
