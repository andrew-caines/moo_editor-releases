# MOO1 Save Editor

A save-game editor for **Master of Orion 1** (version 1.3), for Windows and Linux.

Download the latest version from the [Releases page](../../releases/latest).

## What it does

- Shows the galaxy map of a save, drawn with the game's own graphics, in a screen and windows dressed like the game's own. The map is alive: stars twinkle, nebulae pulse, and a star field drifts behind it all.
- **Planets:** edit any planet, including the computer players' planets: owner, population, factories, missile bases, environment, size, special, shields, spending, position and more.
- **Fleets:** change the ships in any fleet in orbit or in flight, add a fleet at any planet, redirect or delete a fleet in flight, and change a transport's destination and how many are aboard. A fleet's or transport's course is drawn on the map with an arrow.
- **Ship designs:** add, edit and remove any empire's ship designs, with any component, whatever the empire has researched. Cost, space, speed and hit points are worked out the way the game does.
- **Empires:** each empire's tab opens with its race's portrait and a summary: home world, planets, population, factories, ships, reserve and tech levels.
- **Technology:** give or take any technology for any empire, choose what it can research, and change its research in progress. Technology names are read from your own game files.
- Undo and redo for every change.

The editor only allows changes the game can load: every edit is checked against the game's own limits, and an edit that would break the save is refused with the reason.

## What you need

- **Windows:** Windows 10 or 11 (64-bit).
- **Linux:** a 64-bit (x86_64) desktop Linux as new as Ubuntu 22.04 or later (glibc 2.35 or newer), with X11 or Wayland.
- Your own copy of Master of Orion 1, version 1.3. The editor contains none of the game's files; it reads the graphics and technology names from your game folder.

## Download and run

**Windows:** download `moo_editor.exe` from the Releases page and run it. There is nothing to install. Windows may warn about an unrecognised app the first time, because the program is not signed: choose "More info" and then "Run anyway".

**Linux:** download `moo_editor-linux-x86_64.tar.gz` from the Releases page, then in a terminal:

```
tar -xzf moo_editor-linux-x86_64.tar.gz
./moo_editor
```

There is nothing to install; the program is a single file. The game folder is the one holding the game's `.LBX` files, for example the game's folder inside a DOSBox or GOG install; the files' names can be upper or lower case. Settings are kept in `~/.config/moo_editor/`.

If the folder dialog cannot be shown on your system, give the game folder on the command line once and it is remembered:

```
./moo_editor --game-dir /path/to/moo
```

## How to use it

1. Start the editor.
2. The first time, choose **File > Set game folder...** and pick the folder Master of Orion is installed in.
3. Choose **File > Open...** and pick a save (`SAVE1.GAM` to `SAVE6.GAM` in the game folder).
4. Click a star to see its planet; double-click it to edit. Double-click a fleet or transport marker to edit it. Pick an empire from the **Empires** menu for its ship designs and technology; the window that opens has a tab for every empire.
5. **File > Save** writes the save. Load it in the game as usual.

Every time you save, the editor first keeps a timestamped backup copy of the save next to it, so a change can always be taken back.

## Notes

- This is a hobby project and comes with no warranty. Keep a copy of any save you care about.
- Not affiliated with or endorsed by the makers or publishers of Master of Orion.
- Thanks to the [1oom](https://github.com/1oom-fork/1oom) project, whose documentation of the save format made this possible.

## Problems

Please report problems on the [Issues page](../../issues), with the save file attached if you can.
