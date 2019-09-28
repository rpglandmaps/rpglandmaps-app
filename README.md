# rpglandmaps-app
## Contents 
[Intro](https://github.com/rpglandmaps/rpglandmaps-app/blob/master/README.md#Intro)

[Layouts and Controls](https://github.com/rpglandmaps/rpglandmaps-app/blob/master/README.md#Layouts)

[Displays](https://github.com/rpglandmaps/rpglandmaps-app/blob/master/README.md#Displays)

[Mouse Display Control](https://github.com/rpglandmaps/rpglandmaps-app/blob/master/README.md#Mouse)

 [Keyboard Shortcuts](https://github.com/rpglandmaps/rpglandmaps-app/blob/master/README.md#Keyboard)

[Setting Dialogs](https://github.com/rpglandmaps/rpglandmaps-app/blob/master/README.md#Setting)

 [Orbit and Pans](https://github.com/rpglandmaps/rpglandmaps-app/blob/master/README.md#Orbit)

 [Grid](https://github.com/rpglandmaps/rpglandmaps-app/blob/master/README.md#Grid)

 [Dayand Night](https://github.com/rpglandmaps/rpglandmaps-app/blob/master/README.md#Day)

[Version Number Control](https://github.com/rpglandmaps/rpglandmaps-app/blob/master/README.md#Version)

<a name="Intro"/>

# Intro
RpgLandMaps is a windows application built in unity3d to view and control 3d top down animated tabletop roleplay maps of land, villages, towns and city maps. It is for use on any tabletop roleplay games (like D&D, RuneQuest, etc thats your choice), Using a ceiling mounted projector, or table top mounted TV as secondary or duplicated screen. 

The GM/DM is able to control the main view, by pan and zoom mode or orbit views. Control the grid visibility, size and colour. Also day and night control with a random (bias controlled) lights on for building lights at night.

The maps areas of land, to facilitate encounters, adventures, and campaigns and hopefully not let players feel like they are fenced in by the map edges and thus fully immersed into the world, and understand where they are. Also each application can include sub maps (for example The Tavern, keep, tower, temple interiors), and each sub map can have save locations that can be jumped to. Control to swap objects can be pre programed in so i can build both the castle wall and breached versions.

Detail of mpas is a complex subject, that includes performance of PC, Enough detail to inspire GM/DM and players, but leave room for GM/DM to add elements by storytelling.

The maps are drawn in 3d, using either custom home brew drawn objects and or prefabs.I plan to slowly ramp up the size/detail and include such technologies as LOD and Occlusion to add performance, and add more animated items (such as wildlife, birds etc), weather controls, and sounds controlled by location

<a name="Layouts"/>

# Layouts and Controls
<a name="Displays"/>

## Displays
The main window has 2 layouts “Full Screen” or “Control View” and can also display the map view in fullscreen on a seperate display. 
![Displays jpg](https://github.com/rpglandmaps/rpglandmaps-app/blob/master/displays.jpg?raw=true)

1. Current Map name (see Locations on how to change) (only on both primary display views)
2. Main Icon Control Panel (only on both primary display views)
   - Orbit Pan view toggle.
   - Grid on off toggle
   - Day night toggle
   - Send to secondary display (no way in unity to deactivate secondary display one activated, so close and reopen is only option to switch back to single display)
   - Full Screen Control view toggle
3. Locations tree view of sub maps and saved locations (only on primary display contol views)
   - Sub map with add location using current view state button (only on current active sub map)
   - Save Locations with view orbit or pan icon, name and delete location button (only on current active sub map)
4. Location name edit and location notes for GM/DM to add what they need / want. (only on primary display contol views)

![Control View Locations jpg](https://github.com/rpglandmaps/rpglandmaps-app/blob/master/Layout%20Control%20View.JPG?raw=true)

Note
The Control view is done in a dark theme so as not to distract from any mood lighting and aid GM/DM viewing.
Where possible I want to use universal icons (hieroglyphic controls) so as to make it un nationality and language specific.
<a name="Mouse"/>

## Mouse Display Control
Mouse controls for view 
### Orbit View Mode
- Left Button and Drag = Orbit map around target point.
- Middle Button and Drag = Drag map.
- Right Button and Drag = Zoom map
- Scroll Wheel = Zoom map
### Pan View Mode
- Left Button and Drag = Pan map
- Middle Button and Drag = Rotate map
- Right Button and Drag = Zoom map
- Scroll Wheel = Zoom map
<a name="Keyboard"/>

## Keyboard Shortcuts
- ALT+F4 = Close application
- ALT+Enter = Toggle windowed full screen of single display view (standard Unity control and thus not available in dual display mode).

- CTRL-A = Toggle activation of animate mode where the camera will in pan mode will travel between all pan mode saved locations, and in orbit mode will rotate around the current view target location.
- CTRL-C = Go back to map predefined start position as specified by the map in the application (hard coded)
- CTRL-D = Toggle day night view mode
- CTRL-G = Toggle grid display
- CTRL-H = Toggle display of map name and control icons (only on single display full screen mode)
- CTRL-I = Save a 1920 x 1080 png image of current view in the unity “Application.dataPath”, the file name will be the current Map name and prefixed with “Night” if in night mode and " y" + pady + " x" + padx + ".png"
- CTRL-M = Save current view as a saved location to current map.
- CTRL-Left Cursor Arrow = Jump to previous saved location.
- CTRL-Right Cursor Arrow = Jump to next saved location.
- CTRL-O - Toggle orbit pan view modes, it will save last location view position and angle so when toggling back the last view will be restored, allowing the GM/DM to go from pan mode to orbit and show players whats around)
- CTRL-S = Save map data settings, names, locations to disk now, the file will be located in the unity “Application.dataPath” and called “MapData.save"

<a name="Setting"/>

# Setting Dialogs
Right click on the Orbit Pan, Grid, or Day Night icons will open up relevant settings dialogs so the GM/DM can adjust control and display settings as desired
<a name="Orbit"/>

## Orbit and Pan
- Pan Speed (Slider) = Set mouse pan mode speed
- Pan Scroll Speed (Slider) = Set mouse pan mode scroll zoom speed
- Orbit Pan Speed (Slider) = Set mouse orbit mode pan speed
- Orbit Speed (Slider) = Set mouse orbit mode speed
- Orbit Scroll Speed (Slider) = Set mouse orbit mode scroll zoom speed
![Orbit Pan Settings Dialog](https://github.com/rpglandmaps/rpglandmaps-app/blob/master/Settings%20Orbit%20Pan.JPG?raw=true)
<a name="Grid"/>

## Grid
- Grid Type (Dropdown) = Select grid type (only rectangle atm)
- Grid Size (Slider) = Set grid size
- Grid Colour (RGB Spectrum Image) = Select grid colour.
- Grid Alpha (Slider) = Select grid alpha value.
![Grid Settings Dialog](https://github.com/rpglandmaps/rpglandmaps-app/blob/master/Settings%20Grid.JPG?raw=true)
<a name="Day"/>

## Day and Night
- Night Lights on Random Bias = Set the value of random lights on (low = none, mid = 50%, and high = all) 
![Day Night Settings Dialog](https://github.com/rpglandmaps/rpglandmaps-app/blob/master/Settings%20Day%20Night.JPG?raw=true)

<a name="Version"/>

# Version Number Control
At the moment all maps on patreon page are single display without save locations and notes etc. I want to back port them but will take time. This is Version 1-0-0 and thus any map will be published with the version number prefixed to map name so you can see if the version you have downloaded is older than the offered version, and thus update.

And this github is to track any issues suggestions for this application

Many thanks


