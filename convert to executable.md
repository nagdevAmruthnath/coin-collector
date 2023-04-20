# Converting Coin Collector Game to Executable

If you want to distribute your Pygame-based game as an executable file, you can use PyInstaller to create a standalone executable package that includes all of the necessary dependencies. This allows users to run your game without having to install Python or any additional packages.

Here are the steps to convert the Coin Collector Game to an executable file:

## Step 1: Install PyInstaller

First, you need to install PyInstaller by running the following command:
```
pip install pyinstaller
```
##Step 2: Create a Spec File

The next step is to create a spec file for your game. A spec file is a configuration file that tells PyInstaller how to package your game. You can create a spec file by running the following command:
```
pyinstaller game.py --name game --onefile
```
This command creates a spec file called game.spec and a build directory containing the necessary files.
## Step 3: Edit the Spec File

Open the game.spec file with a text editor and add the following lines:
```
import os
os.environ['PYGAME_HIDE_SUPPORT_PROMPT'] = '1'
```
This hides the Pygame support prompt that is displayed when the game is launched.
## Step 4: Build the Executable

Once you have edited the spec file, you can build the executable by running the following command:
```
pyinstaller game.spec
```
This creates a dist directory containing the standalone executable file.
## Step 5: Test the Executable

You can test the executable by navigating to the dist directory and running the game.exe file. The game should launch and function as expected.
## Step 6: Distribute the Executable

Finally, you can distribute the executable file to other users. They can simply double-click the game.exe file to launch the game without having to install Python or any additional packages.

Note: The size of the executable file may be large due to the inclusion of all necessary dependencies. You can reduce the size by using PyInstaller's --exclude-module option to exclude unnecessary modules or by using UPX to compress the executable.
License

This project is licensed under the MIT License. See the LICENSE file for more details.