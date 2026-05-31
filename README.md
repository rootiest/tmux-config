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

## Installation

1. Install [Tmux](https://github.com/tmux/tmux)

2. Backup your current Tmux configuration (if you have one)

   ```bash
   mv ~/.config/tmux ~/.config/tmux.bak
   mv ~/.tmux.conf ~/.tmux.conf.bak
   ```

3. Clone the repository

   ```bash
   git clone https://git.rootiest.dev/rootiest/tmux-config.git ~/.config/tmux
   ```

4. **Enjoy!** 🎉

## Features

- Smart key bindings
- Leader key and modal mode
- Session mux/management/resurrection
- Advanced tab management
- Splits and panes integrate seamlessly with NeoVim
- Seamless integration with fish shell
- Catppuccin theme by default
- Integrates cleanly with other Rootiest projects

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

- [wezterm](https://github.com/wez/wezterm)
- [resurrect.wezterm](https://github.com/MLFlexer/resurrect.wezterm)
- [smart-splits.nvim](https://github.com/mrjones2014/smart-splits.nvim)
- [wezterm-bar](https://github.com/nekowinston/wezterm-bar)
