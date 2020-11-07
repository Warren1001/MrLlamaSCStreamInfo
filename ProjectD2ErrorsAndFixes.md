# How to Fix The "armor.bin" Error in Project Diablo 2.

### The reason this happens is because `ProjectDiablo.dll` fails to load. When this fails to load, Diablo 2 tries to automatically patch to 1.14d when the game loads. Since we are playing on a mod, we do not want this. Diablo 2 fails to update because its modded, which leaves the game in a corrupted state.
### The way to determine the reason why your `ProjectDiablo.dll` fails to load is as follows:

#### Check your `ProjectD2` folder inside your `Diablo II` folder. If `ProjectDiablo.dll is there`, then it's failing to load. If `ProjectDiablo.dll` is NOT there, that means your anti-virus is quarantining it. So far, Windows Defender, McAfee, and Bitdefender have also been known to quarantine the file.
#### If the file is there, you are likely missing the redistributables.
#### If your game worked previously but doesn't now and the file is missing, Windows Defender is catching something new they added which flags more than just `ProjectDiablo.dll` it seems.

## If `ProjectDiablo.dll` is there:

1. **99% of the time, you're missing the Redistributables needed.**
  - You can obtain them [here](https://support.microsoft.com/en-us/help/2977003/the-latest-supported-visual-c-downloads). You need the x86 and x64 links under 2015/2017/2019.
    - You can find the direct links [here](https://aka.ms/vs/16/release/vc_redist.x86.exe) and [here](https://aka.ms/vs/16/release/vc_redist.x64.exe).
      - Yes, you need both.
2. **On the chance that it is the 1%, try installing outside of the Program Files folder or running the launcher in Administrator.**

## If `ProjectDiablo.dll` is *NOT* there:

1. **If the game worked before, PD2 team released a patch that Windows Defender now flags. Disable Windows Defender real-time scanning.**
  1. Go to Start Menu > Settings > Update & Security > Windows Security.
  2. Click on Virus & threat protection.
  3. Under 'Protection history', find `ProjectDiablo.dll` and restore it and allow it.
    - You will have to do this every time ProjectD2 updates most likely.
2. **If the game working before doesn't apply to you, start with Step 1. anyway.**
3. **Check your own anti-virus for quarantines. Make sure you restore the `ProjectDiablo.dll` file similarly to how Step 1. describes.**
4. **You could just disable your anti-virus outright (real-time protection). This does not always work though which is why Step 3. is recommended.**
