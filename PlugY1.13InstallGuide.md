# How to install PlugY for Diablo 2 version 1.13d

#### Because this is for an outdated version of Diablo 2, if you also want to play Battle.net, you will need two separate installations.

#### There is [a video guide](https://www.youtube.com/watch?v=czO1LYKytG8) you can use instead of text guide, but people have reported issues with some of the steps he has shown in the guide. It is also a little over-complicated.


1. **You will need to obtain a legacy online installer.**
	- The reason is because you cannot downgrade from 1.14, as it has undergone too many changes.
	1. *You can find links to the legacy online installer [here](https://www.reddit.com/r/pathofdiablo/comments/4b48oz/how_to_download_and_install_version_113/d160fdh/) or [here](https://www.reddit.com/r/slashdiablo/wiki/index/setup)*.
		- Here are the links to the hosting sites linked at the above links:
			- [Mega.nz](https://mega.nz/#!e9thyD6A!ExGJuZUtvRJ2c8DrxSL0ihCouh-ARbdVxODXIqVt3dc)
			- [Google Drive](https://drive.google.com/file/d/0BwtmRlAuN2x8X2FoWmhoR2pWQ2s/view)
			- [OneDrive](https://onedrive.live.com/redir?resid=C9512C8BBA34920C!1795&authkey=!AHKYNghIssoWWVs&ithint=file%2czip)
			- [Mediafire](http://www.mediafire.com/file/51r3c5s6hezsruz/DiabloII_113c_Installer.zip/file)
			- [Torrent](https://cdn.discordapp.com/attachments/157962768534863872/160784109642186753/DiabloII_113c_Installer.zip.torrent)
2. **Install Diablo 2 using the legacy online installer.**
	- In the event that loading up the installer says "Play Diablo 2" instead of "Install Diablo 2", you will have to rename your current Diablo 2 folder.
		- Find your current Diablo 2 folder and either delete it if you do not plan to use it at all or rename the folder to something else so that you can install Diablo 2 again. Then restart the installer and install as normal.
3. **Your Diablo 2 is now at 1.12a. However, we want to be at 1.13d, so we need to patch Diablo 2 to 1.13d.**
	1. To do this, we will download the standalone patch from Blizzard's website, which you can find [here](http://ftp.blizzard.com/pub/diablo2exp/patches/PC/LODPatch_113d.exe).
	2. To ensure everything goes smoothly, go to your Diablo 2 folder and apply the following settings to both `Diablo II.exe` and `Game.exe`:
		1. Right click the executable and go to `Properties`.
		2. Go to the `Compatibility` tab.
		3. Check the box that says `Run this program in compatibility mode for:` and change the compatibility mode to `Windows XP (Service Pack 2)`.
		4. Check the box that says `Run this program as an administrator`.
		- Now these programs should work properly and not cause issues when we update using the standalone patch.
4. **Run the `LODPatch_113d.exe` program in administrator mode.**
	- This will update your Diablo 2. HOWEVER, Diablo 2 will try to start immediately. If it loads successfully, it will try to connect to Battle.net and get the latest patch. Obviously, we do not want this! *If Diablo 2 begins loading, spam `Esc` until it closes!*
	- Sometimes, Diablo 2 will not load properly, which is okay. If you suspect the Diablo 2 application hung, go to your Task Manager and force `Game.exe` to close. Or restart your computer.
5. **Now we are at the proper Diablo 2 version, so we can begin installing PlugY. You can obtain [PlugY v14.02 here](http://plugy.free.fr/PlugY_The_Survival_Kit_v14.02.zip).**
	- You can view the official PlugY site [here](http://plugy.free.fr/). We will be using the `Zip version` as the installer version tends to create more issues than it solves.
6. **Open the `PlugY_The_Survival_Kit_v14.02.zip` file.**
7. **Drag and all the files from this file into the Diablo 2 folder.**
	- We do not care about the any of the `.txt`, the `PatchD2File.exe`, or the `RestoreD2File.exe` files. You can get rid of them if you wish.
8. **Perform the settings we did in Step `3.ii` to `PlugY.exe` in your Diablo 2 folder.**
9. **Right click `PlugY.exe` and press `Send to > Desktop (create shortcut)`.**
10. **Go to your Desktop, right click the new shortcut, go to `Properties` and click on the `Shortcut` tab.**
11. **In the `Target:` box, add `-w` to the end.**
	- For most people, the `Target:` box should read `"C:\Program Files (x86)\Diablo II\PlugY.exe" -w`.
		- The `"` on either side of the path are required to add `-w` to the end.
12. **Launch PlugY using the shortcut on your desktop.**

##### Enjoy! If you run into any issues (which is likely, as there are several things that can cause the PlugY installation to go astray), @mention or DM Warren1001 on [MrLlama's Discord](https://discord.gg/BePVw9e).	
