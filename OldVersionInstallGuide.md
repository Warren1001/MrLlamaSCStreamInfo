# How to Install and Play an Older Version of Diablo 2


###### It's a lot of steps, but most of them are very quick, such as clicking buttons or opening folders.

##### Something worth nothing, while these files do not directly change the game, logging into Battle.net with these files in your Diablo 2 folder may or may not get you banned. Caution should be exercised. It is recommended that you have a separate installation for playing on Battle.net. A simple copy and paste of your current Diablo 2 folder should be enough to install this version-switcher into Diablo 2.


1. **Install Diablo 2 as normal.**
	- The version does not matter. It can be 1.12 or 1.13 or 1.14d.
	- It should be unmodded though.
2. **[Download Cactus](https://themovingcaravan.com/diablo/Cactus.7z) (~27 MB).**
	- Cactus is a version-switcher. You can find more information about Cactus [here](https://codeberg.org/fearedbliss/Cactus).
3. **Open `Cactus.7z`.**
4. **Navigate to and open the `1. Files` folder.**
5. **Take every file in this folder and drag and drop it into your Diablo 2 folder.**
6. **Navigate to and open the `3. Other` folder.**
7. **Take every file in this folder and drag and drop it into your Diablo 2 folder.**
8. **Run the two 'Other' exes, `MSVC_..` and `NET_Framework_..`.**
9. **Open the `MpqFixer` folder now in your Diablo 2 folder.**
10. **Right click `FIX_MPQS_RUN_AS_ADMIN.bat` and press *Run as administrator*.**
	- This fixes your MPQs to work with older versions of Diablo 2.
11. **Navigate back to your Diablo 2 folder.**
12. **Open `Cactus.exe`.**
	- This will be the program you use to launch older versions of Diablo 2, so consider making a shortcut of it if you intend to use it frequently.
13. **Press `Add` at the bottom left.**
	- This adds a new profile to the program which will be used to launch the older version of Diablo 2.
14. **For `Platform`, input the version you wish to play.**
	- The available platforms to choose from are `1.00`, `1.01`, `1.02`, `1.03`, `1.04b`, `1.04c`, `1.05`, `1.05b`, `1.06`, `1.06b`, `1.07` (first LoD version), `1.08`, `1.09` (original Runewords introduced), `1.09b`, `1.09d`, `1.10` (op Runewords introduced), `1.10b (Beta 1)`, `1.10s (Beta 2)`, `1.11`, `1.11b`, `1.12a` (Den Respecs introduced), `1.13a (Beta)` (Tokens introduced), `1.13c`, `1.13d`, `1.14a`, `1.14b`, `1.14c`, and `1.14d`.
	- If I wanted to play v1.00, I would simply write `1.00` into the `Platform` dialog box.
	- If you make a typo with the `Platform` and try to edit the box, it will tell you that the `Platform` already exists. Delete the profile and make it from scratch again. It will let you specify the right `Platform` this time.
15. **For `Path`, this will be the path to the executable to launch Diablo 2.**
	- This path is relative to where the Cactus program is, so if you installed it inside the Diablo II folder (which you should have), most people will simply write `Game.exe` here. If you have another exe to use, like PlugY or something else, then you would use that exe instead.
16. **For `Flags`, this is where you input your startup arguments.**
	- Flags consist of `-w`, `-ns`, `-3dfx`, and so forth.
	- Choose what you want. Most users will just want `-w`.
17. **The `Expansion` checkbox should be *un*checked if:**
	1. You do not own the expansion.
	2. You want to play without LoD features (Classic Diablo 2).
	3. You are playing a version less than `1.07`. All versions from `1.00` to `1.06b` are Classic only.
18. **Press `Add` to finish creating the profile.**
19. **Click on your newly created profile and press `Launch`.**
	- This will launch Diablo 2 with the profile you just created. This is how you will launch the older version of Diablo 2 every time.


##### Enjoy! If you have issues, @mention or DM Warren1001 on [MrLlama's Discord](https://discord.gg/mrllamasc). If you are intending to play v1.00, you can check a list of differences [here](https://github.com/Warren1001/MrLlamaSCStreamInfo/blob/master/D2v1.0Info.md).
