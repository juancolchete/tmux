# Tmux
Main repo goal, arrive most productive setup using TMUX on linux

## Configure it global
```
sudo touch /etc/tmux.conf
```
```
sudo vim /etc/tmux.conf
```
## add tmux as default terminal
Edit bashrc
```
vim ~/.bashrc
```
Add this line to the end
```
[[ $TERM != "screen" ]] && exec tmux
```

## add alias
```
alias tmux="TERM=screen-256color-bce tmux"
```
