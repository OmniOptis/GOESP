# GOESP

# GOESP
[![Windows](https://github.com/danielkrupinski/GOESP/workflows/Windows/badge.svg?branch=master&event=push)](https://github.com/danielkrupinski/GOESP/actions?query=workflow%3AWindows) [![Linux](https://github.com/danielkrupinski/GOESP/workflows/Linux/badge.svg?branch=master&event=push)](https://github.com/danielkrupinski/GOESP/actions?query=workflow%3ALinux)

Cross-platform streamproof ESP hack for CS:GO. Currently supports Windows and Linux.

## Showcase

### Hit Effect (new!)

![Hit Effect](https://i.imgur.com/pQUBuS4.gif)

### Player List

![Player List](https://i.imgur.com/Hvc4Olk.png)

### Menu

![Menu](https://i.imgur.com/3zvz2us.png)

### Purchase List

![Purchase List](https://i.imgur.com/V4lIx1G.png)

### Player ESP

![Player ESP](https://i.imgur.com/l4cOW0c.png)

## Getting started

### Prerequisites

#### Windows
Microsoft Visual Studio 2019 (preferably the latest version), platform toolset v142 and Windows 10 SDK are required in order to compile GOESP. If you don't have ones, you can download VS [here](https://visualstudio.microsoft.com/) (Tools and Windows SDK are installed during Visual Studio Setup).

`GOESP` folder should have been succesfully created, containing all the source files.


## FAQ

### How do I open menu?
Press <kbd>INSERT</kbd> while focused on CS:GO window.

### Can I use custom font in the ESP?
Of course. After installing new font you have to unload and load GOESP again.

### Does this hack hook any of game engine functions?
Nope. Functions GOESP hooks are:

on windows:
-   DirectX Present & Reset from overlay
-   SetCursorPos from overlay
-   game window WNDPROC

on linux:
-   SDL_PollEvent
-   SDL_GL_SwapWindow

### How GOESP renders its stuff?
GOESP hooks game overlays and draw things using them. Currently supported overlays are Steam and Discord.

### Is the ESP visible on recording?
Nope, but you have to use 'Game capture' instead of 'Window capture' or 'Desktop capture'. Also remember to uncheck 'Capture external overlays' option in your recording software.

### Can I use this alongside other cheats?
Yes, GOESP shouldn't collide with any other game modification.
