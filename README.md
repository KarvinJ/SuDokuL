# SuDokuL
This is a Sudoku game made in C++ and SDL2. It's currently available for Switch, Wii U, Vita, PC, and Android.

## Features
- Play Sudoku puzzles of Easy, Normal, Hard, or Very Hard difficulty
  - These puzzles are generated on-demand using a built-in algorithm; however, to eliminate computation time on weaker devices, Hard and Very Hard puzzles have been pre-generated.
- Mouse, keyboard, controller, and touch screen support
- Supports many resolution options ranging from 320x240 to 5120x2160
- Scrolling background with customizable settings (size, scroll speed, angle)
- Calm and envigorating MOD music to suit your mood
- Shaded text for a nice, 3D look
- Runs on a potato
- Optional auto-fill cheat, in case you get stuck

## Screenshots (click for full size)

All screenshots are from PC version 1.11 (unless otherwise specified) and can be found in the [screenshots](https://github.com/Mips96/SuDokuL/tree/main/screenshots) folder.

<img src="https://github.com/Mips96/SuDokuL/blob/main/screenshots/screenshot-1920-1080_1.png?raw=true" width="480" height="270"/>

This game was initially designed for 640x480 displays, but it is compatible with any resolution, and higher resolutions will utilize more detailed text and support for smaller background tiles.

<img src="https://github.com/Mips96/SuDokuL/blob/main/screenshots/screenshot-640-480_1.png?raw=true" width="320" height="240"/> <img src="https://github.com/Mips96/SuDokuL/blob/main/screenshots/screenshot-640-480_2.png?raw=true" width="320" height="240"/> <img src="https://github.com/Mips96/SuDokuL/blob/main/screenshots/screenshot-640-480_3.png?raw=true" width="320" height="240"/>

## How to Compile
(Note: To run any compiled version, you must have the `fonts`, `graphics`, `music`, and `sfx` folders which can be obtained from the latest release.)
#### PC
1. Download the latest SDL2 development libraries (Visual C++ versions):
- [SDL2](https://www.libsdl.org/download-2.0.php)
- [SDL2_image](https://www.libsdl.org/projects/SDL_image/)
- [SDL2_ttf](https://www.libsdl.org/projects/SDL_ttf/)
- [SDL2_mixer](https://www.libsdl.org/projects/SDL_mixer/)
2. Extract the above ZIP files into a folder called SDL2, which should be located in the SuDokuLVS2019 directory.
3. From there, use the Visual Studio project file from the repo with Visual Studio 2019.
#### Wii U
Install devkitPro, Wii U Toolkit, and SDL2 for Wii U, then build with CMake. I've included a `make_wii_u.sh` file for convenience once you have everything installed.
#### Vita
Install VitaSDK, then build with CMake. I've included a `make_vita.sh` file for convenience once you have everything installed.
#### Switch
Install devkitPro and switch-portlibs (which includes SDL2 for Switch), rename `Makefile_switch` to `Makefile`, then build with make.
#### Android
Install Android Studio, then follow [this tutorial](https://discourse.libsdl.org/t/building-sdl2-0-10-in-android-studio-3-4-2-in-windows-10/26481).

## Credits
Everything in this game is made by me except for the following assets:

### Music
- [Nuke of Anarchy - "Wonder Flow"](http://modarchive.org/index.php?request=view_by_moduleid&query=38132) (alternate version can be found [here](http://modarchive.org/index.php?request=view_by_moduleid&query=133262))
- [Okeanos - "Sudoku Padawan"](http://modarchive.org/index.php?request=view_by_moduleid&query=64812)
- [Nuke of Anarchy - "Electroquest"](http://modarchive.org/index.php?request=view_by_moduleid&query=41515)
- [Soundscape - "Main Menu"](http://modarchive.org/index.php?request=view_by_moduleid&query=49158)
- [Okeanos - "Insomnia"](http://modarchive.org/index.php?request=view_by_moduleid&query=45908)
- [Solon - "Ontario"](http://modarchive.org/index.php?request=view_by_moduleid&query=128908)
- [Noiseless - "Addiction"](http://modarchive.org/index.php?request=view_by_moduleid&query=32912)

### Font
Commodore Pixelized v1.2 by by Devin Cook

### Sound Effects
[Luke.RUSTLTD](https://opengameart.org/users/lukerustltd)

### Libraries / Tools
##### PC
- SDL2 2.0.16
- SDL2_image 2.0.5
- SDL2_ttf 2.0.15
- SDL2_mixer 2.0.4
- Visual Studio 2019
##### Wii U
- devkitPro
- Wii U Toolkit
- SDL2 for Wii U
- CMake
##### Vita
- VitaSDK
- CMake
##### Switch
- devkitpro
- SDL2 for Switch
- Make
##### Android
- Android Studio
