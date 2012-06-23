ABOUT
=====

libKiCad is a compilation of footprints and 3d models of various electronics
components for the KiCad EDA (http://www.kicad-pcb.org/).

The footprint and 3d libraries are based on the Walter Lain's kicad library
(http://smisioto.no-ip.org/elettronica/kicad/kicad-en.htm).

In addition to the original libraries, the following improvements have been 
made:
+ The structure of the library have been changed to make it cross-platform
  (tested on Ubuntu and Windows).

LICENSE
=======

This library is licensed under the:
Creative Commons license v3.0, Attribution-Share Alike (CC BY-SA 3.0).
For further details see LICENSE.3D.txt and LICENSE.FOOTPRINT.txt.

INSTALLATION AND USE
====================

Get the library using:

git clone https://github.com/JorgeAparicio/libKiCad.git

This library and all your kicad projects must be inside the same folder for
proper integration. Your directory should look like the following example.

<path/to/projects>
    awesomeProject
        awesomeProject.pro
        awesomeProject.sch
        awesomeProject.brd
        ...
    coolProject
        coolProject.pro
        coolProject.sch
        coolProject.brd
        ...        
    libkicad
        3d
            ...
        footprint
            ...
        README
	...

Open your project .brd file (e.g. awesomeProject.brd) in KiCad's pcbnew, go to
preferences > library, remove the default libraries and add all the .mod files
under libKiCad/footprint.

SCHEMATIC SYMBOLS
=================

If you need schematic symbols you should look at the latest KiCad official
library (https://code.launchpad.net/~kicad-lib-committers/kicad/library).

