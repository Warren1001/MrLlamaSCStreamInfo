# Common Issues With Diablo 2 and How to Fix Them

###### Note: If you have a Github account, you can edit this file by submitting a PR in the case more information can be provided or information given is inaccurate.

### `Checking versions...` or `Disconnected from Battle.net, please reconnect` or `Battle.net is not responding, please try reconnecting in a few minutes`

1. The most common reason this happens is because you logged onto the realm with a proxy, VPN, or business-class internet. If you know you did, the only way the ban can be bypassed is change your IP (if you have a dynamic IP) (unless you have business-class internet) and get new CD keys.
	- Duration of two weeks.
	- Proxies, VPNs, and business-class internet are banned to combat MASS botting. Mass botting is different from a person running their own 1-4 public bot(s).
	- Sometimes Blizzard or your ISP will mistakenly label you as business-class. Contact Blizzard to see if you were banned for having business-class internet. If so, contact your ISP and see if you were mistakenly labeled as business-class. If you were not, then unfortunately you are out of luck, as Blizzard will not do anything to fix it.
2. Windows is zealous with its protection of modifying applications inside its folders and Blizzard's anti-cheat is not being allowed to act properly, causing Blizzard to think you are tampering with their anti-cheat and denying you entry. Re-install Diablo 2 outside of any Windows folder, such as `C:\Games\Diablo II\`.
3. The game may have failed to update properly. The version on the main menu should read 1.14d. If it does not, you need to re-install. If it does, you may want to consider re-installing anyway. This time, try [using the standalone patch](http://ftp.blizzard.com/pub/diablo2exp/patches/PC/LODPatch_114d.exe) to update Diablo 2, instead of doing it through the client. If this still does not help, try re-installing outside of any Windows folders (see #2), as Windows may be preventing the game from updating correctly.
4. You have a zealous anti-virus that interferes with Blizzard's anti-cheat. Blizzard's anti-cheat is a bit shady so a zealous anti-virus might try quarantining the files used to prevent hacking online. As such, Blizzard thinks you are tampering with their anti-cheat and denies you entry. Disabling the anti-virus (or adding the Diablo 2 folder to a list to not be monitored) should fix this.
5. Your ISP struggles to resolves the names of the realm IPs OR one of the realm servers that you are trying to connect to is down. This issue is unlikely and so far has happened with one reset with a few ISPs in Europe (which could suggest a realm server was not working correctly). Anyhow, if you've tried all the other suggestions, then you could [try this fix]().

### `Unhandled Exception (c000005)`

1. 99% of the time this issue occurs is from a corrupted installation. Re-install the game. It is recommended to install Diablo 2 outside of any Windows folders, such as in `C:\Games\Diablo II\`.
	- If this issue continues to happen, especially after updating the game, try [using the standalone patch](http://ftp.blizzard.com/pub/diablo2exp/patches/PC/LODPatch_114d.exe) to update the game.
2. An improperly configured Glide can cause this issue. Be sure you run the `Query OpenGL-infos` option in the Glide program so that options your PC does not support is disabled. This only applies if you are using Glide.
3. You're trying to launch in fullscreen and fullscreen just does not work for most people. Launch in windowed mode to see if it works.

### `Extremely low FPS`

1. If the lag shows its tendencies around mobs and a lot of activity. Try running the game with sound disabled, using the `-ns` flag. If this fixes it, its a sound issue. Install an [audio fix](https://www.indirectsound.com/) that allows sound to work better for older games. Be sure to read the `How Does It Work?` section. Simply take the `dsound.dll` and put it into your Diablo 2 folder. This should not get you banned online, as it simply replaces the Windows `dsound.dll` with this one.
2. Your modern computer does not play well with the graphics engine of the video mode you are using.
	- If you are using Glide, be sure it is properly configured (by running the `Query OpenGL-infos` option). If this does not help, Glide probably does not work for you and you will have to play without Glide.
		- Glide simply does not work well for some people.
	- If you are not using Glide, try [using Glide](https://github.com/Warren1001/MrLlamaSCStreamInfo/blob/master/GlideInstallGuide.md).

### `CD-Key in Use` (by yourself)

This issue happens because a game server crashed while you were in the game. As a result, the realm still thinks you are in a game, when you are not. The only way this issue gets resolved is for the realm server to realize you are, in fact, not in a game. Usually the issue corrects itself in 5 minutes. However, occasionally a game server can hang hard and it can be up to 48 hours for the issue to fix itself.

### `CD-Key in Use` (by someone else)

1. You bought a CD key from someone that was not Blizzard and someone other than you also has access to this key (you got scammed, basically).
2. You bought it from Blizzard and the CD key was brute-forced. Unlucky. Only way around this is to simply get a new CD key.
	
### `Unable to connect to Battle.net`

1. Most of the time, this is usually a 5 minute ban (called tempban) for performing too many actions too fast. Actions include:
	- Creating/leaving/joining games too quickly. You are allowed to create 20 games per hour per IP. Game lengths should be at least 3 minutes.
	- Spammed a lobby channel or a realm command like /friends or /whisper.
	- Spammed a NoDelay skill far too much or scrolled through your skills with Scroll Wheel at a very fast rate.
	- Other actions exist.
2. The server is simply down. You get this error on occasion during a Ladder Reset.
3. Be sure Diablo 2 is allowed through your Firewall. Search `Allow an app through Windows Firewall` in the Start Menu. Be sure all Diablo 2 instances have both private and public checked.
4. Windows does not like your user account and, for some unknown reason, it doesn't let you connect.
	- This can be the case if you are able to connect to Battle.net on a different PC on the same IP but affects all realms on the PC with the issue.
	- The way to resolving this is simply creating a new admin user on your PC and see if launching Diablo 2 on there works.
	
### `Diablo II was unable to connect to the realm server` (in the Character selection screen after login)

1. The ladder is resetting or there is a server issue.
2. Similar to the tempban, however usually longer for repeat offenders. This is called a realm down (r/d). See #1 for "Unable to connect to Battle.net".
	- Can last anywhere from 5 minutes to 48 hours.
	
### `Gateway: None` (In the main menu)

1. Somehow your realms in the registry got deleted (usually happens because of mods). [Run this](http://ftp.blizzard.com/pub/misc/BattleNet.zip).
	
### Forcing your ISP to resolve a realm IP


##### This fix is used for a rare issue when connecting to the Battle.net servers.

Fzarg (06/16/2018):

> @Warren1001 Found a solution to the 'Checking Versions' problem. Apparently it's only affecting certain ISP's in combination with specific DNS providers.\
> By forcing your local hosts lookup table to resolve the name of blizzards hostname into a specific IP, it's working flawlessly.\
> Edit C:\Windows\System32\drivers\etc\hosts and add: 5.42.181.18 europe.battle.net

This fix can be applied to other realms as well. There are multiple IPs you can try incase one does not solve it.

`useast.battle.net`: `199.108.55.59`, `199.108.55.58`, `199.108.55.57`\
`uswest.battle.net`: `12.129.236.19`, `12.129.236.18`, `12.129.236.17`\
`europe.battle.net`: `5.42.181.18`, `5.42.181.17`, `5.42.181.16`, `5.42.181.15`, `5.42.181.14`\
`asia.battle.net`: `121.254.164.19`, `121.254.164.18`, `121.254.164.17`\

To apply this fix, you need to edit your HOSTS file which can be found at `C:\Windows\System32\drivers\etc\hosts`. You can use the `Run` program to open this file (Windows button + R). Open it with any text editor.  
At the end of the file, you write the numerical IP that you are trying, then a space, then the letter IP.  
If I were wanting to try to use the IP `199.108.55.59` to connect to USEast, I would write `199.108.55.59 useast.battle.net` to the end of the HOSTS file and then save it.  

If this fix ultimately ends up not helping you, you should remove the entry from the HOSTS file, as you generally do not want to modify the HOSTS file unless you need to. If this fix does work for you, and after some time it stops working, try removing the HOSTS file entry and connecting without it to see if it works.
\
\
\
##### If these fixes do not help resolve your issue, @mention or DM Warren1001 or post in the `# technical-support` detailing your issue on [MrLlama's Discord](https://discord.gg/BePVw9e).
