# Gehl 125 Grinder for Middleburgh

- This Mod is customized for the Middleburgh, NY map by Nitrodad1115 (https://nitrodad1115.itch.io/fs22-middleburgh).
- The original Gehl Grinder is part of the Westby, WI map by MB Farms. (https://mb-farms.itch.io/fs22-westby-wi-4x-map)
- Suggestion of this conversion came from Mighty Mike Farms (https://www.youtube.com/watch?v=iu08CES6GAU)

Both mods `FS22_Gehl125_Westby.zip` & `FS22_Gehl125_Middleburgh.zip` are required.

## Installation Instructions
1. Download this release, put in your mod folder
2. Download the `WESTBYV2_BUILDINGS_UNZIP.zip` pack from the [Westby, WI download page](https://mb-farms.itch.io/fs22-westby-wi-4x-map) to a temporary location.
3. Unzip the file `WESTBYV2_BUILDINGS_UNZIP.zip`  and copy the zip `FS22_Gehl125_Westby.zip` in your mod folder.
4. Launch the game selecting the Middleburgh, NY map, and load only this mod - the original mod just needs to be in your mod folder, but doesn't need to be marked as installed when choosing mods.
5. Purchase the item in game as normal, and use as you would expect.

## Map Related Changes
This mod does *not* add in textures or allow you to put the output of the Grinder into any vehicle / trailer / silo. To use or store the bulk products created above while on the map - additional changes are needed to the Middleburgh, NY map `maps_fillTypes.xml` file - detailed in this video: https://youtu.be/iu08CES6GAU?t=414

1. Unzip the `FS22_Middleburgh.zip` file in place
2. Edit `FS22_Middleburgh/maps/mapUS/maps_fillTypes.xml` and make the following changes
   - In the `<fillTypes>` section, Copy the `<textures>` line from the `<fillType name="MAIZE">` section and add it to the similar `<fillType name="CRACKEDCORN">` further down the file.
   - In the `<fillTypes>` section, Copy the `<textures>` line from the `<fillType name="BARLEY">` section and add it to the similar `<fillType name="ROLLEDBARLEY">` further down the file.
   - In the `<fillTypeCategories>` section, you'll want to add `CRACKEDCORN ROLLEDBARLEY` to the following `fillTypeCategory` lines.
    - `<fillTypeCategory name="BULK">`
    - `<fillTypeCategory name="AUGERWAGON">`
    - `<fillTypeCategory name="TRAINWAGON">`
    - `<fillTypeCategory name="SHOVEL">`
    - `<fillTypeCategory name="FARMSILO">`
3. Save your changes to the file
4. Re-zip the `FS22_Middleburgh` folder to `FS22_Middleburgh.zip`

### Note on making map-related changes
Any time you forcefully unzip and edit a mod of any kind (in this case, a map), you are "diverging" from the mod as downloaded. This means a few things, and there are a few things to keep in mind.

- If the original mod is updated, and you either download via modhub or the web, the new file (since the filename is the same) will overwrite your changes.
  - To avoid that, if you have not used the mod yet - it's always advisable to change the mod-name for yourself to avoid this from happening. `FS22_Middleburgh_EDIT.zip` for example.
  - If the original mod is updated, you will need to re-make your changes on top of the new files.
- If you make changes to a mod for yourself, **DO NOT UNDER ANY CIRCUMSTANCES** upload said mod to any external site. Keep those changes for yourself.
  - If you feel like your changes can be shared with the community, do so through the original map author - reach out to them, let them know what you changed. In many cases map or mod authors are very responsive to making thier mods better; that said, if the mod author does not "accept" your suggestions,  **DO NOT UNDER ANY CIRCUMSTANCES** upload said mod to any external site. Keep those changes for yourself.
