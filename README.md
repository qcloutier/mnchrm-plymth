# mnchrm-plymth

Monochrome 
[Plymouth](https://www.freedesktop.org/wiki/Software/Plymouth/) 
theme that displays white icons on a black background.

![screenshot](screenshot.png?raw=true)

Features logos for several popular distros, including:

- Arch Linux
- CentOS
- Debian
- elementaryOS
- Fedora
- Gentoo Linux
- Linux Mint
- openSUSE
- Solus
- Ubuntu
- Void Linux

... as well as a generic Tux icon.

Also supports password entry for unlocking encrypted drives.

## Installation

Copy the `mnchrm` folder to the Plymouth theme directory.
For example, on Arch Linux:

    # cp -r mnchrm /usr/share/plymouth/themes/

Then set it as the default theme and rebuild the kernel image.
Again, on Arch Linux:

    # plymouth-set-default-theme -R mnchrm

Consult your distribution's documentation for more details.

## Changing the Distribution Logo

Open `mnchrm/mnchrm.script` in your favourite text editor and find this line:

```
logo.image = Image("icons//tux.png");
```

Change `icons//tux.png` to the name of the desired logo.

Themed logos are provided in the `mnchrm/logos` directory.

