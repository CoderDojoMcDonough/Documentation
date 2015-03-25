##Quick installation instructions for ScriptCraft

We have created a zip file to help streamline the ScriptCraft installation process.  CoderDojo students with Windows laptops can use these instructions to install the CanaryMod server and ScriptCraft.

1.  [Click here](https://dl.dropboxusercontent.com/u/9362458/CoderDojoMcDonough/CanaryModServer.zip) to download a zip file containing the CanaryMod server and ScriptCraft.  Unzip the file when the download is complete.

2.  Move the unzipped folder and create a desktop shortcut.  This step is optional.  Use File Explorer on Windows 8 (or Windows Explorer on Windows 7 and below) to move the unzipped ScriptCraft folder to the C drive of your computer or some other location on your disk.  You can also make a shortcut to the start.bat file on your Desktop so you can easily start the CanaryMod server in the future.

3.  Start the CanaryMod server.  Double-click on the file named "start.bat".  A command prompt window should open.  
  * If you see a message "Loading libraries, please wait..." followed by dozens of lines of more text saying things like "Preparing spawn area", the CanaryMod server is running properly so you can proceed to step the next step.
  * If you see a message "Loading libraries, please wait..." and the forth line says "Failed to load eula.txt", press any key to close the CanaryMod command window.  Double-click on the file "eula.txt" and change the last line to "eula=true".  Safe and close the file.  Double-click on "start.bat" again to run the CanaryMod server.
  * If you see the message "'java' is not recognized as an internal or external command", install Java from the http://www.java.com website.  If you have already performed that step and you are still seeing this error, Java will need to be added to your computer's path.  Adding Java to your computer's path is technically challenging... mentors at one of our coding sessions will be happy to help you with this task.  Instructons for adding Java to your classpath may be found here: http://www.java.com/en/download/help/path.xml

4.  In the CanaryMod command window type op {your_username} and hit enter, replacing {your_username} with your own minecraft username.  This will give you operator access which is necessary to run ScriptCraft.  The CanaryMod server keeps track of operators in a text file, so you do not need to perform this step every time you start the CanaryMod server.

5.  Follow the ["First Steps" section on the Young Person's Guide to Programming in Minecraft](https://github.com/walterhiggins/ScriptCraft/blob/master/docs/YoungPersonsGuideToProgrammingMinecraft.md#first-steps) to connect the CraftBukkit server you just finished setting up with your Minecraft game. 



Once you have successfully installed ScriptCraft, we recommend that you continue reading through [The Young Person's Guide to Programming in Minecraft]
(https://github.com/walterhiggins/ScriptCraft/blob/master/docs/YoungPersonsGuideToProgrammingMinecraft.md#installation).


##Run CraftBukkit without an internet connection (Outdated!)
The CraftBukkit server will attempt to authenticate users using your internet connection.  In order to start the CraftBukkit server properly when you are not connected to the internet, stop the CraftBukkit server and change the first line of the start.bat file from:  
java -Xmx1024M -jar craftbukkit.jar -o true  
to...  
java -Xmx1024M -jar craftbukkit.jar -o false

The "-o" parameter will cause the server to start in online mode if set to true and offline mode if set to false.  This value overrides the "online-mode" value in the server.properties file.  Instead of using the -o paremeter in the start.bat file... you could remove the -o parameter from the start.bat file and edit the server.properties file and change the online-mode setting to false to enable offline mode.

Please note that you will run into problems if you start the CraftBukkit server or Minecraft with an internet connection and then you go offline.  So if you need to run Minecraft without an internet connection, disconnect from the internet and then start the CraftBukkit server and then start Minecraft.

You should not run the CraftBukkit server in offline mode if you have a working internet connection.  If you have a workign internet connection you should set the -o startup parameter in the start.bat file to true.  When you're running in offline mode you'll see warnings in the CraftBukkit command window saying the following:  
> **** SERVER IS RUNNING IN OFFLINE/INSECURE MODE!  
> The server will make no attempt to authenticate usernames. Beware.  
> While this makes the game possible to play without internet access, it also opens up the ability for hackers to connect with any username they choose.

