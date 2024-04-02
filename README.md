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
if command -v tmux &> /dev/null && [ -n "$PS1" ] && [[ ! "$TERM" =~ screen ]] && [[ ! "$TERM" =~ tmux ]] && [ -z "$TMUX" ]; then
  exec tmux
fi
```

## add alias
```
alias tmux="TERM=screen-256color-bce tmux"
```
