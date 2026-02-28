# fzfm
A simple fzf file manager for Linux

<table width="100%">
  <tr>
    <th>main</th>
    <th>image preview</th>
  </tr>
  <tr>
    <td width="50%">
      <img src="https://github.com/archusXIV/fzfm/blob/main/screenshots/fzfm_v0.1.9.png" />
    </td>
    <td width="50%">
      <img src="https://github.com/archusXIV/fzfm/blob/main/screenshots/fzfm_image.png" />
    </td>
  </tr>
  <tr>
    <th>media info</th>
    <th>tree</th>
  </tr>
  <tr>
    <td width="50%">
      <img src="https://github.com/archusXIV/fzfm/blob/main/screenshots/fzfm_media.png" />
    </td>
    <td width="50%">
      <img src="https://github.com/archusXIV/fzfm/blob/main/screenshots/fzfm_tree.png" />
    </td>
  </tr>
</table>

FZFM uses a configuration file (~/.config/fzfm/fzfmrc) where customization can be done:
- colors
- default programs
- files extensions definition
- mpv options (if MEDIA_PLAYER=mpv)

When copying/pasting in the same directory, the new one will be named with an underscore
- example: my_file -> myfile_ (same as [ranger](https://ranger.fm/) does)

Some prompts may appear when deleting, creating files

## Dependencies
- bat: for files preview
- chafa: for images preview
- [fzf](https://github.com/junegunn/fzf) (of course)
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
| `ctrl-z` | deselect file(s) |
| `esc` | exit |

## Dynamic settings
After editing [fzfmrc](https://github.com/archusXIV/fzfm/blob/main/.config/fzfm/fzfmrc) using F12, new settings are applied if correct.

## Credits
Thanks to all the fzf devs and maintainers for their greater work.
