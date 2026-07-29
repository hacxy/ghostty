# Ghostty Configuration

A clean and modern configuration for [Ghostty](https://ghostty.org), the GPU-accelerated terminal emulator.

## Features

### Typography

- **Font**: JetBrainsMono Nerd Font (18px)
- **Font thickening**: Disabled for crisp rendering

### Window & Appearance

- **Padding**: 5px horizontal and vertical
- **Background opacity**: 90% with 64px blur
- **Window state**: Never saved (fresh start each time)
- **Title bar**: macOS tabs style
- **Decoration**: Auto (system default)

### Cursor & Mouse

- **Cursor style**: Block (non-blinking)
- **Mouse**: Auto-hide while typing

### macOS Optimizations

- **Option key**: Functions as Alt key
- **Title bar style**: Tabs

### Theme

- **Color scheme**: Atom One Dark

### Keybindings

- **Ctrl+`**: Maps to Ctrl+_ (for Vim/Neovim compatibility)

## Installation

### Prerequisites

1. Install Ghostty from [ghostty.org](https://ghostty.org)
2. Install the JetBrainsMono Nerd Font from [Nerd Fonts](https://www.nerdfonts.com/)

### Setup

1. Clone this repository:

   ```bash
   git clone https://github.com/yourusername/ghostty-config.git
   ```

2. Copy the configuration file to your Ghostty config directory:

   ```bash
   mkdir -p ~/.config/ghostty
   cp ghostty-config/config ~/.config/ghostty/config
   ```

3. Restart Ghostty to apply the configuration.

## Customization

### Changing the Font

Edit the `font-family` and `font-size` lines in the config file:

```bash
font-family = YourPreferredFont
font-size = 16.0
```

### Adjusting Transparency

Modify the opacity and blur values:

```bash
background-opacity = 0.85  # Lower = more transparent
background-blur = 32       # Higher = more blur
```

### Changing the Theme

Replace `Atom One Dark` with any Ghostty-supported theme:

```bash
theme = YourPreferredTheme
```

### Adding Custom Keybindings

Add new keybindings following this format:

```bash
keybind = ctrl+shift+a=your_action
```

## File Structure

```
~/.config/ghostty/
└── config          # Main configuration file
```

## Troubleshooting

### Configuration not loading

- Ensure the config file is in `~/.config/ghostty/config`
- Check file permissions (should be readable)
- Restart Ghostty completely

### Font not rendering

- Verify JetBrainsMono Nerd Font is installed
- Check the exact font name in your system

### Performance issues

- Reduce `background-blur` value
- Increase `background-opacity` (closer to 1.0)

## License

This configuration is provided as-is. Feel free to modify and distribute.

## Contributing

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

---

**Note**: This configuration is optimized for macOS but can be adapted for other platforms by removing macOS-specific settings.
