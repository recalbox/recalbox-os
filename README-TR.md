[![English](http://upload.wikimedia.org/wikipedia/commons/e/e1/Union_Jack_22x16.png "English")](README.md)
[![Italiano](http://upload.wikimedia.org/wikipedia/commons/7/70/Flag_of_italy.png "Italiano")](README-IT.md) 
[![Français](http://upload.wikimedia.org/wikipedia/commons/1/14/Flag_of_france.png "Française")](README-FR.md)
[![Deutsch](http://upload.wikimedia.org/wikipedia/commons/4/4b/Flag_of_germany.png "Deutsch")](README-DE.md)
[![Portugues](http://upload.wikimedia.org/wikipedia/commons/a/aa/Flag_of_Portugal_icon.png "Portugues")](README-PT.md)
[![Español](http://upload.wikimedia.org/wikipedia/commons/3/30/Flag_of_spain.png "Español")](README-ES.md)
[![Türkçe](https://upload.wikimedia.org/wikipedia/commons/thumb/b/b4/Flag_of_Turkey.svg/24px-Flag_of_Turkey.svg.png "Türkçe")](README-TR.md)

****
# recalbox-os
**Yeni : v3.2.11 Aynı isimdeki kontroller hatası düzeltildi, zoid teması eklendi**

**Yeni : v3.2.4 Yeni recalbox.conf sistem, yeni boot sistem.**

**Yeni : v3.2.3 Hata düzeltmeleri, Analog joystick ve L2/R2 joystick ayarlarına eklendi**

**Yeni : recalboxOS şimdi RPi2 uyumlu !**

**Yeni : recalbox-os hakkında bütün bilgileri için [WIKI](https://github.com/digitalLumberjack/recalbox-os/wiki)**

Recalbox için süper depo.

Bu deponun amacı değişik recalbox projelerini tek bir çatı altında toplayarak sistemi daha kolay derleme amacı sağlamaktır.

## Sunum
recalboxOS işletim sistemi, raspberryPi ve raspberry Pi2 cihazlar için tasarlanmış hafif bir sistemdir.

Rpi cihazınızı 32 sisteme kadar destekli bir emülasyon platformuna dönüştürebilirsiniz !


## Özellikler 
- Atari 2600, Atari 7800, NES, Game Boy, Game Boy color, Game Boy Advance, Super Nintendo, Famicom Disk System, Master System, Megadrive (Genesis), Gamegear, Game and Watch, Lynx, NeoGeo, NeoGeo Pocket, FBA (subset), iMame4all (subset), PCEngine, Supergrafx, MSX1/2, PSX, Sega Cd, Sega 32X, Sega SG1000, Playstation, ScummVM, Vectrex, VirtualBoy, Wonderswan destekler
- Sistem buildroot ile yapılmıştır, dolayısıyla kök dosya sistemi sıkıştırılmış olarak sadece 100MB dır.
- Kurtarma sistemi NOOBS baz alınarak yapılmıştır : sd kartınızdan tekrar doğrudan kurulum yapın veya netten son versiyonu indirin
- Çevrimiçi güncelleme
- rom klasörüne ağ bağlantısı, ekran görüntüleri, kayıtlar.
- fat32 rom biçimi : tüm sistemlerle uyumludur
- Ön planda konsol kontrolörü ayarlaması : bir kere ayarla, her yerde oyna.
- Arkaplan müzik
- PS3 and Shanwan Bluetooth dahili desteği (tak, çıkar ve çalıştır)
- Fransızca, İngilizce, Portekizce, İspanyolca, Almanca, İtalyanca, Türkçe ve belki katılım sağlanırsa diğer dillerde.
- Önyüz harika EmulationStation2 tabanlo Aloshi
- FBA 4 kullanıcı destekli versiyona optmize edildi (evet Zindanlar ve Ejderhalar)
- RPi GPIO larını kontrolör olarak kullanma

## Projeler
**recalboxOS** ana proje olarak, 3 alt-projeyi sistemi oluşturmak için kapsar :

- **recalbox-buildroot** : 
https://github.com/digitalLumberjack/recalbox-buildroot (branch recalbox)  
recalbox-buildroot projesi buildroot sistemidir. recalbox çalışabilmesi için tüm linux işletim sistemini oluşturur.
Bu projeyi derleyebilirsiniz, daha sonra çıktı dosyalarını manuel olarak formatlanmış SD karta kopyalayarak sistemi raspberryPi de çalıştırabilirsiniz. Fakat bunun daha iyi bir yolu var, nam-ı diğer recalbox-rescue.

- **recalbox-rescue** : 
https://github.com/digitalLumberjack/recalbox-rescue (branch recalbox)  
rpi-takımının muhteşem NOOBS sistemine dayanır, recalbox kurtarma size kolay bir şekilde retroboxOS işletim sistemini kurmanıza olank sağlar ve SD kartınızda bir kurtarma alanı açar. Bu retroboxOS indirmenize olanak sağlayan bir diğer küçük işletim sistemidir, SD kartınızı formatlayın ve sistemi sizin için kursun.  
SD kart versiyonunu kurmadan önce sizin için nette yeni bir versiyon olup olmadığını kontrol eder.. 

- **recalbox-emulationstation** : 
https://github.com/digitalLumberjack/recalbox-emulationstation/tree/recalbox-buildroot  
Aloshi'nin muhteşem emulationstation 2 üzerine inşa edilmiştir, önyüzü ogg müzik desteği için biraz modifiye edildi, dil seçimi, güncelleme desteği ve kontrolör ayarları.
