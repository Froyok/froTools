# froTools

Current version : **3.2.5**

The froTools is a toolset for **Autodesk Maya** to speed up your modeling workflow. This game content oriented script allow you a quicker access to the common tools that you use in Maya when you do polygonal modeling. It also provide a lot of new tools to make some task more easy to perform.

This script also provide : 
 * A quick exporter for the FBX and OBJ format
 * Custom hotkeys dedicated to the functions inside the froTools
 * New UV window with custom tools


# How to Install ?
Put the content of the folder "froTools" inside your "My Documents/Maya" folder.
Ex : "My Documents\maya\2011-x64\"
This script has been tested and works properly with :
 * Maya 2011
 * Maya 2012
 * Maya 2013
 * Maya 2014

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
