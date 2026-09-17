# Catppuccin Mocha for Omarchy

This theme owns its Hyprland blur, window rounding, and Quickshell rounding
through `hyprland.lua` and `shell.toml`.

Omarchy treats a theme directory containing `.git` as an untrusted installed
theme and deliberately excludes `*.lua` files when applying it. Keep this
checkout outside `~/.config/omarchy/themes` and expose it there as a symlink:

```sh
mkdir -p ~/.local/share/omarchy/themes
mv ~/.config/omarchy/themes/catppuccin-mocha ~/.local/share/omarchy/themes/catppuccin-mocha
ln -s ~/.local/share/omarchy/themes/catppuccin-mocha ~/.config/omarchy/themes/catppuccin-mocha
```

The symlink marks the checkout as user-owned, so `omarchy theme set Catppuccin\ Mocha`
stages `hyprland.lua` along with the rest of the theme.
