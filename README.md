# MOO1 Save Editor

A save-game editor for **Master of Orion 1** (version 1.3), for Windows.

Download the latest version from the [Releases page](../../releases/latest).

## What it does

- Shows the galaxy map of a save, drawn with the game's own graphics.
- **Planets:** edit any planet, including the computer players' planets: owner, population, factories, missile bases, environment, size, special, shields, spending, position and more.
- **Fleets:** change the ships in any fleet in orbit or in flight, add a fleet at any planet, redirect or delete a fleet in flight, and change how many are aboard a transport.
- **Ship designs:** add, edit and remove any empire's ship designs, with any component, whatever the empire has researched. Cost, space, speed and hit points are worked out the way the game does.
- **Technology:** give or take any technology for any empire, choose what it can research, and change its research in progress. Technology names are read from your own game files.
- Undo and redo for every change.

The editor only allows changes the game can load: every edit is checked against the game's own limits, and an edit that would break the save is refused with the reason.

## What you need

- Windows 10 or 11 (64-bit).
- Your own copy of Master of Orion 1, version 1.3. The editor contains none of the game's files; it reads the graphics from your game folder.

## How to use it

1. Download `moo_editor.exe` from the Releases page and run it. There is nothing to install.
2. The first time, choose **File > Set game folder...** and pick the folder Master of Orion is installed in.
3. Choose **File > Open...** and pick a save (`SAVE1.GAM` to `SAVE6.GAM` in the game folder).
4. Click a star to see its planet; double-click it to edit. Double-click a fleet or transport marker to edit it. Ship designs and technology are under the **Empires** menu.
5. **File > Save** writes the save. Load it in the game as usual.

Every time you save, the editor first keeps a timestamped backup copy of the save next to it, so a change can always be taken back.

Windows may warn about an unrecognised app the first time you run it, because the program is not signed. Choose "More info" and then "Run anyway".

## Notes

- This is a hobby project and comes with no warranty. Keep a copy of any save you care about.
- Not affiliated with or endorsed by the makers or publishers of Master of Orion.
- Thanks to the [1oom](https://github.com/1oom-fork/1oom) project, whose documentation of the save format made this possible.

## Problems

Please report problems on the [Issues page](../../issues), with the save file attached if you can.
