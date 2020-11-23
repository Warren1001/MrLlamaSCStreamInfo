##### Note: With continuing updates, prior knowledge to fixes are being lost and new ways have to be discovered. As such, it is quite likely that some of these fixes are outdated.

##### Note: This list is not exhaustive and there are definitely unreported fixes to some of the complex issues. If none of these work, post in the [PD2 Discord #troubleshoot](https://discord.gg/MgbKSmm6Mt) chat.

| [****Issues****](https://github.com/Warren1001/MrLlamaSCStreamInfo/blob/master/ProjectD2ErrorsAndFixes.md) |
| :-: |
| [Armor.bin](https://github.com/Warren1001/MrLlamaSCStreamInfo/blob/master/ProjectD2ErrorsAndFixes.md#how-to-fix-armorbin--missing-or-wrong-gateway--patch-failed-or-not-needed--missing-resolution--inventory-cut-off-error) |
| [d2data.mpq is corrupt](https://github.com/Warren1001/MrLlamaSCStreamInfo/blob/master/ProjectD2ErrorsAndFixes.md#how-to-fix-d2datampq-is-corrupt-error) |
| [Missing or Wrong Gateway](https://github.com/Warren1001/MrLlamaSCStreamInfo/blob/master/ProjectD2ErrorsAndFixes.md#how-to-fix-armorbin--missing-or-wrong-gateway--patch-failed-or-not-needed--missing-resolution--inventory-cut-off-error) |
| [Patch Failed or Not Needed](https://github.com/Warren1001/MrLlamaSCStreamInfo/blob/master/ProjectD2ErrorsAndFixes.md#how-to-fix-armorbin--missing-or-wrong-gateway--patch-failed-or-not-needed--missing-resolution--inventory-cut-off-error) |
| [Missing Resolution](https://github.com/Warren1001/MrLlamaSCStreamInfo/blob/master/ProjectD2ErrorsAndFixes.md#how-to-fix-armorbin--missing-or-wrong-gateway--patch-failed-or-not-needed--missing-resolution--inventory-cut-off-error) |
| [Inventory Cut Off](https://github.com/Warren1001/MrLlamaSCStreamInfo/blob/master/ProjectD2ErrorsAndFixes.md#how-to-fix-armorbin--missing-or-wrong-gateway--patch-failed-or-not-needed--missing-resolution--inventory-cut-off-error) |
| [c0000005](https://github.com/Warren1001/MrLlamaSCStreamInfo/blob/master/ProjectD2ErrorsAndFixes.md#how-to-fix-c0000005-error) |
| [Halt](https://github.com/Warren1001/MrLlamaSCStreamInfo/blob/master/ProjectD2ErrorsAndFixes.md#how-to-fix-halt-error) |
| [VCRUNTIME140_1.dll](https://github.com/Warren1001/MrLlamaSCStreamInfo/blob/master/ProjectD2ErrorsAndFixes.md#how-to-fix-vcruntime140_1dll-error) |
| [Play on Launcher Does Nothing](https://github.com/Warren1001/MrLlamaSCStreamInfo/blob/master/ProjectD2ErrorsAndFixes.md#how-to-fix-play-on-launcher-does-nothing-error) |
| [Silent Crash](https://github.com/Warren1001/MrLlamaSCStreamInfo/blob/master/ProjectD2ErrorsAndFixes.md#how-to-fix-silent-crash-error) |
| [Direct3D Error](https://github.com/Warren1001/MrLlamaSCStreamInfo/blob/master/ProjectD2ErrorsAndFixes.md#how-to-fix-a-critical-error-has-occured-while-initializing-direct3d-error) |
| [Bugged Launcher](https://github.com/Warren1001/MrLlamaSCStreamInfo/blob/master/ProjectD2ErrorsAndFixes.md#how-to-fix-bugged-launcher-with-white-background-error) |
| [Unable to Connect to Battle.net](https://github.com/Warren1001/MrLlamaSCStreamInfo/blob/master/ProjectD2ErrorsAndFixes.md#how-to-fix-unable-to-connect-to-battlenet-error) |
| [Failed to Join Game](https://github.com/Warren1001/MrLlamaSCStreamInfo/blob/master/ProjectD2ErrorsAndFixes.md#how-to-fix-failed-to-join-game-error) |
| [C000000D (Error on Close)](https://github.com/Warren1001/MrLlamaSCStreamInfo/blob/master/ProjectD2ErrorsAndFixes.md#how-to-fix-c000000d-glide3xdll--invalid-parameter-error) |
| [Cannot Create an Account](https://github.com/Warren1001/MrLlamaSCStreamInfo/blob/master/ProjectD2ErrorsAndFixes.md#how-to-fix-cannot-create-an-account-error) |
| [Wrong Password](https://github.com/Warren1001/MrLlamaSCStreamInfo/blob/master/ProjectD2ErrorsAndFixes.md#how-to-fix-wrong-password-error) |
| [CD-ROM](https://github.com/Warren1001/MrLlamaSCStreamInfo/blob/master/ProjectD2ErrorsAndFixes.md#how-to-fix-cd-rom-error) |

# How to Fix Armor.bin / Missing or Wrong Gateway / Patch Failed or Not Needed / Missing Resolution / Inventory Cut Off Error

### The fixes here are for any error which comes from "PD2" being missing at the bottom left of the D2 main menu after you launch PD2. If your main menu only says "1.13" and not "PD2 1.13" then the two fixes here apply to you.

### The reason this happens is because `ProjectDiablo.dll` fails to load. When this fails to load, Diablo 2 tries to automatically patch to 1.14d when the game loads. Since we are playing on a mod, we do not want this. Diablo 2 fails to update because its modded, which leaves the game in a corrupted state.
### The way to determine the reason why your `ProjectDiablo.dll` fails to load is as follows:

#### Check your `ProjectD2` folder inside your `Diablo II` folder. If `ProjectDiablo.dll` is there, then it's failing to load. If `ProjectDiablo.dll` is NOT there, that means your anti-virus is quarantining it. So far, Windows Defender, McAfee, and Bitdefender have also been known to quarantine the file.
#### If the file is there, you are likely missing the redistributables.
#### If your game worked previously but doesn't now and the file is missing, Windows Defender is catching something new they added which flags more than just `ProjectDiablo.dll` it seems.

## If `ProjectDiablo.dll` is there:

1. **You are missing the [x86 Redistributable](https://aka.ms/vs/16/release/vc_redist.x86.exe) needed. Install the Redistributable and restart your PC.**
2. **Try installing outside of the Program Files folder or running the launcher in Administrator.**

## If `ProjectDiablo.dll` is *NOT* there:

1. **If the game worked before, PD2 team released a patch that Windows Defender now flags. Disable Windows Defender real-time scanning.**
	1. Go to Start Menu > Settings > Update & Security > Windows Security.
	2. Click on Virus & threat protection.
	3. Under 'Protection history', find `ProjectDiablo.dll` and restore it and allow it.
		- You will have to do this every time ProjectD2 updates most likely.
	4. The BEST fix is to add your Diablo 2 folder to the Exclusions folder for Windows Defender after performing Step 3. This will ensure you do not have to do this fix every time PD2 updates.
2. **If the game working before doesn't apply to you, start with Step 1. anyway.**
3. **Check your own anti-virus for quarantines. Make sure you restore the `ProjectDiablo.dll` file similarly to how Step 1. describes.**
	- For McAfee, the only way is to disable real-time scanning. You can do this by right-clicking the McAfee icon in your Windows taskbar, press the top option to open the app, click `PC Security` or whatever at the top, click `Real-time scanning` or whatever on the left, then click `Turn off` on the right to disable it. You will probably need to keep McAfee disabled while playing PD2. Enjoy the overzealous anti-virus.
4. **You could just disable your anti-virus outright (real-time protection). This does not always work though which is why Step 3. is recommended.**

# How to Fix "d2data.mpq is corrupt" Error

### The reason this happens is because downgrading from 1.14 is finnicky and the MPQFixer doesn't work for all people. The solution is to go to the source and get the original MPQs from the older installers. Install Diablo 2 using the provided legacy installer links and install PD2 into the new install.
- [Google Drive](https://drive.google.com/file/d/0BwtmRlAuN2x8X2FoWmhoR2pWQ2s/view)
- [OneDrive](https://onedrive.live.com/redir?resid=C9512C8BBA34920C!1795&authkey=!AHKYNghIssoWWVs&ithint=file%2czip)
- [Mediafire](http://www.mediafire.com/file/51r3c5s6hezsruz/DiabloII_113c_Installer.zip/file)
- [Torrent](https://cdn.discordapp.com/attachments/157962768534863872/160784109642186753/DiabloII_113c_Installer.zip.torrent)
- [Mega.nz](https://mega.nz/#!e9thyD6A!ExGJuZUtvRJ2c8DrxSL0ihCouh-ARbdVxODXIqVt3dc)

# How to Fix c0000005 Error

## Context: You press `Play` on the Launcher and you receive the error.

### Possibility 1: Missing x86 2015/2017/2019 Redistributable.

- Install [this](https://aka.ms/vs/16/release/vc_redist.x86.exe). Then restart your PC.

### Possibility 2: Your PC just needs a full restart. Restart it.

### Possibility 3: You need to update your Vanilla client to 1.14d and then restart your PC afterwards.

#### Not sure what triggers this bug, but patching the Vanilla client from 1.14b to 1.14d reportedly fixes this issue for some. PC restart required to see if fix worked.

### Possibility 4: Compatibility

#### Sometimes Diablo 2 just isn't nice, especially if you're installing into a Diablo 2 version that is lower than 1.14.

1. For `Game.exe` in the `ProjectD2` folder, go to its properties and set the compatibility mode to `Windows XP SP2` or `Windows XP SP3`.
2. For both `Game.exe` and `PD2Launcher.exe` in the `ProjectD2` folder, go to their properties and set both of them to `Run as admininstrator`.

### Possibility 5: DEP

#### I don't know the technicalities behind it, but some people need to perform the "DEP" fix.

1. **Go to your Start Menu and simply start typing `Control Panel` and click it.**
2. **Click `System`.**
3. **Click `Advanced system settings` on the left menu.**
4. **Under the `Advanced` tab, under the `Performance` section, click `Settings`.**
5. **Click the `Data Execution Prevention` (DEP) tab.**
6. **Click `Turn on DEP for essential Windows programs and services only`.**
7. **Press `Apply` and `OK`.**
8. **Restart your PC.**

### Possibility 6: Cinematics Bug

#### PD2 reintroduced the old Cinematics bug where if your game client has no sound (usually through `-ns`), you crash on cinematics, including the intro cinematics.

- **If you do not have sound, get sound. If you do not want sound, simply turn down the audio in-game. You can mute the main menu with `Ctrl + M`.**

### Possibility 7: Bad Diablo II Install

- **Try launching Vanilla (unmodded) Diablo 2. If you get the error there, do a fresh re-install. If you don't, click on Battle.net to ensure you have the latest version. Then try launching PD2 again.**

### Possibility 8: Hovered Over Bottom Right of Stash

- Theres a critical bug where mousing over the bottom two slots? of the bottom-right stash forces a crash. No known fix. Just keep your cursor away from bottom right of stash.

### Possibility 9: Non-English Diablo 2 Install

#### This crash happens randomly when interacting with certain items, skills, and monsters.

- Diablo 2 must be installed in English. Any other language will cause completely random crashes with items, skills, and monsters.
	- Link to English [Classic](https://www.blizzard.com/download/confirmation?platform=windows&locale=en_US&product=d2) and [LOD](https://www.blizzard.com/download/confirmation?platform=windows&locale=en_US&product=d2lod) installers. May need to sign in.
- If English Diablo II, re-install.

### Possibility 10: Some Other Missing Dependency

#### I have yet to figure out what makes this bug. Typically, it is either some form of corruption or missing a required library that is not listed anywhere.

1. **Try repairing the launcher by running the PD2 installer again and repairing.**
2. **Try making sure your Windows is up to date with everything a computer generally needs.**
	1. [.NET Framework 3.5](https://docs.microsoft.com/en-us/dotnet/framework/install/dotnet-35-windows-10) and [.NET Framework 4.8](https://dotnet.microsoft.com/download/dotnet-framework/net48)
	2. [As many Redistributables as you can](https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads). Both x86 and x64 versions.
	3. Make sure Windows is up-to-date.
	4. Update your drivers, especially your audio and video card drivers.

## Context: You travel to a new Act in-game.

- Almost always because of -ns. See [here](https://github.com/Warren1001/MrLlamaSCStreamInfo/blob/master/ProjectD2ErrorsAndFixes.md#possibility-6-cinematics-bug).

## Context: Hovering over item or skill descriptions.

- You have a non-English Diablo II installation. Must be English Diablo II.
- If English Diablo II, re-install.

## Context: Killed Ventar the Unholy in Baal's fourth wave.

- I have yet to figure out why this happens. Other fixes have not seemed to help this issue. Usually not related to language or locale. Perhaps an issue with non-English Windows? Issue not solved, sorry.

# How to Fix Halt Error

## Context: Character creates or joins a game.

- If you are able to create a new character and join a game but cannot join a game with an existing character because your game crashes with a Halt error, your character may have been corrupted somehow. This is not proven, waiting may simply fix it. I would be worried though, especially if it's online.
- If creating a new character still gives you a Halt error, then you likely have a bad install.
	- Be sure your game is a completely fresh install. You cannot copy and paste. You cannot re-use files from a previously modded install. Install Diablo II and then LOD and then PD2 all into the same folder.

# How to Fix `VCRUNTIME140_1.DLL` Error

- You are missing the Redistributables needed. You need both [x86](https://aka.ms/vs/16/release/vc_redist.x86.exe) and [x64](https://aka.ms/vs/16/release/vc_redist.x64.exe). Run them.

# How to Fix `Play` on Launcher Does Nothing Error

### Possibility 1: The launcher is checking the wrong spot for the game and so it fails to launch.
1. Press the Windows button and R at the same time (launch `Run.exe`).
2. Type regedit and press `OK`.
3. Navigate to `HKEY_CURRENT_USER\SOFTWARE\Blizzard Entertainment\Diablo II`.
4. Double cick on the key `InstallPath`.
5. Set the `Value data` to your D2 folder (not your PD2 folder).
	- If your path ends in `...\ProjectD2`, delete that part.

# How to Fix Silent Crash Error

## Context: Interacting with items, skills, or monsters.

- Diablo 2 must be installed in English. Any other language will cause completely random crashes with items, skills, and monsters.
	- Link to English [Classic](https://www.blizzard.com/download/confirmation?platform=windows&locale=en_US&product=d2) and [LOD](https://www.blizzard.com/download/confirmation?platform=windows&locale=en_US&product=d2lod) installers. May need to sign in.
- If English Diablo II, re-install.
- Hovering over the bottom right of the stash is a known crash bug. No fix. Avoid moving your cursor to the bottom right of the stash.

# How to Fix `A critical error has occured while initializing Direct3D` Error

#### This error is a generic error when Diablo 2 tries to load in fullscreen which does not work for many people without special settings.

- In the `Options` menu on the Launcher, enable `Windowed Mode (-w)`.
- If you want fullscreen, disable `Windowed Mode (-w)` and follow these steps:
	1. Go to your `ProjectD2` folder and open `ddraw.ini`.
	2. Set `width` and `height` at the top to your desktop resolution.
	3. Set `fullscreen` to `false`.
	4. Set `windowed` to `true`.
	5. If applicable to you, set `maintas` to `false` to avoid the black bars.

# How to Fix Bugged Launcher With White Background Error

- Run the Launcher as Administrator.

# How to Fix `Unable to Connect to Battle.net` Error

## Context: Main menu has the 5 characters in the background

1. Press the Windows button and R at the same time (launch `Run.exe`).
2. Type `regedit` and press `OK`.
3. Navigate to `HKEY_CURRENT_USER\SOFTWARE\Blizzard Entertainment\Diablo II`.
4. Double click on the key `InstallPath`.
5. Set the `Value data` to your D2 folder (not your PD2 folder).
	- If your path ends in `...\ProjectD2`, delete that part.

# How to Fix `Failed to Join Game` Error

- The game server you were in crashed. The realm server still thinks your character is in-game because the game server did not report you leaving the game since it crashed. Therefore, the realm doesn't let your character into another game. The only fix is to wait for the game server to restart and let your character out of the void. Patience. It could be 5 minutes or 24 hours.

# How to Fix C000000D (glide3x.dll & Invalid Parameter) Error

#### This error happens upon closing the game.

1. Download [IndirectSound](https://www.indirectsound.com/downloads/IndirectSound_0_20.zip).
2. Copy `dsound.dll` and `dsound.ini` to your `ProjectD2` folder.
3. Ensure you have the [DX9 Runtimes](https://www.microsoft.com/en-us/download/confirmation.aspx?id=35). Install it.
4. In your `ProjectD2` folder, set `Game.exe` and `Diablo II.exe` to run in Windows 7 Compatibility mode.
5. Restart PC.

- Optional feature: Edit `dsound.ini` and change `eax2` to `true`. This will enable the ability to toggle `3D Sound and Environmental Effects` in the D2 sound menu.

#### Fix found by several [Reddit users](https://www.reddit.com/r/ProjectDiablo2/comments/js8neb/glide3xdll_not_working/).

# How to Fix `Cannot Create an Account` Error

#### No matter what random string of text you try, all accounts cannot be made.

- This is because you cannot use the D2 client to make an account. You need to [make an account on the website](https://www.projectdiablo2.com/authentication/login). The Game Account you provide is your in-game account name and password. If you aren't sure if you are typing it correctly, [check here](https://www.projectdiablo2.com/pd2accountmanagement). This will tell you your account but not your password. If you lost your password, as of now you are out of luck. Simply make a new account until they implement password resetting.

# How to Fix `Wrong Password` Error

#### This is a manifest of other issues.

### Possibility 1: [Try the Armor.bin fix](https://github.com/Warren1001/MrLlamaSCStreamInfo/blob/master/ProjectD2ErrorsAndFixes.md#how-to-fix-armorbin--missing-or-wrong-gateway--patch-failed-or-not-needed--missing-resolution--inventory-cut-off-error)

### Possibility 2: [Try the Cannot Create an Account fix](https://github.com/Warren1001/MrLlamaSCStreamInfo/blob/master/ProjectD2ErrorsAndFixes.md#how-to-fix-cannot-create-an-account-error)

# How to Fix CD-ROM Error

- You need [VC 2010 SP1 x86](https://www.microsoft.com/en-US/download/confirmation.aspx?id=8328). Run it then restart your PC.
