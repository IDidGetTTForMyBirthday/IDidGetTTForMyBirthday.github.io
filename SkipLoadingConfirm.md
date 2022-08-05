## Skip Loading Confirm Mod

[[HOME]](index.md)

This mod skips the loading confirmation.

### Download

`The mod will be available soonTM`

[How to install a mod](HowToInstall.md)

### Details

This mod starts the game as soon as it finished loading so you don't have to press a key anymore. This is useful for example when you want to go away while Techtonica loads and want that your factory runs as soon as the game finished loading without you being back.

### Informations about bug and error safety

It's unlikely **but not impossible** that this mod creates game bugs or errors.

#### Addidtional informations for the devs of Techtonica

This mod only executes code at two moments when the mod is loaded at game startup and when the game finished loading.

The mod loading should always work except Harmony fails to patch `LoadingUI.OnFinishLoading` (if this function is removed or the name is changed this will fail). If the mod loading fails this mod automatically disables itself. This is written as an warning in the log.

The second time the mod executes code is as soon as `LoadingUI.OnFinishLoading` is called. Then `LoadingUI.confirmedLoad` will be set to true and `DJManager.OnFinishInit` will be called.

#### Data

.NETFramework version: `4.6.2`

BepInEx.Core version: `5.4.21`

Mod GUID: `io.github.ididgetttformybirthday.SkipLoadingConfirm`

[[HOME]](index.md)
