# Ajustes

## Gnome Classic
http://www.debugpoint.com/2016/04/install-classic-gnome-flashback-in-ubuntu-16-04-replacing-unity/

> sudo apt-get update
> 
> sudo apt-get install gnome-session-flashback

## Ventanas con botones a la derecha
> gsettings set org.gnome.desktop.wm.preferences button-layout ':minimize,maximize,close'


## Prompt git

1. cd ~
2. wget https://raw.githubusercontent.com/git/git/master/contrib/completion/git-completion.bash
3. mv git-completion.bash .git-completion.bash
4. Añadir estas lineas a ~/.bashrc 
> source ~/.git-prompt.sh
> 
> PS1="\[\033[38;5;2m\]\u@\h:\[$(tput sgr0)\]\[\033[38;5;11m\]\w\\$\[$(tput sgr0)\]\[\033[38;5;15m\] \[$(tput sgr0)\]\[$(tput bold)\]\[\033[38;5;5m\]$(__git_ps1 "(%s)")\[$(tput sgr0)\] "
