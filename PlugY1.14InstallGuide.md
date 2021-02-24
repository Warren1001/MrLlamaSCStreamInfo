# How to Install PlugY for Diablo 2 version 1.14d (or any version, really)


#### As usual, the PlugY files being in your Diablo 2 folder may risk you getting banned if you connect to the Battle.net even without PlugY loaded. As such, you should have a separate installation for PlugY if you also want to play on Battle.net.	


1. **Install Diablo 2 as normal** ***AND*** **patch it to 1.14d.**	
	- You can patch the game by simply connecting to Battle.net.	
	- *If you already have Diablo 2 1.14d installed, you can simply copy and paste the Diablo 2 folder and rename it to something that indicates it is your Diablo 2 for Battle.net.*	
		- They way PlugY works, PlugY has to be installed to the Diablo 2 path that was most recently listed in the installer. If you install PlugY into the folder that you copy and paste, you will run into errors. So make the Diablo 2 folder that you copy and paste your unmodded Diablo 2, and the original folder will become the modded Diablo 2.	
			- However, any pre-existing shortcuts for unmodded Diablo 2 will link back to the PlugY version, which can have issues listed in the warning above. Delete pre-existing shortcuts for Diablo 2, and create a new one from the unmodded Diablo 2 folder in the same way that is shown in steps 6-8 for `Diablo II.exe`.	
		- So, if you have taken this step, your Diablo 2 folder for installing PlugY will be the original folder.	
2. **Navigate to your Diablo 2 folder.**	
	- For most users, your Diablo 2 folder will be located at `C:\Program Files (x86)\Diablo II\`.	
	- You can quickly get to it by right clicking on the newly created Diablo 2 shortcut on your Desktop and pressing `Open file location`.	
3. **[Download PlugY v14.02 for Diablo 2 1.14d](http://plugy.free.fr/PlugY_The_Survival_Kit_v14.02.zip).**	
	- In the event the above link breaks, [visit here](http://plugy.free.fr/en/index.html). Get the Zip version.
4. **Open `PlugY_The_Survival_kit_v14.02.zip`.**	
5. **Take all of the files inside this .zip file and place them into your Diablo 2 folder.**	
6. **Right click the `PlugY.exe` file that you just placed in your Diablo 2 folder. Press `Send to > Desktop (create shortcut)`.**	
	- This creates a shortcut to launch PlugY from your desktop. You will need a shortcut either way to launch in windowed mode.	
7. **Go to your Desktop, right click the PlugY shortcut we just created, and press `Properties`.**	
8. **Go to the `Shortcut` tab of the Properties window. In the `Target:` box, add `-w` to the end.**	
	- This will launch PlugY in windowed mode.	
	- Your `Target:` box should read something similar to `"C:\Program Files (x86)\Diablo II\PlugY.exe" -w`.	
		- The `"` at both ends of the path are required to add `-w` to the end.	
9. **Use the shortcut on your desktop to play Diablo 2 with PlugY!**	

##### Enjoy! :)	


## If you are upgrading from 1.13 PlugY to 1.14 PlugY and wish to use your old saves, you will need to follow these steps as well:	

1. **Go to your old PlugY installation. Your character saves will be in the Diablo 2 folder in the Save folder.**	
2. **Move all these files to the 1.14 save location. This is found in your Saved Games folder.**	
	- The Saved Games folder is usually located at `C:\Users\[your user]\Saved Games\Diablo II\`	
3. **Lastly, you will have one or two `x_SharedStashSave.sss` files, depending on if you did or did not play both softcore and hardcore. You will need to rename one or both of them to have a `_` in front of the file name.**	
	- For softcore, you will originally have a file named `LOD_SharedStashSave.sss`. It should be changed to read `_LOD_SharedStashSave.sss`.	
	- For hardcore, you will originally have a file named `LOD_HC_SharedStashSave.sss`. It should be changed to read `_LOD_HC_SharedStashSave.sss`.	
	- If your files already have a `_` in front, then you're all good!	



#### If you have any issues or questions, post in the [#technical-support channel on MrLlama's Discord](https://discord.gg/BePVw9e).
