# How to Install d2modmaker (Randomizer mod) for Diablo II


##### This guide works for 1.13 AND 1.14, and includes optional steps to have PlugY as well.
##### If you're a video guide type of person, [here is Llama's video guide](https://www.youtube.com/watch?v=1A5tyriB6kY).


1. **Install your desired Diablo II version.**
	- The version does not matter. Diablo II 1.13x and 1.14x have both been confirmed to work. The install method used does not matter either.
	- If you want PlugY, install PlugY first. Additional PlugY steps can be found below for mod compatibility.
		- You can install [PlugY](https://github.com/Warren1001/MrLlamaSCStreamInfo/blob/master/PlugY1.14InstallGuide.md) here. This guide works for any Diablo 2 version.
2. **Install [d2modmaker](https://github.com/tlentz/d2modmaker).**
	- You can find the download under [Releases](https://github.com/tlentz/d2modmaker/releases).
		- Under the image for the latest version, there is an `Assets` dropdown menu. The zip file is found there.
	- To install, you simply open the zip file and drag and drop all files into your Diablo II folder.
3. **Run d2modmaker.**
	- d2modmaker comes with two executables. Use the one that your system should use.
		- If you have no idea, use `d2modmaker-windows-386`. I had no issues using this executable on a 64-bit system.
			- New information states that this mod may only work for 64-bit systems.
	- This will open a web UI in your browser.
4. **Configure the mod to your desire.**
	- You can find information about the options at the [d2modmaker website](https://github.com/tlentz/d2modmaker).
5. **Save the configuration and generate the files for the mod.**
	- To do this, press `Save Config` and `Run` at the top of the editor.
6. **Add the launch arguments `-direct -txt` to the shortcut you use to launch the game.**
	- To do this, go to the shortcut properties, go to the `Shortcut` tab, and find the `Target` box. Add `-direct -txt` to the end, the same way you would with `-w`.
	- This same step applies to PlugY. Add the launch arguments to the PlugY shortcut the same way you do for a normal Diablo II shortcut.
7. **Launch the game and have fun!**


##### Do know that each time you press `Run` in the editor, you will re-generate all the randomized items. If you want to modify settings but keep the same randomized items, there is a `Seed.txt` in your Diablo II folder which has the randomization seed. Use the `UseSeed` option in the editor to specify the specific seed stored in your `Seed.txt` file to keep the same randomization.


#### If you have any issues or questions, post in #technical-support on [MrLlama's Discord](https://discord.gg/BePVw9e) or ask the mod managers themselves at [their Discord](https://discord.com/invite/eQt2Z9b).
