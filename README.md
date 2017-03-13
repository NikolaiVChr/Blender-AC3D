#Blender-AC3D - Version 2.12

##What is it?
It's a few python scripts to import/export Inivis AC3D data into and out of Blender 2.63+. For earlier Blender 2.6x versions you need an older revision of the plugin (https://github.com/majic79/Blender-AC3D/tree/BL2.62)

##Why blender 2.6/2.7?
Because in the migration from 2.4X to 2.5, it lost AC3D support. This mod aims to bring that back to 2.6 and 2.7

##So it had it before?
Yes, this is mainly a port of those files to enable the import/export of .ac files in blender 2.5

##How do I install it?
open the blender/x.x/scripts/addons folder, then pull the io_scene_ac3d folder into the addons folder of blender. There's an alternative location you can drop it, at ~/.blender/x.x/scripts/addons (linux) or c:\Users\[username]\AppData\Roaming\Blender Foundation\Blender\x.x\scrips\addons (Windows 7+), where x.x is the version of Blender and [username] is the Windows user name.

##I can't see it in the import/export menu!
You'll need to enable the script in the user preferences window after installing it - open the user preferences window (File->User Preferences or Ctrl-Alt-U) and then go to the Add-on tab, click the button for Import-Export and then check the box on the right of "Import-Export: AC3D (.ac)"

##Uh, I've done all that how do I use it?
Go to File->Import->AC3D (.ac), select a file and let it do the work

##Why is export/import mirror color as emissive not longer checked by default?
In latest Blender versions mirror color is white per default, and that confused many users that what they exported would get totally emissive per default.

##Known Issues:

##Things to come:
* I want to have an option to overwrite, or to prompt the operator if they want to overwrite textures on an export

##Follow the discussion at:

http://www.flightgear.org/forums/viewtopic.php?f=18&t=13442

##Acknowledgments:

The Blender team: (http://www.blender.org) for such a fine piece of software
Willian P Gerano for his original work (the very first version of this script was a port of his original work)
Rene Negree for his help with the importer, tips on the texture mapping and materials and user settings saving
The FlightGear community for their help in testing and feedback for development

- BEGIN GPL LICENSE BLOCK -

  This program is free software; you can redistribute it and/or
  modify it under the terms of the GNU General Public License
  as published by the Free Software Foundation; either version 2
  of the License, or (at your option) any later version.

  This program is distributed in the hope that it will be useful,
  but WITHOUT ANY WARRANTY; without even the implied warranty of
  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  GNU General Public License for more details.

  You should have received a copy of the GNU General Public License
  along with this program; if not, write to the Free Software Foundation,
  Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301, USA.

- END GPL LICENSE BLOCK -
