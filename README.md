# Complete guide for maximum performance on Yuzu + Download links for Keys, Firmware, Switch Games and Shaders
### Hi and welcome! This [subreddit](https://www.reddit.com/r/NewYuzuPiracy/) is about pirating Yuzu as you can guess from the title. In this post, we'll help you to get yuzu up and running. Please read the post till the end to maximize performance. Links for keys, firmware, switch games and shaders at the end of the post.


1. Installing the Emulator
Install yuzu from https://yuzu-emu.org/downloads/. After you've done that, you can install the Early Access builds that we give out here for free too but if you want you can keep using the mainline versions

2. Installing Keys and Firmware
When you launch yuzu for the first time it will show an error of missing components. To fix that, you'll need to get the prod.keys file which you can get from here

OG Link: https://codebeautify.org/base64-decode?input=aHR0cHM6Ly9kcml2ZS5nb29nbGUuY29tL2ZpbGUvZC8xLU5uZHBIZTBJZWN2TFh1X1lZWERHQl9hSDNvYkhRWkkvdmlldz91c3A9c2hhcmluZw== (dead)
Mirror: https://drive.google.com/file/d/16RPCsmTWgnwRANJTQcaRi-ORgApFER_j/view?usp=sharing

Once you install the prod.keys file, open yuzu (you will still get the error for now) and go to the top left corner and click on "file" and then "Open yuzu Folder". It will open a folder, make a folder and name it "keys" and put the prod.keys file on there. Restart yuzu and you shouldn't get the error (if you get the error again, you've done something wrong. Make sure you followed the steps and did it correctly!)

Note: Title.keys are not required as yuzu autogenerates them. Firmware is only needed for a few games such as Mario Kart 8 Deluxe. You can get firmware from here aHR0cHM6Ly9kYXJ0aHN0ZXJuaWUubmV0L3N3aXRjaC1maXJtd2FyZXMv

Open yuzu and go to the yuzu folder then nand\system\Contents\registered and paste all the firmware files in there.

3. Getting your games
Now you'll need your games. Where to get switch games? Well here is a list of a few websites that have switch games

aHR0cHM6Ly9ueGJyZXcuY29tLwoKaHR0cHM6Ly9uc3cydS5jb20vCgpodHRwczovL3d3dy56aXBlcnRvLmNvbS8KCmh0dHBzOi8vd3d3LnNvZnRjb2JyYS5jb20vCgpodHRwczovL25zd2dhbWUuY29tLw==
Mirror: https://pastelink.net/torrjmy2
(Paste the above link in https://www.base64decode.org and press decode to get real link!)

There are a few file types of switch games NSP, XCI, NSZ etc. You should ONLY download NSP or XCI. NSZ won't work. So you might ask do i download NSP or XCI? Well its up to you, both are fine.
Now make a folder and put your game files in it (only the game not the update or dlc). Open yuzu and double click on the yuzu screen. It will prompt you to select a folder, select the folder where you put the games, it will start to show the games you downloaded. You can launch a game by double clicking on it but first let's see how to install DLCs and updates. Go to the upper left corner and click file and "Install files to NAND" and choose your update/DLC file



4. Optimizing your emulator for the best performance
Now on to configuring your emulator for the best performance. Go to the upper left corner and click "Emulation" and then "Configure".
It will open up a yuzu configuration windows which has a few tabs. I'll go over all that requires changing.
General Tab
In the general tab make sure you have "Multicore CPU Emulation" ticked. Other than that, you can make changes to your own liking like the UI etc.
System Tab
In the system tab go to "Services" on the top and make sure BCAT Backend is set to none.
CPU Tab
On the "CPU" tab you only need to change the Accuracy to Unsafe and tick all the options that appear.
Graphics Tab
This is tab that's the most important. If you're using an Nvidia GPU, then always set your API to "OpenGL". If you're using AMD GPU, then set the API to "Vulkan". Make sure you have "Disk Shader Cache", "Asynchronous GPU Emulation" and "NVDEC Emulation" turned on. Then go to "Advanced" from the top and turn Accuracy level to Normal. Now if you're using OpenGL, turn on "assembly shaders" and turn off "asynchronous shaders". That should give you the best performance. For AMD GPU, turn on "asynchronous shader building" and "assembly shaders" should be off.
Audio Tab
The default settings on the Audio tab should be ok
Controls Tab
Its pretty straightforward, you just need to map your controls. You should choose "Pro Controller" for the emulated controller and then choose the controller you want to use in "Input Device". Yuzu will automatically map all the controls for you.
Those were the settings you needed to change in the emulator. Now let's look at some other thing that can improve your performance
You should always run yuzu as administrator. How? If you're using the builds we give you from here, just go to the yuzu folder, right click yuzu.exe, click properties, go to the Compatibility tab from the top and tick "Run this program as Administrator". That makes sure that the settings you choose outside of yuzu are applied to it.

Now right click your windows icon and click "Power Options". Then on the rightmost side click "Additional Power Settings" and Choose the "High Performance" power plan.

This next step is for Nvidia GPU users only.
Right click on your desktop and click "NVIDIA Control Panel". Once it opens, click on "Manage 3D Settings" on the right. Once it opens, go to "Program Settings" and click Add and select Yuzu. Then scroll down the list of settings and Turn
Vertical Sync - Off
Triple Buffering - On
Threaded Optimization - On
Power Management Mode - Prefer Maximum Performance
OpenGL rendering GPU - [Select your GPU]
Then click Apply on the lower right corner.

One last thing. This step is mostly recommended for users who have low RAm for example 6 or 8 GB of RAM, however if you want constant stability you can try doing this too
You should change your Virtual Memory Pagefile to about 10,000 MB. How to do that? Here's a video tutorial https://youtu.be/u-UL-aKbE68 . Remember, only set it to about 10,000 MB

5. Installing Mods, Shader and Saves to your games
First, installing Mods. Right click the game you want to add a mod for. Then paste the mod there, the whole folder not just the files in it. You can get some basic yuzu mods from here https://github.com/yuzu-emu/yuzu/wiki/Switch-Mods .
Note: You can check which mods you have for a game by right clicking the game and clicking properties.

Now on to installing shaders. Open yuzu folder by clicking file on the top left corner and select "Open yuzu folder" and go to shaders\opengl\transferable and put your shader file there OR open the game you want to add shaders for and you can close it when it launches and shows some textures. Then right click the game and click "Open Transferable Shader Cache" and put the shader file there.
You can find shaders for some games on here https://docs.google.com/spreadsheets/d/1vFIQwLbbWBwdjxOVLNPvV4lv9E2kfmFSaWdSbmIh21M/edit?usp=sharing
Note: This is for OpenGL users only, Transferable shaders do not work on Vulkan on yuzu as of now.

And finally on to saves. To install saves, right click the game you want to add a save for, click Open Save data location and put the save files in there. You can find some saves for games on our discord.

6. Some Custom Game Settings
These are just some custom settings for specific games. To apply custom settings to games, right click the game and click properties and navigate to what you want to change.
You should use Vulkan for Legend of Zelda: Link's Awakening regardless of your GPU
You should use an Accuracy level of High for xenoblade games as Normal does not render the games perfectly
You should not use any update for Super Mario Odyssey. You should use the following mods for this game.
Disable Dynamic Resolution
Disable FXAA
Disable Camera Motion Blur
Disable Web Applet

Here I'll just put links for people who aren't willing to read the whole thing
Keys - https://drive.google.com/file/d/16RPCsmTWgnwRANJTQcaRi-ORgApFER_j/view?usp=sharing
Firmware - aHR0cHM6Ly9kYXJ0aHN0ZXJuaWUubmV0L3N3aXRjaC1maXJtd2FyZXMv
List of websites to get switch games from - aHR0cHM6Ly9ueGJyZXcuY29tLwoKaHR0cHM6Ly9uc3cydS5jb20vCgpodHRwczovL3d3dy56aXBlcnRvLmNvbS8KCmh0dHBzOi8vd3d3LnNvZnRjb2JyYS5jb20vCgpodHRwczovL25zd2dhbWUuY29tLw== or  https://pastelink.net/torrjmy2
Shaders - https://docs.google.com/spreadsheets/d/1vFIQwLbbWBwdjxOVLNPvV4lv9E2kfmFSaWdSbmIh21M/edit?usp=sharing

Put the above strings in https://www.base64decode.org to get real game

And that's it. That's the guide to maximize performance in yuzu. If i missed something or messed something up, don't hesitate to tell me about it in the comments section. If you're still having problems then you should join our discord server and ask for help there!
https://discord.gg/NF38g3ENVc



END OF POST------------
