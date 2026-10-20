# Potato Hack

**Potato Hack** is a trainer for World of Warcraft 3.3.5a (build 12340).

## Usage

1. Launch WoW 3.3.5a (build 12340).
2. Run `PotatoHack.exe` and click **Attach**. If the game is running as Administrator, the trainer must also be run as Administrator.
3. Until your character enters the world, the status will display `waiting for a character in world…`. Code patch features such as Mount, No Clip, Water Walk, and Infinite Jump can be enabled even from the login screen.
4. Settings, hotkeys, and waypoints are saved to `potato.ini` in the same directory as the executable.

### Scale Controls

The `+` and `−` buttons must be used in-game, with your character already in the world. Scale is a character-specific property, and the player object does not exist on the login screen.

These buttons are no longer disabled. If you press either one before entering the world, a message will explain that you need to log in first.

Clicking **Attach** only attaches the trainer to the game process. It does not create a character or log you in.

## Default Hotkeys

All hotkeys can be changed in the `[Hotkeys]` section of `potato.ini`.

| Key | Function |
|---|---|
| F1 | Fly |
| F2 | Speed |
| F3 | Wallclimb |
| F4 | Super Jump (hold Space) |
| F5 | Freeze Z |
| F6 | Water Walk |
| F7 | Infinite Jump |
| F8 | Mount Indoors |
| F9 | No Clip |
| F10 | Go to Corpse |

Hotkeys are polled rather than intercepted, so the game can still receive the same key presses. They are temporarily disabled while typing in text fields.

Each hotkey is saved by name in `potato.ini`, for example:

```ini
Fly=F1
WaterWalk=F6
```

## Keep Functions Active After Exit

By default, closing the trainer restores all patches and modified values to their original state.

Enable **Keep functions active after exit** to leave the changes in the game's memory after the trainer closes. This works similarly to the **Continue After Exit** option found in the original trainer.