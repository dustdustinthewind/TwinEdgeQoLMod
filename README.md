# TwinEdgeQoLMod
primarily an editor mod for twin edge that makes advanced "glitch" mapping features accessible within the in-game editor

ask for help or questions or suggestions or idfk on #dusts-mod channel on twin edge discord here: https://discord.gg/hAX6TDvZGY

#### how to install
- download the version for your os:
  - windows: https://github.com/dustdustinthewind/TwinEdgeQoLMod/raw/main/Windows/Assembly-CSharp.dll
  - mac: https://github.com/dustdustinthewind/TwinEdgeQoLMod/raw/main/Mac/Assembly-CSharp.dll
  - (i can make a linux version if needed)
- right click twin edge in steam > click on "managed" > "browse local game files"
- for windows:
  - open "TwinEdge_Data" then open "Managed"
- for mac:
  - right click "TwinEdge.app", and click "Show Package Contents"
  - go into "Contents" then "Resources" then "Data" then "Managed"
- drag'n'drop the file you downloaded earlier into this "Managed" folder
- mod installed, restart twin edge to see changes

#### how to revert to vanilla
- close Twin Edge
- right click twin edge in Steam, click on "properties" > "local files"
- click on "verify integrity of game files..."
- steam will change the game back to vanilla
- game updates will also remove the mod

#### features/changes
- Colors are no longer clamped (can go from 0-255) ([vid](https://youtu.be/uZcW6QnpZYs))
   - Be careful with this, high values can brighten the screen so much it's hard to see. Gameplay will be brighter than the Editor
- Can select between "Hold Start" and "Hold End" notes ([vid](https://youtu.be/wex8bXg_bCs))
  - Hold Starts should act nearly identical to vanilla "Hold"
  - Hold Ends change the note to a Hold End (release input)
- Changed how Hold Notes render in editor to more accurately represent gameplay
- Removed checks for side swapping a selection of notes
  - Necessary for chain holds and other hold manipulations
  - Be careful when swapping, you can stack notes or cause weird bugs. There's a reason vanilla had this check.
- Can buy any skin without the necessary stars
- Map doesn't save when opening the "Upload to Workshop" panel or when you click "publish" (useful for .song editing)
- Undo history tepss increased to 1000
- Workshop Description Limit has been increased from 1000 characters to 8000 characters
   - Note: Steam Workshop Description only allows 8000 bytes, not 8000 characters. I think most European characters are 1 byte though.
- Custom note angles in editor
  - First click on "new angle" to tell the editor you want to modify this angle. Then input your angle in the angle text box. You can use the preview to help figure out where the note will be.
  - Note: Twin Edge calculates the angle of default notes using the angle before it, make sure the last custom angle you make is lined up with the cursor so default notes continue to line up after the custom angles.
  - Note: Angle 0 is the angle of the very first note of each hand for that map (left hand will have a different angle 0 than right hand unless you started the map with a chord (note on each hand at same time))
- Removed rotation speed limits
- Can zoom into to level 50
- Can slow down playback to .125x
- Increased limits for custom events
  - no caps on custom speed changes
  - higher limits for flash, fadeout, special section, scale circle, audio band, and chromatic abberation events
