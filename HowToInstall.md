## How to install a mod

[[HOME]](index.md)

This works for every mod I created for Techtonica. Every other mod or every other game might not work this way.

### Install BepInEx

1. Download [this](https://github.com/BepInEx/BepInEx/releases/download/v5.4.21/BepInEx_x64_5.4.21.0.zip) .zip file.
2. Extract it in the game folder. (normally `C:\Program Files (x86)\Steam\steamapps\common\Techtonica`)
3. Launch the game via steam or by launching `Techtonica.exe`. (This start is required before installing mods)

### Install a mod

1. Download the mod .zip file.
2. Extract the mod file into `[game folder]\BepInEx\plugins`.
3. Done!

### Check if a mod is working

1. Open `[game folder]\BepInEx\LogOutput.log` or `%appdata%\..\LocalLow\Fire Hose Games\Techtonica\Player.log`. (you can paste the second path in the file explorer path)
2. Search for `[Message:   BepInEx] Chainloader started`
3. no)  If you didn't found that message BepInEx did not correctly start.
3. yes) If you found that message look at the next lines. Does one of the following lines equals `[Info   :   BepInEx] Loading [<ModName> <ModVersion>]`?
4. no)  If this is not the case BepInEx didn't recognize the mod. Report this as a bug on the mod site (probably nexusmods).
4. yes) If this is the case check if the next line starts with `[Info   :<ModName>]` and continues with a loading success message.
5. no)  If this is not the case the mod failed to load. Report this as a bug on the mod site (probably nexusmods).
5. yes) If this is the case the mod loaded successful.
6. If you think the mod doesn't work anyway look for any errors that contain the mod name in `[game folder]\BepInEx\LogOutput.log`. If you find an error report this as a bug on the mod site (probably nexusmods).

[[HOME]](index.md)
