### Teensy 4.1

Setup (first time):
1. Download VSCode.
2. Get C/C++ extension for VSCode.
3. Dowload PlatformIO for VSCode. https://platformio.org/platformio-ide 
4. Check the PlatformIO QuickStart guide: https://docs.platformio.org/en/latest//integration/ide/vscode.html#quick-start
By following the steps in the guide PlatformIO will download all tools needed for Teensy 4.1

To use this code you will need to pull it from github onto your computer.

5. Create a folder on your computer to host the files of this program.
6. Clone the github repository onto the folder.
7. Now open VSCode, open the PlatformIO home menu and open this project (naviguate to the folder where you cloned this project).
8. Build the project and run it!

***Optional:***
To remove the squiggles/error messages, you need to generate a .vscode folder containing "c_cpp_properties.json" and "launch.json" files.
To do that, follow these steps. (Note that the code will build correctly even without removing the squiggles).

1. Open `platformio.ini` file, and add the following line:

`-D generate_vscode_folder=1`

This is a simple macro definition. 
2. If this line is already present, simply change the value it is equal to, for example:

`-D generate_vscode_folder=0`

Now save your changes and build the project. The objective was to modify the `platformio.ini` file because doing so prompts PlatformIO to generate a new ".vscode" folder.
