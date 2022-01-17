# MapMarkers
[Slime Rancher](http://slimerancher.com/) mod for [SRML](https://www.nexusmods.com/slimerancher/mods/2) that adds custom markers to the in-game map.

## Implemented Features
- Show discovered Treasure Pods on the map, a Treasure Pod counts as discovered once the player looks at it from close enough so that the open/upgrade required UI text shows up (an audio cue will be played).
- Commands:
    - *showalltreasures*: toggles if all treasure pods should be shown on the map (default: false)
    - *showopenedtreasures*: toggles if already opened treasure pods should be shown on the map (default: true)
    - *resetdiscoveredtreasures*: resets all locked treasure pods to undiscovered (no longer shows them on map)

## Planned Features
- Custom markers that can be added by clicking on the map

## Install
1. Install SRML
2. Download the latest *MapMarkers.zip* from [NexusMods](https://www.nexusmods.com/slimerancher/mods/279)
3. Extract *MapMarkers.dll* from the archive
4. Move *MapMarkers.dll* to `<slime rancher game folder>/SRML/Mods`

## Build
1. Clone the repo
2. You may have to fix you References, this project needs:
    - *0Harmony.dll* - found in  `<slime rancher game folder>/SRML/Libs`
    - *Assembly-CSharp_old.dll* - found in `<slime rancher game folder>/SlimeRancher_Data/Managed`
    - *SRML.dll* - found in `<slime rancher game folder>/SlimeRancher_Data/Managed`
    - *UnityEngine.CoreModule.dll* - found in `<slime rancher game folder>/SlimeRancher_Data/Managed`
    - *UnityEngine.AssetBundleModule.dll* - found in `<slime rancher game folder>/SlimeRancher_Data/Managed`
    - *UnityEngine.PhysicsModule.dll* - found in `<slime rancher game folder>/SlimeRancher_Data/Managed`
    - *UnityEngine.UI.dll* - found in `<slime rancher game folder>/SlimeRancher_Data/Managed`
3. Make sure that the resource *mapmarkers.assetsBundle* is correctly configured and its *Build Action* is set to *Embedded Resource*
4. Build the solution, the output *MapMarkers.dll* is located at `<project folder>/bin/Debug/MapMarkers.dll`