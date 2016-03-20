# Linux Factorio Mod Installer

FMI is a simple perl script, which installs mods for the game [Factorio](www.factorio.com) from the [FactorioMods](www.factoriomods.com) site. Essentially, it processes factoriomods:// URIs using xdg-open.

## Install

1. The `.desktop` file needs to be copied to `/usr/share/applications/` or `~/.local/share/applications`.
2. The main script needs to be in your $PATH. eg, copy to `/usr/loical/bin/`.
3. Finally, you need to associate the url:

```
xdg-mime default factoriomod-installer.desktop x-scheme-handler/factoriomods

```
## Dependencies

The script uses `notify-send` for desktop notifications

