# Antes de Instalar Ubuntu 16.04

## Configuración Uefi
Entramos en la Bios, con F10, durante el arranque.

* Seguridad / Seguridad del sistema
> Tecnologia de virtualización: Habilitado

* Seguridad / Arranque seguro
> Compatibilidad heradada : Inhabilitado
> 
> Arranque seguro : Inhabilitado
> 
> > Administrador de claves 
> > > Borrar claves: Borrar
> > > Propiedad de las claves: Claves de HP
> 
> Arranque rápido: Habilitado

## Tabla de particiones
Para 1 disco de 1Tb de capacidad

| Partición 	| Tipo 	| Tamaño    	| Montaje    	|
|-----------	|------	|-----------	|------------	|
| /dev/sda1 	| efi  	| 40Mb      	|            	|
| /dev/sda2 	| swap 	| 4.000Mb   	|            	|
| /dev/sda3 	| ext4 	| 10.000Mb  	| /          	|
| /dev/sda4 	| ext4 	| 5.000Mb   	| /tmp       	|
| /dev/sda5 	| ext4 	| 45.000Mb  	| /var       	|
| /dev/sda6 	| ext4 	| 45.000Mb  	| /usr       	|
| /dev/sda7 	| ext4 	| 250.000Mb 	| /home      	|
| /dev/sda8 	| ext4 	| ~         	| /mnt/datos 	|

