# ayu bat

Handcrafted implementation of the [ayu] [^1] theme for the [bat] [^2] cli tool.

**[ayu]** is a bright color theme and comes in three versions — _dark_,
_mirage_, and _light_ — for all-day comfortable work.

## Configuration

Copy these theme files to the configuration directory for bat. 

```bash
mkdir -p "$(bat --config-dir)/themes"
cd "$(bat --config-dir)/themes"

# Download a theme in '.tmTheme' format, for example:
git clone https://github.com/freddiehaddad/ayu-bat .

# Update the binary cache
bat cache --build

# Confirm theme is present
bat --list-themes

# Use the theme by setting an environment variable
export BAT_THEME="ayu-dark"

# Or directly with the --theme command line argument
bat --theme ayu-mirage
```

> **NOTE** If any of these instructions fail, refer to the official bat
configuration steps in the [documentation].


## License

`ayu` `bat` theme is made available under the terms of the [MIT] license.

[ayu]: https://ayutheme.com/
[bat]: https://github.com/sharkdp/bat
[documentation]: https://github.com/sharkdp/bat?tab=readme-ov-file#customization
[MIT]: LICENSE

[^1]: Simple, bright, and elegant theme. For any hour — day, dusk, deep night.
[^2]: A cat(1) clone with syntax highlighting and Git integration.
