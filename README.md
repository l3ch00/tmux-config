# Tmux Configuration

Personal tmux configuration with custom keybindings, theme, and plugins.

## Features

- **Custom prefix**: `Ctrl+a` (instead of default `Ctrl+b`)
- **Vim-style navigation**: Use `h/j/k/l` for pane movement
- **Mouse support**: Enabled for scrolling and selecting
- **Catppuccin theme**: Mocha flavor with rounded window style
- **Enhanced status bar**: Shows session, git branch, hostname, date/time, CPU, and uptime
- **Popup shortcuts**: Quick access to lazygit and scratch sessions
- **System clipboard integration**: Copy with `y`, paste with system clipboard
- **Auto-renumbering**: Windows automatically renumber when closed

## Key Bindings

### Prefix
- `Ctrl+a` - Prefix key

### Navigation
- `h/j/k/l` - Move between panes
- `Arrow keys` - Resize panes by 5 cells

### Popups
- `Ctrl+a` + `Ctrl+y` - Open lazygit popup
- `Ctrl+a` + `Ctrl+t` - Open terminal popup
- `Ctrl+a` + `Alt+s` - Open/attach to scratch session

### Copy Mode
- `v` - Start selection
- `y` - Copy to clipboard
- `Enter` - Copy and cancel

## Plugins

- [tpm](https://github.com/tmux-plugins/tpm) - Tmux Plugin Manager
- [catppuccin/tmux](https://github.com/catppuccin/tmux) - Catppuccin theme
- [tmux-resurrect](https://github.com/tmux-plugins/tmux-resurrect) - Save/restore sessions
- [tmux-continuum](https://github.com/tmux-plugins/tmux-continuum) - Automatic saving
- [tmux-sensible](https://github.com/tmux-plugins/tmux-sensible) - Sensible defaults
- [vim-tmux-navigator](https://github.com/christoomey/vim-tmux-navigator) - Vim integration
- [tmux-cpu](https://github.com/tmux-plugins/tmux-cpu) - CPU monitoring

## Dependencies

- [gitmux](https://github.com/arl/gitmux) - Git status in status bar
- [lazygit](https://github.com/jesseduffield/lazygit) - Terminal UI for git
- [wl-copy](https://github.com/bugaevc/wl-clipboard) - Wayland clipboard (Linux)

## Installation

1. Clone this repository:
   ```bash
   git clone <repo-url> ~/.config/tmux
   ```

2. Install TPM (Tmux Plugin Manager):
   ```bash
   git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
   ```

3. Install plugins in tmux:
   ```bash
   # Press prefix + I (capital i) inside tmux
   ```

## Requirements

- tmux 3.0+
- gitmux (for git status)
- lazygit (optional, for git popup)
- wl-clipboard (for Wayland copy/paste)

## License

MIT
