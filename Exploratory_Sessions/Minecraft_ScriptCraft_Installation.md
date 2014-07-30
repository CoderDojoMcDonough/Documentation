##Quick installation instructions  
CoderDojo students with Windows laptops can use these instructions to streamline the installation of ScriptCraft:

1) Download this zip file containing the CraftBukkit server and ScriptCraft: http://coderdojomcdonough.github.io/assets/scriptcraft.zip .  Unzip this file after you have downloaded it.

2) Move unzipped folder and create desktop shortcut.  This step is optional.  Use File Explorer on Windows 8 (or Windows Explorer on Windows 7 and below) to move the unzipped ScriptCraft folder to the C drive of your computer or some other location on your disk.  You can also make a shortcut to the start.bat file on your Desktop so you can easily start the CraftBukkit server in the future.

3) Start the CraftBukkit server.  Double-click on the file named "start.bat".  A command prompt window should open.  
  * If you see a message "Loading libraries, please wait..." followed by dozens of lines of more text saying things like "Preparing spawn area", the CraftBukkit server is running properly so you can proceed to step the next step.
  * If you see a message "Loading libraries, please wait..." and the forth line says "Failed to load eula.txt", press any key to close the CraftBukkit command window.  Double-click on the file "eula.txt" and change the last line to "eula=true".  Safe and close the file.  Double-click on "start.bat" again to run the CraftBukkit server.
  * If you see the message "'java' is not recognized as an internal or external command", install Java from the http://www.java.com website.  If you have already performed that step and you are still seeing this error, Java will need to be added to your computer's path.  Adding Java to your computer's path is technically challenging... mentors at one of our coding sessions will be happy to help you with this task.  Instructons for adding Java to your classpath may be found here: http://www.java.com/en/download/help/path.xml

4) In the CraftBukkit command window type op {your_username} and hit enter, replacing {your_username} with your own minecraft username.  This will give you operator access which is necessary to run ScriptCraft.  The CraftBukkit server keeps track of operators in the ops.json file, so you do not need to perform this step every time you start the CraftBukkit server.


Full instructions for installing and configuring ScriptCraft can be found in the [The Young Person's Guide to Programming in Minecraft]
(https://github.com/walterhiggins/ScriptCraft/blob/master/docs/YoungPersonsGuideToProgrammingMinecraft.md#installation).
