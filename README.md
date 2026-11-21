# Rootiest Tmux Configuration

```none
 ██▀███   ▒█████   ▒█████  ▄▄▄█████▓ ██▓▓█████   ██████ ▄▄▄█████▓
▓██ ▒ ██▒▒██▒  ██▒▒██▒  ██▒▓  ██▒ ▓▒▓██▒▓█   ▀ ▒██    ▒ ▓  ██▒ ▓▒
▓██ ░▄█ ▒▒██░  ██▒▒██░  ██▒▒ ▓██░ ▒░▒██▒▒███   ░ ▓██▄   ▒ ▓██░ ▒░
▒██▀▀█▄  ▒██   ██░▒██   ██░░ ▓██▓ ░ ░██░▒▓█  ▄   ▒   ██▒░ ▓██▓ ░
░██▓ ▒██▒░ ████▓▒░░ ████▓▒░  ▒██▒ ░ ░██░░▒████▒▒██████▒▒  ▒██▒ ░
░ ▒▓ ░▒▓░░ ▒░▒░▒░ ░ ▒░▒░▒░   ▒ ░░   ░▓  ░░ ▒░ ░▒ ▒▓▒ ▒ ░  ▒ ░░
  ░▒ ░ ▒░  ░ ▒ ▒░   ░ ▒ ▒░     ░     ▒ ░ ░ ░  ░░ ░▒  ░ ░    ░
  ░░   ░ ░ ░ ░ ▒  ░ ░ ░ ▒    ░       ▒ ░   ░   ░  ░  ░    ░
   ░         ░ ░      ░ ░            ░     ░  ░      ░

░▒▓████████▓▒░▒▓██████████████▓▒░░▒▓█▓▒░░▒▓█▓▒░▒▓█▓▒░░▒▓█▓▒░
   ░▒▓█▓▒░   ░▒▓█▓▒░░▒▓█▓▒░░▒▓█▓▒░▒▓█▓▒░░▒▓█▓▒░▒▓█▓▒░░▒▓█▓▒░
   ░▒▓█▓▒░   ░▒▓█▓▒░░▒▓█▓▒░░▒▓█▓▒░▒▓█▓▒░░▒▓█▓▒░▒▓█▓▒░░▒▓█▓▒░
   ░▒▓█▓▒░   ░▒▓█▓▒░░▒▓█▓▒░░▒▓█▓▒░▒▓█▓▒░░▒▓█▓▒░░▒▓██████▓▒░
   ░▒▓█▓▒░   ░▒▓█▓▒░░▒▓█▓▒░░▒▓█▓▒░▒▓█▓▒░░▒▓█▓▒░▒▓█▓▒░░▒▓█▓▒░
   ░▒▓█▓▒░   ░▒▓█▓▒░░▒▓█▓▒░░▒▓█▓▒░▒▓█▓▒░░▒▓█▓▒░▒▓█▓▒░░▒▓█▓▒░
   ░▒▓█▓▒░   ░▒▓█▓▒░░▒▓█▓▒░░▒▓█▓▒░░▒▓██████▓▒░░▒▓█▓▒░░▒▓█▓▒░

             ▄████▄   ▒█████   ███▄    █   █████▒
             ▒██▀ ▀█  ▒██▒  ██▒ ██ ▀█   █ ▓██   ▒
             ▒▓█    ▄ ▒██░  ██▒▓██  ▀█ ██▒▒████ ░
             ▒▓▓▄ ▄██▒▒██   ██░▓██▒  ▐▌██▒░▓█▒  ░
             ▒ ▓███▀ ░░ ████▓▒░▒██░   ▓██░░▒█░
             ░ ░▒ ▒  ░░ ▒░▒░▒░ ░ ▒░   ▒ ▒  ▒ ░
             ░  ▒     ░ ▒ ▒░ ░ ░░   ░ ▒░ ░
             ░        ░ ░ ░ ▒     ░   ░ ░  ░ ░
             ░ ░          ░ ░           ░
             ░
                      ╭─────────────╮
                      ╭─────────────╮
                      │ $W          │
                      │             │
                      │             │
                      ╰─────────────╯
```

The rootiest Tmux configuration you will ever see!

## Requirements

- [tmux](https://github.com/tmux/tmux) 3.5 or newer
- `git` (to install the plugins)
- [fish](https://fishshell.com/) (the default shell for new panes)
- `wl-copy` from [wl-clipboard](https://github.com/bugaevc/wl-clipboard) for the primary selection
- A Nerd Font for the status line glyphs

## Installation

1. Install [tmux](https://github.com/tmux/tmux)

2. Back up your current tmux configuration (if you have one)

   ```bash
   mv ~/.config/tmux ~/.config/tmux.bak
   mv ~/.tmux.conf ~/.tmux.conf.bak
   ```

3. Clone the repository

   ```bash
   git clone https://git.rootiest.dev/rootiest/tmux-config.git ~/.config/tmux
   ```

4. Start tmux. The first start clones [tpm](https://github.com/tmux-plugins/tpm)
   and installs the plugins; restart tmux once it finishes to load the theme.

## Features

- **Sessions that survive reboots:** tmux-resurrect saves every session, window,
  pane, working directory and visible pane contents; tmux-continuum saves every
  5 minutes and restores the last save when the server starts. nvim, ssh, btop,
  htop, yazi and lazygit are started again in their panes.
- **Tuned for kitty:** truecolor, undercurl, hyperlinks, synchronized output,
  extended keys (CSI u) and focus events are enabled for `xterm-kitty`, and the
  kitty tab title follows the session and window (`session: window`).
- **Passthrough:** kitty graphics in unicode placeholder mode (yazi, image.nvim),
  desktop notifications and kitty user variables reach the outer terminal.
- **Clipboard:** copies go to the system clipboard through OSC 52 (also over
  ssh) and to the primary selection through `wl-copy`. Mouse selections copy on
  release; hold <kbd>Shift</kbd> to select with the terminal instead.
- **Catppuccin Mocha** status line at the top, showing the directory and session.

## Key bindings

The prefix is the tmux default, <kbd>Ctrl</kbd>+<kbd>b</kbd>.

| Keys | Action |
|---|---|
| <kbd>prefix</kbd> <kbd>\|</kbd> | Split right |
| <kbd>prefix</kbd> <kbd>\\</kbd> | Split right, full height |
| <kbd>prefix</kbd> <kbd>-</kbd> | Split down |
| <kbd>prefix</kbd> <kbd>_</kbd> | Split down, full width |
| <kbd>prefix</kbd> <kbd>c</kbd> | New window |
| <kbd>prefix</kbd> <kbd>h</kbd> <kbd>j</kbd> <kbd>k</kbd> <kbd>l</kbd> | Move to the pane left, down, up, right |
| <kbd>prefix</kbd> <kbd><</kbd> / <kbd>></kbd> | Move the window left / right (repeatable) |
| <kbd>prefix</kbd> <kbd>r</kbd> | Reload `tmux.conf` |
| <kbd>prefix</kbd> <kbd>Ctrl</kbd>+<kbd>s</kbd> | Save all sessions now (tmux-resurrect) |
| <kbd>prefix</kbd> <kbd>Ctrl</kbd>+<kbd>r</kbd> | Restore the last save (tmux-resurrect) |

Splits and new windows open in the current pane's directory. Copy mode uses vi
keys: <kbd>v</kbd> starts a selection and <kbd>y</kbd> copies it.

## Using it with kitty

The [Rootiest Kitty](https://git.rootiest.dev/rootiest/kitty-config) config opens
tmux sessions as kitty tabs, so plain tabs stay the default and only the tabs
you choose are restorable:

| Keys | Action |
|---|---|
| <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>m</kbd> | New tab with a tmux session named after the current directory |
| <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>i</kbd> | fzf picker: attach, create or kill sessions |
| <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>d</kbd> | Kill the session in the current tab, after confirming |

Closing a tmux tab only detaches it; the session keeps running and can be
picked again. After a reboot the first tmux tab or picker starts the server,
which restores the saved sessions.

Inside tmux, kitty's own scrollback tools (`search_scrollback`,
kitty-scrollback.nvim, jumping between prompts) see only the visible screen; use
copy mode (<kbd>prefix</kbd> <kbd>[</kbd>, or scroll with the mouse wheel) instead.

## Screenshots

![Rootiest Tmux](.screenshots/tmux.png)

## Companion Tools

[Rootiest WezTerm](https://git.rootiest.dev/rootiest/wezterm-config) -
A wezterm configuration that is designed to work with this tmux config.

[Rootiest Kitty](https://git.rootiest.dev/rootiest/kitty-config) -
A kitty configuration that is designed to work with this tmux config.

[Rootiest Fish](https://git.rootiest.dev/rootiest/fish-config) -
Fish shell configuration that pairs well with this Tmux configuration
and the NeoVim configuration.

[Rootiest Neovim](https://git.rootiest.dev/rootiest/neovim-config) -
A NeoVim config built to work alongside this and the fish config.

[Rootiest Iosevka Font](https://git.rootiest.dev/rootiest/rootiest-iosevka) -
A custom Iosevka font that is designed by developers, for developers.

[Nerd Fonts](https://github.com/ryanoasis/nerd-fonts/) -
A collection of fonts that include many icons and glyphs that are used in this configuration.

## Dotfiles

[Rootiest Dotfiles](https://github.com/rootiest/dotfiles)

## Credits

- [tpm](https://github.com/tmux-plugins/tpm)
- [tmux-resurrect](https://github.com/tmux-plugins/tmux-resurrect)
- [tmux-continuum](https://github.com/tmux-plugins/tmux-continuum)
- [catppuccin/tmux](https://github.com/catppuccin/tmux)
