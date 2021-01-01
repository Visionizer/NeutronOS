# STYLEGUIDE

## FILENAMES

NeutronOS uses the `.cpp` file extension for all CPP files and the `.hpp` extension for all header files that belong to cpp files.
Headers that are included in `.c` files are using a single `.h` 

## HOW TO IGNORE A FILE

If you want to ignore a file, but do not want to delete it (For example, if you want to work on it later but do not want to have it in a PR),
use the `.osignore.` extension. An example is this: `core.cpp` will not be ignored, but `core.osignore.cpp` will be ignored (This works with any file).
The files will still be registered as the original extension, but git will ignore it.

## IF EVERYTHING IN A FILE IS DEPRECATED,

use the `.deprecated.` extension, an example: `core.cpp` will become `core.deprecated.cpp`. Please only use this if there are 0 not deprecated
functions in the file. This file will not be ignored, this is just to show if something is deprecated.