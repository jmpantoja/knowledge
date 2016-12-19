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
> 
> parse_git_branch() {
> 
>      git branch 2> /dev/null | sed -e '/^[^*]/d' -e 's/* \(.*\)/ (\1)/'
> 
> }
> 
> export PS1="\u@\h \[\033[32m\]\w\[\033[33m\]\$(parse_git_branch)\[\033[00m\] $ "
> 


