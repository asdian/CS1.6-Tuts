# CS1.6-Singleplayer-Setup
## Guide to set up the game for testing mods.

> [!WARNING]
> This is a long step, make sure you followed carefully. A slight miss can lead to game crash/unstable.
> Don't rush it, take your time.

> [!CAUTION]
> This guide is only for single player mode (offline).

### Setting up the base game.

1. Download and install this specific version of CS1.6 [here](https://archive.org/details/counter-strike-1.6_202106). [Why?](#why-must-3266)
2. Download and install latest [MetahookSV](https://github.com/hzqst/MetaHookSv/releases/), choose blob version.
   - Copy `cstrike_hd`, `echoes`, `gearbox`, `platform`, `Metahook_blob.exe`, and `SDL2.dll` into your installed CS1.6 folder.
   - Open `svencoop` folder and copy everything into `cstrike` folder.
   - Back to your installed CS1.6 folder, rename the original `cstrike.exe` to something else if exist (as a backup).
   - Rename `Metahook_blob.exe` to `cstrike.exe`
   - Go to `cstrike\metahook\configs` folder, delete `plugins_svencoop.lst` and rename `plugins_goldsrc.lst` to `plugins.lst`.

3. Run and play your CS1.6 from `cstrike.exe`, play with bots, make sure eveything runs fine, no crash. If you're facing crashes and other, might be your installment/system issue.
4. Inside the game, press tilde "~" symbol on your keyboard, then type _`mh_pluginlist`_. If the output shows as shown on this image below, the Metahook is successfully installed.

![List of installed Metahook Plugins.](https://i.imgur.com/77nEkmr.png)

5. Make sure the game is stable first before continuing. Play for few minutes or hours to make sure. Also try to change maps, change teams, change classes, etc.
6. Now download this Metahook plugin) from [here](https://www.mediafire.com/file/nh8ui1ht070k96u/MH_Precache.rar/file).
7. Copy the `.dll` file into `cstrike\metahook\plugins`.
8. Open `cstrike\metahook\configs\plugins.lst` with any text editor.
9. Write the `.dll` file name you just copied from the .rar to there and save it.
10. Open `cstrike\delta.lst` with any text editor.
11. Find every parameter that contains `modelindex`, `viewmodel`, `weaponmodel`, then change the value from `10` to `16`, and save it.
12. Repeat step 3-5. Make sure the new Metahook plugin is listed after you're typing _`mh_pluginlist`_.

<a name="why-must-3266"></a>
> [!NOTE]
> #### Why specific build 3266 is required?
> The Metahook plugin we're going to use currently only works with build 3266. That's why it requires build 3266, which is quite hard to find nowadays. Thanks to archive.org I can find one that easy to download and install without crappy files (clean).
---
### Installing AMX Mod X
Now, on to installation of AMX Mod X.

1. Download [this](https://github.com/asdian/CS1.6-Singleplayer-Setup/blob/main/AMX%20Mod%20X%20Starter%20Pack.rar) package. This package includes reGameDLL - ReAPI, SYPB (disabled by default), Metamod-P 1.21p38, Printcenter fix, and AMXModX 1.10.0.5467.
2. Extract all the files into _`cstrike`_ folder.
3. Start and run the game.
4. Inside the game, press tilde "~" symbol on your keyboard, then type _`meta list`_ and _`amxx plugins`_. If the output shows as shown on this image below or similar (outputs something, not an unknown command), the package is successfully installed.

![Metamod installed plugin list.](https://i.imgur.com/1KR8It3.png)

5. Make sure the game is stable first before continuing. Play for few minutes or hours to make sure. Also try to change maps, change teams, change classes, etc.

> Congratulations!
> -
> Now you have a working base game to start modding. You don't have to worry with 512 precache limit again thanks to that Metahook plugin. It increases the precache to around 1024.
---

### Installing Metadrawer [Optional]
Optionally, you can install Metadrawer, a Metahook plugin to load images for UI enhancements into the game.

1. Download from [here](https://gamebanana.com/mods/39420).
2. Place `binkw32.dll` and `cstrike` folder into your installed CS1.6 folder.
3. Open `cstrike\metahook\configs\plugins.lst` with any text editor.
4. Write that .dll file name you just copied and save it.
5. Go to cstrike folder, create a file named _`userconfig.cfg`_ (a must, can't use random naming). Not a .txt file, make sure you have done that properly.
6. Write this command: _`md_newmenu "0"`_ inside and save it.
7. Go to `cstrike\addons\amxmodx\configs` folder, open `modules.ini` with any text editor, write _`metadrawer`_ in it and save.
8. Repeat from step 3-5 of this [guide.](https://github.com/asdian/CS1.6-Singleplayer-Setup/blob/main/README.md#setting-up-the-base-game).

> [!TIP]
> Alternatively, you can use [MetaCSU](https://csumods.blogspot.com/2023/06/cs16-plugin-metahook-mhmetacsu-v02.html) which provides around the same functionality. But don't mix them unless you're know what you're doing.

> That's all, you have successfully installed a CS1.6 complete with its addons for modding.
> -
