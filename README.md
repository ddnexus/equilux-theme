# Equilux Theme

![Screenshot](screenshot.png)

The Equilux Theme provides a couple of full-dark, neutral-gray themes (for GTK2, GTK3, Shell, and GDM) using the Equilux palette.

It is based on the [Materia Theme](https://github.com/nana-4/materia-theme). For detailed features and documentation, please, check upstream.
                                                                                                                            app
### Motivation

The Equilux themes provide a neutral dark-balanced color-scheme not designed to be __fancy__, but to be __useful__ for a few specific goals.

1. __Minimize eye strain__: when you pass many hours in front of the screen or you are hyper-sensitive to light, saturation and contrast, your eyes will benefit from a dull UI

2. __Avoid disrupting your circadian rhythms__: a neutral color-cast-free UI helps your body to produce enough melatonin at night time and sleep better, working nicely with software like `f.lux`, `redshift`, `NightLight`, ...

3. __Professional use in image editing, graphic design, 3D rendering__: in that fields any color cast or excessive contrast, brightness or darkness introduced by the UI would affect the overall perception of the color and balance of the images

4. __You may find it stylish__: even if the style is not the main goal, many people find that its very clean and minimalistic UI looks cool and professional


### Technical Focus

The Equilux Theme sticks to the upstream theme as much as possible, and is exclusively focused on the following points:

- Total removal of any color cast from the background elements (neutral base)
- Use of a neutral base for all the UI elements, with exception of a few button/boxes
- Maximum reduction of contrast/saturation
- Medium overall brightness/darkness of the UI

### Changes from the Upstream Theme

- The installer script installs only the Equilux variants
- The Chrome extension is not supported (you may try Vivaldi and change its colors in the settings)
- Addition of Ubuntu font family and removal of the "M+ c1" font.
- Addition of a few utility scripts handy to use in development/hacking
- A few minor cosmetic fixes
- Minimal changes in the color assignations in order to make the Equilux palette work OK with the theme.

## Theme Installation/Uninstallation

**Installation**: Download the latest `equilux-theme-*.tar.xz` version listed in the __Files__ tab [here](https://www.opendesktop.org/p/1182169/), unzip it and move the Equilux* dirs to `/usr/share/themes`. As an alternative you can download the source of the latest release [here](https://github.com/ddnexus/equilux-theme/releases) and run the `install.sh` script as privileged user.

**Uninstallation**: Delete the installed directories: `sudo rm -rf /usr/share/themes/Equilux{,-compact}`

## Font Customization

After you install the themes, you may want to customize the fonts by replacing their names inside the installed CSS file. Here is the command to run (courtesy of nana-4). Just remember to edit the "your-preferred-font" string :).

```
    sudo sed -i 's/Ubuntu, Roboto/your-preferred-font/g' /usr/share/themes/Equilux{,-compact}/gnome-shell/gnome-shell.css
```

## GDM Theme Installation/Uninstallation

See the the upstream instruction [here](https://github.com/nana-4/materia-theme/wiki/GDM-Theme).

## Related Items

A quick list of items that - for different reasaons - fit well with the Equilux style and concept. Please, submit your suggestions as a new Issue, so I will add a note in this section.

### Wallpapers

Seamless textures from various sources and authors, converted to low contrast/brightness grayscale available in the __Files__ tab [here](https://www.opendesktop.org/p/1182169/)

### Icons

- [Circle Numix Icons](https://github.com/numixproject/numix-icon-theme-circle): a circle themed icon set well maintained and not too bright (if you use Numix Folders below to tame the folder colors)

- [Numix Folders](https://github.com/numixproject/numix-folders): Customization script to change the colors and style of the numix folder (otherwise too bright and saturated). Recommended settings: Style: 6, Primary color: #9c9c9c, Secondary color; #9c9c9c, Symbol: #656565

### GNOME Extensions

- [Darker Overview](https://extensions.gnome.org/extension/1177/darker-overview/): Customize the darkness of the background in the Overview. It can also remove the ugly vignette effect

- [Desaturate All](https://extensions.gnome.org/extension/1102/desaturate-all/): Desature the entire gnome workspace (I hacked a copy to have 4 deaturation levels instead of all-or-none: ask if interested)

- [AppMenu Regular Icons](https://extensions.gnome.org/extension/970/appmenu-regular-icons/): Disables Symbolic Icons in the app menu. In the mostly grayscale UI, a small colored icon is useful to quickly identify the app you are in. Besides it normalizes the icons that otherwise would be grey or colored with no particular consistence.

- [Background Logo](https://extensions.gnome.org/extension/889/background-logo/): Overlay an icon/pict in the bottom right corner. A bit buggy and useless :) but a nice touch.

### App Themes and Settings

- [Equilux-Telegram](https://github.com/aquatix/Equilux-Telegram-Theme)

- [Equilux-Flubox](https://www.opendesktop.org/p/1193958/) 

- TBD: add the style settings consistent with the Equilux Palette for apps like Vivaldi, Tilix, RubyMine, SmartGit, DeepGit, ... 


## Branches

Master is always the upstream master: no changes from the base theme there.
The `equilux-*` branch(es) are the branches with the changes from the upstream master.
Please, notice that the `*-dev` branches may get rebased on top of master. The old versions will be tagged and will not be removed/rebased.

## License

The Equilux Theme is distributed under the terms of the GNU General Public License, version 2 or later. See the [`COPYING`](COPYING) file for details.

## Credits

- All credits go to the [Materia Theme](https://github.com/nana-4/materia-theme), its author and contributors.
