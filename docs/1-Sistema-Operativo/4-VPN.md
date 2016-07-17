# VPN Juniper en Ubuntu 16.04 64bits

1. Descargar [jre-8u73-linux-i586.tar.gz](http://www.oracle.com/technetwork/java/javase/downloads/jre8-downloads-2133155.html) de la página de oracle y descomprimir en /usr/java32
2. Descomprimir 

> cd /usr/java32
>
> tar –xvf jre-8u73-linux-i586.tar.gz

3. Actualizar el enlace de "alternatives"

> sudo update-alternatives –install /usr/bin/java java /usr/java32/jre1.8.0_73/bin/java 1099

4. Instalar las librerias de 32 bits
> sudo add-apt-repository ppa:maarten-fonville/ppa
> 
> sudo echo "deb http://cz.archive.ubuntu.com/ubuntu trusty main " >> /etc/apt/sources.list
> 
> sudo dpkg --add-architecture i386
> 
> sudo apt-get update
> 
> sudo apt-get install libstdc++6:i386 lib32z1 lib32ncurses5 lib32bz2-1.0 libxext6:i386 libxrender1:i386 libxtst6:i386 libxi6:i386
> 

5. Instalar el plugin icedtea para firefox
> sudo apt-get install icedtea-8-plugin

