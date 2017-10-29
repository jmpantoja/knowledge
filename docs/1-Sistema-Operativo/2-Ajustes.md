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
4. wget https://raw.githubusercontent.com/git/git/master/contrib/completion/git-prompt.sh
5. mv git-prompt.sh .git-prompt.sh
6. Añadir estas lineas a ~/.bashrc 

> . ~/.git-completion.bash
> 
> . ~/.git-prompt.sh
> 
> export GIT_PS1_SHOWDIRTYSTATE=1
> export PS1='\[\e]0;\u@\h: \w\a\]${debian_chroot:+($debian_chroot)}\[\033[01;32m\]\u@\h\[\033[00m\]:\[\033[01;34m\]\w\[\033[00m\]\[\033[33m\]$(__git_ps1)\[\033[00m\]\$ '


