# dotfiles

## Description
Installing these packages allows you to levereage tmux and vim benefits such as being able to detach tmux windows to continue work on other screens or log out of cloud machines without stopping running processes.

## Instructions

1. Run `./dotfiles/bin/bootstrap.sh`
2. Answer `y` for all options if Ubuntu
    - For Mac OSX: Answer `y` for all options EXCEPT `YouCompleteMe`
3. Enter github username and email (for the repositories you will be using on this machine) when prompted
4. After installation, change terminal font to any font containing the word "powerline"

## Vocabulary
**bind-key**: Key(s) you prepend keyboard shortcuts with

TIP: You can map your `CAPS LOCK` key to your `CTRL` key on your keyboard if you don't use your caps lock key a lot

## For this tmux configuration
**bind-key** = `CTRL + a`

NOTE: The default bind-key is usually `CTRL + b` in most tmux configurations, but I found `CTRL + a` to be easier because I mapped my `CAPS LOCK` key to my `CTRL` key

## Common commands outside TMUX session
| Shortcut | Action |
|--|--|
|`tmux ls`| List all already running tmux sessions |
|`tmux attach-session -t <id>`| Attach to a specific tmux session from the tmux ls list |
|`tmux`| Start a new tmux session |

## Common commands within TMUX session (check `.tmux.conf` for more)
| Shortcut | Action |
|--|--|
|`CTRL + c`| Opens New tmux window|
|`CTRL + d`| Close current tmux pane or window |
|`SHIFT + left-arrow`| Switch to the previous tmux window |
|`SHIFT + right-arrow`| Switch to the next tmux window |
|`bind-key + w`| Opens list of all your created windows|
|`bind-key + v`| Opens a new vertical tmux pane |
|`bind-key + s`| Opens a new horizontal tmux pane |
|`bind-key + V`| Evens out tmux panes widths vertically |
|`bind-key + S`| Evens out tmux panes heights horizontally |
|`bind-key + d`| Detach from your tmux session (does not stop running proccesses in any tmux panes or windows) |
