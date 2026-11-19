# Sweet Folders
Folder icons from the [Sweet GTK Theme](https://www.opendesktop.org/s/Gnome/p/1253385/) for Linux desktop environments.

![Sweet Folder Icons](img/sweet-folder-icons.png)

![Screenshot](img/screenshot.png)

## Important
This repo only contains the folder icons, to complement an existing icon theme: every other icon comes from the themes listed in `Inherits`.

Each variant is its own theme: `Sweet-Blue`, `Sweet-Mars`, `Sweet-Purple`, `Sweet-Rainbow`, `Sweet-Red`, `Sweet-Teal` and `Sweet-Yellow`, and the `-Filled` versions of all but Mars and Rainbow.

## Install

On Arch Linux, the AUR package `sweet-folders-git` installs every variant to `/usr/share/icons`.

Otherwise:

1. Download the folder theme of your choice, from this GitHub repo or [Open Desktop](https://www.opendesktop.org/p/1284047#files-panel)

2. Copy the variant's directory, e.g. `Sweet-Blue`, to `~/.local/share/icons/` (just for you) or `/usr/share/icons/` (for every user)

3. Set it as your icon theme (e.g. GNOME Tweaks -> Appearance -> Icons, or System Settings -> Colors & Themes -> Icons on KDE)

## Choosing the other icons

Icons that aren't folders come from the first theme in the `Inherits` line of the variant's `index.theme` that has them:
```ini
Inherits=candy-icons,breeze-dark,gnome,ubuntu-mono-dark,Mint-X,elementary,hicolor
```
To use another theme, put its directory name first, for example `breeze-extra-gnome`:
```ini
Inherits=breeze-extra-gnome,candy-icons,breeze-dark,gnome,ubuntu-mono-dark,Mint-X,elementary,hicolor
```
A package update overwrites `/usr/share/icons`; to keep the change, copy the variant to `~/.local/share/icons/` first and edit it there.
