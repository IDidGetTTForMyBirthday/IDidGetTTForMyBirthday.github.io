## Meme Language Mod

[[HOME]](index.md)

This mod changes the name of some ingame object to "meme" names. The names are chosen by the community and are based on jokes. For example "Power Floors" are renamed to "Uppy Downy Supporties".

### Download

[Download on Nexusmods](https://www.nexusmods.com/techtonica/mods/1)

[How to install a mod](HowToInstall.md)

### Details

This mod changes the name of some ingame object as well as research to "meme" names. The names are chosen by the community and are based on jokes.
Current name changes:
- Power Floor     -->   Uppy Downy Supporties
- Floors          -->   Supporties
- Inserter        -->   Handy Mandy
- Long Inserter   -->   Long Larry
- Stack Inserter  -->   Stacky Jackie
- Fast Inserter   -->   Rapid Randy
- Filter Inserter -->   Picky Ricky
- Biobrick        -->   Flower Power
- Advanced Belt   -->   Jas Belts
- Containers      -->   Boxy Bertha

### Informations about bug and error safety

#### Version 1.0.0
This version might creates game bugs or errors. This version is achieved and **should not be used**!

#### Version: 1.1.0+
It's unlikely **but not impossible** that this version creates game bugs or errors.

#### Addidtional informations for the devs of Techtonica

This mod only executes code at two moments when the mod is loaded at game startup and when the game finished loading before the "Click any button to continue" message.

The mod loading should always work except Harmony fails to patch `LoadingUI.OnFinishLoading` (if this function is removed or the name is changed this will fail). If the mod loading fails this mod automatically disables itself. This is written as an warning in the log.

The second time the mod executes code is as soon as `LoadingUI.OnFinishLoading` is called. This function is changed using Harmony to rename all defined object before executing the original code.

#### Data

.NETFramework version: `4.6.2`

BepInEx.Core version: `5.4.21`

Mod GUID: `io.github.ididgetttformybirthday.MemeLanguage`

[[HOME]](index.md)
