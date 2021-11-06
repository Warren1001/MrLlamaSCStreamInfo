# How to Install Glide (any Diablo 2 version)

*Differences with using Glide*:
- The game looks nicer and better utilizes color.
- The game runs and feels smoother.
- The game takes slightly longer to load in load screens.
- The game usually performs better.

1. **Obtain the Glide wrapper files from [here](http://www.svenswrapper.de/gl32ogl14e.zip).**
	- You can view more information about the Glide wrapper [here](http://www.svenswrapper.de/english/index.html).
2. **Open `gl32ogl14e.zip` and drag all the files in the file to your Diablo 2 folder.**
3. **Run `glide-init.exe` that you just placed in your Diablo 2 folder.**
4. **If the application is not in English, click the second to the last button at the bottom, which reads `Deutsch/English`.**
	- Now the application should be in English.
5. **Click `OpenGL-infos` and then click `Query OpenGL-infos`.**
	- This will run a test to see what extensions your computer is capable of handling, and disable any that will not work.
6. **Click `settings`.**
	- `window-mode` should be checked if you intend to play Diablo 2 in windowed mode. You should be running in windowed mode as fullscreen does not work well anymore.
	- `captured mouse` should be checked if you want your mouse to be locked inside the Diablo 2 window so you cannot accidentally click outside of it.
		- There have been reports that this does not work for some people.
	- `keep aspect ratio` should be checked if you do not want your Diablo 2 window to be stretched and stay in the 4:3 resolution scale.
	- `vertical synchronization(VSYNC)` should be self explanatory. I would check it if it is not self explanatory.
	- `fps-limit` should be left alone.
	- `static size` can be changed to make your windowed Diablo 2 window take up more of your screen (similar to pressing the maximize button).
		- Though, using this will cause the mouse to interact weirdly if the mouse leaves the Diablo 2 window, and the mouse speed will feel very fast.
	- `window extras` is probably the minimize/maximize/close buttons at the top right. I wouldn't bother checking this option.
	- `centered` centers the Diablo 2 window in the middle of your screen.
	- `remember position` will put Diablo 2 back in the position it was last in when it was previously run.
7. **You can click `Test` to ensure everything runs smoothly.**
	- After you've tested it, simply click the red Exit circle.
8. **Navigate to the shortcut you use to start Diablo 2, right click it, and press `Properties`.**
9. **Go to the `Shortcut` tab and add `-3dfx` to the end of the `Target:` dialog box, the same way you have added `-w`.**
	- For most users, the `Target:` dialog box will read `"C:\Program Files (x86)\Diablo II\Diablo II.exe" -w -3dfx`.
10. **Run Diablo 2 using the shortcut!**

#### Note: Some people have reported that Glide makes their Diablo 2 run extremely slow. Sometimes this is the case, and you simply cannot use Glide. To stop using Glide, simply remove the `-3dfx` command from the `Target:` dialog box mentioned in Step 9.

##### Enjoy! If you run into any issues, @mention or DM Warren1001 on [MrLlama's Discord](https://discord.gg/BePVw9e).	
