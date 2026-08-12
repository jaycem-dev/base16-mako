# Base16 Niri

This is meant to be used with [tinted-theming](https://github.com/tinted-theming/home).

## Usage

Include theme on your mako config `~/.config/mako/config`

```
include=~/.config/mako/colors
```

Apply with [Tinty](https://github.com/tinted-theming/tinty) `~/.config/tinted-theming/tinty/config.toml`

```toml
[[items]]
name = "tinted-mako"
path = "https://github.com/jaycem-dev/base16-mako"
themes-dir = "themes"
supported-systems = ["base16"]
hook = "cp -f %f ~/.config/mako/colors; makoctl reload"
```
