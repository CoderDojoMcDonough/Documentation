## Installation

Students interested in our Minecraft modding with JavaScript session should have a laptop with Minecraft installed and a Minecraft account.  Some students have successfully used a 30-day demo Minecraft account, but we encourage students to purchase a Minecraft license.  

Please make your best attmempt to install the CraftBukkit server on your laptop before attending your first session.  There are mentors available to help if you're unable to get things running, but another mentor will be guiding students through scripting in Minecraft even if  some students are not able to get the CraftBukkit server running and connected to Minecraft.

[Click here](Minecraft_ScriptCraft_Installation.md) to view our streamlined installation instructions for Windows users.  These steps were created using the installation instructions found in the Young Person's Guide link below, but they save parents or students from having to download separate jar files and create their own start.bat file.

Full instructions for installing and configuring ScriptCraft can be found in the [The Young Person’s Guide to Programming in Minecraft](https://github.com/walterhiggins/ScriptCraft/blob/master/docs/YoungPersonsGuideToProgrammingMinecraft.md#installation) - This guide contains details on how to start using JavaScript with Minecraft. We’ve tested Minecraft version 1.7.10 along with CraftBukkit version 1.7.10-R0.2. 

[Click here](Minecraft_ScriptCraft_Installation.md#run-craftbukkit-without-an-internet-connection) for instructions on running the CraftBukkit server without an internet connection.

If you see the error message "You don't have scriptcraft.evaluate permission” when using ScriptCraft in Minecraft, see step 4 in our streamlined [installation instructions](Minecraft_ScriptCraft_Installation.md).

## Documentation links

[ScriptCraftJS.org](http://www.ScriptCraftJS.org) - Documentation links for ScriptCraft

[The Young Person’s Guide to Programming in Minecraft](https://github.com/walterhiggins/ScriptCraft/blob/master/docs/YoungPersonsGuideToProgrammingMinecraft.md#installation)

ModderDojo Athenry projects  
http://cdathenry.wordpress.com/category/modderdojo/page/3/

Bukkit API reference docs  
http://jd.bukkit.org/dev/apidocs/

Minecraft Data Values  
http://minecraft.gamepedia.com/Data_values

Minecraft server properties file  
http://minecraft.gamepedia.com/Server.properties


## Set time and storm

I find it helpful to switch the time of day when it gets dark or turn off a storm...

change time of day to daytime:  
self.location.world.setTime(6000);  
https://github.com/walterhiggins/ScriptCraft/blob/master/docs/API-Reference.md#example-create-a-sign-which-changes-the-time-of-day

set storm:  
server.worlds.get(0).setStorm(false);  
https://github.com/walterhiggins/ScriptCraft/blob/master/docs/API-Reference.md#example-5

## Ideas for mods

Conway's Game of Life  
http://en.wikipedia.org/wiki/Conway's_Game_of_Life

Maze building  
http://www.mazeworks.com/mazegen/mazetut/
