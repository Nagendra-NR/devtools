# Tmux and WezTerm Setup Guide

## Installation

Download and install or:
```
brew install --cask wezterm
```

Install tmux 
```
brew install tmux
```
Configuration file :
```
~/.tmux.conf
```
## Creating and Managing Tmux Sessions
Create a new tmux session:
```
tmux new -s Session
```
Detach from the current session:
```
tmux detach
```
List all tmux sessions:
```
tmux ls
```
Attach to an existing session:
```
tmux attach -t Session
```
Create another new session:
```
tmux new -s Session2
```
## Basic Tmux Commands
Create a new tmux window:
```
Ctrl+a t
```
we can see the windows at the bottom.

For switching to any window
```
Ctrl+a 1,2,3
```
or 
```
Ctrl+a n # Next Window
```
View all windows:
```
Ctrl+a w
```
Move between panes:
```
Ctrl + L,H,J,K
```
## Copy Mode
Enter copy mode:
```
Ctrl + [
```
Move up and down:
```
# Use j,k or arrow keys
```
Move up or down  half a page 
```
Ctrl + u   or  Ctrl + d
``` 

Move up or down a full page
```
Ctrl + b   or Ctrl + f
```

copy test
```
y
```
Exit from copy mode 
```
Ctrl + c
```

