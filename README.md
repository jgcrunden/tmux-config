# Tmux-config

## Bash prompt
Copy and source [git-prompt.sh](https://github.com/git/git/blob/master/contrib/completion/git-prompt.sh)
```bash
source ~/.git-prompt.sh
export PROMPT_COMMAND='PS1_CMD1=$(__git_ps1 " (%s)")'; PS1=$'\[\e[94m\]\W\[\e[93m\]${PS1_CMD1}\[\e[0m\] \[\e[92m\]\u266B\[\e[0m\] '
```
## Tmuxinator
Install [Tmuxinator](https://github.com/tmuxinator/tmuxinator)
Set editor in `~/.bashrc`
```bash
export EDITOR=nvim
```
Move session.yml to following location: `~/.config/tmuxinator/session.yml`
Start a new tmux session with:
```bash
tmuxinator n session <name_of_session>
```
