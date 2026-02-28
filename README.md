# fzfm
A simple fzf file manager for Linux

![screenshot](https://github.com/archusXIV/fzfm/blob/main/screenshots/fzfm_v0.1.9.png)

FZFM uses a configuration file (~/.config/fzfm/fzfmrc) where customization can be done:
- colors
- default programs
- files extensions definition
- mpv options (if MEDIA_PLAYER=mpv)

## Dependencies
- bat: for files preview
- chafa: for images preview
- fzf (of course)
- stat: for file permission display
- tree: for directories preview

## Installation
```bash
git clone https://github.com/archusXIV/fzfm.git
cd fzfm
mkdir -p ~/.config/fzfm/
cp -r .config/fzfm/ ~/.config/fzfm/
```

## Keyboard shortcuts

| Motions | Description |
| :--------- | :---------- |
| `f12` | edit your config |
| `ctrl-a` | select all |
| `ctrl-d` | delete selected file(s) |
| `ctrl-e` | edit selected file |
| `ctrl-f` | up to first line |
| `ctrl-h` | go back $HOME |
| `ctrl-l` | down to the last line |
| `ctrl-p` | paste previously copied file(s) |
| `ctrl-r` | rename selected file |
| `ctrl-t` | create a file or directory |
| `ctrl-x` | cut (move) selected file(s) |
| `ctrl-y` | yank selected file(s) |
| `esc` | exit |

## Dynamic settings
After editing fzfmrc using F12, new settings are applied if correct.

## Credits
Thanks to all the fzf devs and maintainers for their greater work.
