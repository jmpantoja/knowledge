# Netbeans

## Descargar e instalar
De momento, la última versión de netbeans, no tiene soporte para PHP7, asi que vamos a usar una [nightly](http://bits.netbeans.org/download/trunk/nightly/latest/)

## Plugins

1. Soporte para markdown
http://plugins.netbeans.org/plugin/50964/markdown-support

2. php-cs-fixer
http://plugins.netbeans.org/plugin/49042/php-cs-fixer

## PSR Formatting
https://maniaplanet.github.io/netbeans-psr/

Despues de eso, hay que ir a 
Tools > Options > Formatting > Blank lines
y asignar el valor 1 a After Class, para que todo valide en PSR-2

## Templates

1. Definir user en Tools/Templates/Settings

> user=Jose Manuel Pantoja <jmpantoja@gmail.com>

2. Añadir cabecera a las templates PHP File, PHP Class, PHP Interface, PHP Trait 

> /*
>  * This file is part of the ${project.displayName} project.
> *
>  * (c) ${user}
>  *
>  * For the full copyright and license information, please view the LICENSE
>  * file that was distributed with this source code.
>  */
