# Into AMX Mod X Scripting
Below is tutorials of setting up workspace for AMX Mod X scripting.

> [!NOTE]
> [About AMX Mod X](https://www.amxmodx.org/about.php)
> 
> A RAW file (uncompiled) before `.amxx` is in `.sma` format. We need a software to properly create or modify and then compiling it into an `.amxx`.

### Setting up working space
1. Download the AMX Mod X scripting package [here](https://www.amxmodx.org/downloads-new.php) (or [here](https://www.amxmodx.org/downloads-new.php?branch=master) for the newest available). **Choose `base` package.
2. Create and place the `scripting` folder or contents into your project folder. Here's the example:
![AMX Mod X Minimal Files](https://github.com/asdian/CS1.6-Tuts/blob/main/Pics/AMXX-Scripting/AMXStudio/Screenshot_1.png)
> [!TIP]
> I recommend to not put the files inside the CS1.6 installation folder, in case when you need to clean install the game it saves you the hassle from doing backups.

#### Now, let's set up our scripting software. There are two softwares that I use for AMX Mod X scripting.

> ### Easy Way / [Advanced Way](https://github.com/asdian/CS1.6-Tuts/blob/main/AMXModX-Scripts.md#the-advanced-way-is-using-visual-studio-code)
---
> #### The easy way is using AMX Mod X Studio. A lightweight software for AMX Mod X scripting.

3. Download the AMX Mod X Studio from [here](https://sourceforge.net/projects/amxmodx/files/AMX%20Mod%20X%20Studio/1.4.3%20final/AMXX_Studio_1.4.3_final.zip/download). It's a portable software, you just have to extract it.
4. Place it somewhere. `Example: D:/Projects/CS1.6/AMX Studio/(here)`.
5. Open `AMXX_Studio.exe`.
6. Go to `Tools` -> `Settings`.
![AMXX Studio 1](https://github.com/asdian/CS1.6-Tuts/blob/main/Pics/AMXX-Scripting/AMXStudio/Screenshot_2.png)
7. Go to `Compiler` menu, and apply the corresponding `amxxpc.exe` and `compile.exe` from your directory / the step 2.
![AMXX Studio 2](https://github.com/asdian/CS1.6-Tuts/blob/main/Pics/AMXX-Scripting/AMXStudio/Screenshot_3.png)
8. Press `OK` and you're good to go. Easy right?
---
> #### The advanced way is using Visual Studio Code.
> A modern software for advanced AMX Mod X scripting.

3. Download and install [VSCode](https://code.visualstudio.com/)
4. Go to `Extensions` and install `AMXXPawn Language` by `KliPPy`.
![AMXX VScode1](https://github.com/asdian/CS1.6-Tuts/blob/main/Pics/AMXX-Scripting/VSCode/Screenshot_1.png)
5. After installing it, go to `Manage` then `Settings`.
![AMXX VSCode2](https://github.com/asdian/CS1.6-Tuts/blob/main/Pics/AMXX-Scripting/VSCode/Screenshot_2.png)
6. Click `Edit in settings.json` (doesn't matter which one).
![AMXX VSCode3](https://github.com/asdian/CS1.6-Tuts/blob/main/Pics/AMXX-Scripting/VSCode/Screenshot_3.png)
7. Edit your working folders and files as needed.
![AMXX VSCode4](https://github.com/asdian/CS1.6-Tuts/blob/main/Pics/AMXX-Scripting/VSCode/Screenshot_4.png)
** The syntax must be correct to be able to find your files.
8. Then save it or press `CTRL + S` and you're good to go.

## What are the difference?
So far, from what I can tell only few differences that's significantly affects experience.

For easy and short scripts, AMX Mod X Studio is <ins>better</ins> because it can show dropdown of function suggestions from the loaded include (`.inc`) files, while VSCode **only** shows suggestion from what are inside the currently opened script file. However, when your scripts has 1500+ line long, VSCode is better because AMX Mod X Studio will lag.

# Where to start scripting?
Refer to this [link](https://forums.alliedmods.net/showthread.php?t=172936). There's already a ton of AMX Mod X scripting Tutorials, Guides, Snippets, and References. Good luck!

