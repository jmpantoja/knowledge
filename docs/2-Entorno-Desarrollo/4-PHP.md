# PHP

Aunque la MV tiene todo el software necesario para el entorno de desarrollo, vamos a instalar un par de cosas en el anfitrión para que el trabajo sea mas comodo.

## Composer

1. Con los paquetes que hemos instalado antes, deberia bastar, pero los necesarios para este punto son:

> sudo apt-get install -y php7.0-cli php7.0-xml php7.0-mbstring

2. Instalamos composer

> cd /tmp
>
> php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"
> 
> php -r "if (hash_file('SHA384', 'composer-setup.php') === 'e115a8dc7871f15d853148a7fbac7da27d6c0030b848d9b3dc09e2a0388afed865e6a3d6b3c0fad45c48e2b5fc1196ae') { echo 'Installer verified'; } else { echo 'Installer corrupt'; unlink('composer-setup.php'); } echo PHP_EOL;"
> 
> sudo php composer-setup.php --install-dir=/usr/bin --filename=composer
> 
> php -r "unlink('composer-setup.php');"
