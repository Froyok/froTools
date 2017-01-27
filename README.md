```
///////////////////////////////////////////////////////////////////////
///////////////////////////////////////////////////////////////////////

  ####                  ######                  ####
 ##                       ##                      ##
 ##     ##  ##   ####     ##     ####    ####     ##     #####
 ##     ## ###  ##  ##    ##    ##  ##  ##  ##    ##    ##
######  ###     ##  ##    ##    ##  ##  ##  ##    ##    ##
 ##     ##      ##  ##    ##    ##  ##  ##  ##    ##     ####
 ##     ##      ##  ##    ##    ##  ##  ##  ##    ##        ##
 ##     ##      ##  ##    ##    ##  ##  ##  ##    ##        ##
 ##     ##       ####     ##     ####    ####   ######  #####
///////////////////////////////////////////////////////////////////////
///////////////////////////////////////////////////////////////////////
```

Current version : **3.3**

The ***froTools*** is a toolset for **Autodesk Maya** to speed up your modeling workflow. This game content oriented script allow you a quicker access to the common tools that you use in Maya when you do polygonal modeling. It also provide a lot of new tools to make some task more easy to perform.

This script also provide : 
 * A quick exporter for the FBX and OBJ format
 * Custom hotkeys dedicated to the functions inside the froTools
 * New UV window with custom tools


# How to Install ?
Put the content of the folder "froTools" inside your "My Documents/Maya" folder. **Example** : "My Documents\maya\2011-x64\"

This script has been tested and works properly with :
 * Maya 2011
 * Maya 2012
 * Maya 2013
 * Maya 2014
 * Maya 2015
 * Maya 2016
 * Maya 2017

# How to Launch ?
Call the command below in the mel command line for the first time. You can use the “Make Shelf Button” to make a shelf button in your current shelf.
```c++
source froTools3.mel; froTools3();
```

You can also add the froTools to launch when Maya start, to do so, open the **userSetup.mel** file (create it if it doesn’t exist) inside your script folder (where **froTools3.mel** is located) and put the following line inside it :
```c++
eval("froTools3");
```

# Documentation

Documentation can be found on the following page :

http://www.froyok.fr/blog/2012-12-frotools-3-2-new-enhanced-ui-and-tools


# Contact
For additional contacts and requests you can reach out via my website or Twitter :
 * http://www.froyok.fr
 * https://twitter.com/Froyok

# Changelog

## 3.3
 * Added support for Maya 2015/2016/2017 (fixed bugs and broken functions)
 * Added Edge Outline/Border selection from selected faces
 * Added a mesh analyzer (polycount, mesh size, and so on)
 * Added a system that store the previous state of the Frames when the script is reloaded
 * Added a checkBox to dock/undock the window (which will remember the setting)
 * Added new pivot tool : select a face and move an object on it (helper for floating geometry)
 * Added new pivot tool : min/max based on world space bounding box
 * Added new pivot tool : copy a pivot point from one object to one another
 * Added the "groups" option for the OBJ exporter
 * Added new Normal tool : copy a vertex normal to other vertices
 * Added new button to toggle the x-ray mode per (selected) object
 * Updated export function to be more robust
 * Updated FBX export compatibility (deprecated commands from Maya 2014/2016)
 * Updated FBX combined export to support Triangulation
 * Updated the "move to ori" button, now also splitted into separate axis (available with other pivot tools)
 * Updated every icons as a "shelf button" to allow drag'n'drop to the shelf (and Maya 2014 modeling toolkit)
 * Updated the selection conversion, now available by double-clicking on a component icon
 * Updated the "toggle normals" visibility (now cycling between face and vertex normals)
 * Updated the "look at me" normal tool, now each vertex normal is individual
 * Updated the Mesh creation buttons to set the vertex normals on "Unweighted" by default
 * Updated the combine and merge tool to set the mesh control on "Unweighted"
 * Updated the combine and combine merge tool to avoid the transform creation (aka delete history)
 * Updated the grid subdivision shortcut for the UV window (now changing the main grid)
 * Updated the default FBX version for the quick exporter to 2013 (was on 2011)
 * Updated the UV window (the screen size is now stored per maya session, making it faster to load)
 * Fixed triangulation function during export (could fail and bring up an error sometimes)
 * Fixed the froTools Window position preferences when using the "floating" mode
 * Fixed the float field in the UV window when setting a custom scale (now accepting multiple decimals)
 * Fixed the Orient face normals tool (error with specific geometry configuration, thx to Passerby)
 * Fixed the abs() function error with the "BestOrtho" tool (function withing a function error).
 * Fixed "Unhide all meshes" function (which was disabled for no reason)
 * Fixed a conflict between the froTools3 and the froXnormal when creating a shelfbutton
 * Fixed the UI size in the "Settings" tab (export path was too big)
 * Fixed the "Vertex size" slider to allow to go back to Maya default vertex size (3 instead of 6)
 * Removed the UV focus when opening the UV window (not working properly)
 * Removed FBX Triangulation setting (because different from Maya Triangulation)
 * Removed support for Maya version older than 2011
