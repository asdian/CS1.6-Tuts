# CS1.6-Singleplayer-Setup
## Guide to set up the game for testing mods.

> [!WARNING]
> This is a long step, make sure you followed carefully. A slight miss can lead to game crash/unstable.
> Don't rush it, take your time.

> [!CAUTION]
> This guide is only for single player mode (offline).

### Setting up the base game.

1. Download and install this specific version of CS1.6 [here](https://archive.org/details/counter-strike-1.6_202106). [Why?](#my-custom-anchor-point) Why? 
2. Download and install latest [MetahookSV](https://github.com/hzqst/MetaHookSv/releases/), choose blob version.
   - Copy `cstrike_hd`, `echoes`, `gearbox`, `platform`, `Metahook_blob.exe`, and `SDL2.dll` into your installed CS1.6 folder.
   - Open `svencoop` folder and copy everything into `cstrike` folder.
   - Back to your installed CS1.6 folder, rename the original `cstrike.exe` to something else if exist (as a backup).
   - Rename `Metahook_blob.exe` to `cstrike.exe`
   - Go to `cstrike\metahook\configs` folder, delete `plugins_svencoop.lst` and rename `plugins_goldsrc.lst` to `plugins.lst`.

3. Run and play your CS1.6 from `cstrike.exe`, play with bots, make sure eveything runs fine, no crash. If you're facing crashes and other, might be your installment/system issue.
4. Inside the game, press tilde "~" symbol on your keyboard, then type _`mh_pluginlist`_. If the output shows as shown on this image below, the Metahook is successfully installed.

![Screenshot of a comment on a GitHub issue showing an image, added in the Markdown, of an Octocat smiling and raising a tentacle.](https://i.imgur.com/77nEkmr.png)

5. Make sure the game is stable first before continuing. Play for few minutes or hours to make sure. Also try to change maps, change teams, change classes, etc.
6. Now download this Metahook plugin** from [here](https://www.mediafire.com/file/nh8ui1ht070k96u/MH_Precache.rar/file).
7. Copy the `.dll` file into `cstrike\metahook\plugins`.
8. Open `cstrike\metahook\configs\plugins.lst` with any text editor.
9. Write the `.dll` file name you just copied from the .rar to there and save it.
10. Open `cstrike\delta.lst` with any text editor.
11. Find every parameter that contains `modelindex`, `viewmodel`, `weaponmodel`, then change the value from `10` to `16`, and save it.
12. Repeat step 3-5. Make sure the new Metahook plugin is listed after you're typing _`mh_pluginlist`_.

<a name="my-custom-anchor-point"></a>
> [!NOTE]
> ### Why specific build 3266 is required?
> That Metahook plugin currently only works with build 3266. That's why it requires build 3266, which is quite hard to find nowadays. Thanks to archive.org I can find one that easy to download and install without crappy files (clean).
