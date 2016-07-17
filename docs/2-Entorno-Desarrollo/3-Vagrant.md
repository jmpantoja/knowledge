# Virtual Box + Vagrant + Ansible

1. Con los paquetes que hemos instalado antes, deberia bastar, pero los necesarios para este punto son:

> sudo apt-get install -y virtualbox virtualbox-dkms ansible git vagrant nfs-common nfs-kernel-server

2. Creamos los directorios para el entorno

> mkdir -p /mnt/datos/deploy/vagrant
>
> mkdir -p /mnt/datos/deploy/projects
> 
> mkdir -p /mnt/datos/deploy/tmp

3. Clonamos el repositorio con el proyecto de ansible

> cd /mnt/datos/deploy/vagrant
>
> git clone git@github.com:jmpantoja/ansible-deploy.git .
>

Para levantar la máquina con php7
> vagrant up website

