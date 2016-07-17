# Software

## Repositorios

### Spotify
> sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys BBEBDCB318AD50EC6865090613B00F1FD2C19886
>
> echo deb http://repository.spotify.com stable non-free | sudo tee /etc/apt/sources.list.d/spotify.list
 
### Skype
> sudo dpkg --add-architecture i386
> sudo add-apt-repository "deb http://archive.canonical.com/ $(lsb_release -sc) partner"
 

### Paquetes
> sudo apt-get update
>
> sudo apt-get install -y terminator geany vim virtualbox virtualbox-dkms ansible git hexchat hexchat-indicator spotify-client wallch skype deluge vagrant nfs-common nfs-kernel-server mediainfo

