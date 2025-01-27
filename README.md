# Blender-AC3D - Version 2.27

## About
It's a few python scripts to import/export Inivis AC3D data into and out of Blender 2.63 to Blender 2.79.

## Download

| Blender Version                                                                                         | 
|---------------------------------------------------------------------------------------------------------|
| [Download for Blender 4.3](https://github.com/NikolaiVChr/Blender-AC3D/archive/refs/heads/4.3.zip)      |
| [Download for Blender 4.1](https://github.com/NikolaiVChr/Blender-AC3D/archive/refs/heads/4.1.zip)      |
| [Download for Blender 4.0](https://github.com/NikolaiVChr/Blender-AC3D/archive/refs/heads/4.0.zip)      |
| [Download for Blender 3.2](https://github.com/NikolaiVChr/Blender-AC3D/archive/refs/heads/3.2.zip)      | 
| [Download for Blender 3.0](https://github.com/NikolaiVChr/Blender-AC3D/archive/refs/heads/3.0.zip)      |
| [Download for Blender 2.80](https://github.com/NikolaiVChr/Blender-AC3D/archive/refs/heads/2.80.zip)    |
| [Download for Blender 2.7.9](https://github.com/NikolaiVChr/Blender-AC3D/archive/refs/heads/2.79.zip)   |
| [Download for Blender 2.6.x](https://github.com/NikolaiVChr/Blender-AC3D/archive/refs/heads/bl2.6.zip) |

## Why blender 2.6/2.7?
Because in the migration from 2.4X to 2.5, it lost AC3D support. This mod aims to bring that back to 2.6 and 2.7

## So it had it before?
Yes, this is mainly a port of those files to enable the import/export of .ac files in blender 2.5

## How do I install it?
open the blender/x.x/scripts/addons folder, then pull the io_scene_ac3d folder into the addons folder of blender. There's an alternative location you can drop it, at ~/.blender/x.x/scripts/addons (linux) or c:\Users\[username]\AppData\Roaming\Blender Foundation\Blender\x.x\scripts\addons (Windows 7+), where x.x is the version of Blender and [username] is the Windows user name.

## I can't see it in the import/export menu!
You'll need to enable the script in the user preferences window after installing it - open the user preferences window (File->User Preferences or Ctrl-Alt-U) and then go to the Add-on tab, click the button for Import-Export and then check the box on the right of "Import-Export: AC3D (.ac)"

## Uh, I've done all that how do I use it?
Go to File->Import->AC3D (.ac), select a file and let it do the work

## Why is export/import mirror color as emissive not longer checked by default?
In latest Blender versions mirror color is white per default, and that confused many users that what they exported would get totally emissive per default.

## Known Issues:
- If exporting when in Edit mode, it will not export the last edits done in Edit mode. Best is to export when in Object mode.
- When importing lines, they cannot be assigned UV coordinates as Blender does not support that.
- When exporting lines, they will always be smooth shaded, due to limitations in Blender.
- When exporting lines they will have the DefaultWhite material, except if their Blender object has only 1 and only 1 material, then they will be assigned that. This is due to Blender limitation.
- Exporter will export all materials in object material slots, even if they are not referenced. Good if you had a material you might want to assign to something later. Also annoying cause it potentially can clutter up the AC3D file with unused materials.

## Things to come:
* I want to have an option to overwrite, or to prompt the operator if they want to overwrite textures on an export

## Follow the discussion at:

https://forum.flightgear.org/viewtopic.php?f=18&t=13442

## Complete file format specification, anno 2017

https://sites.google.com/view/ac3dfileformat/home

## Acknowledgments:

- The Blender team: (http://www.blender.org) for such a fine piece of software
- Willian P Gerano for his original work (the very first version of this script was a port of his original work)
- Rene Negree for his help with the importer, tips on the texture mapping and materials and user settings saving
- The FlightGear community for their help in testing and feedback for development

## License

This project is licensed under the GNU GPLv2. See [LICENSE.md](LICENSE.md).
