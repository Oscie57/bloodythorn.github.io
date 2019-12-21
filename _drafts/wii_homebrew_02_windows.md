---
layout: post
title:  "WiiHacks:Developing Wii Homebrew - Part 02 - Windows"
categories: 
  - development
  - wiihacks
published: false
---

## Notes about my environment

Currently I am working on a windows 10 computer. It has mediocre stats for gaming. This tutorial should work on any Windows... I'd say XP system and up. Which means you'll at least need to be on an x86 environment. If you're not familiar with that term, x86 is the intel standard for modern processors. Any system that is compatible with those standards should work fine.

## Setting up your environment in Windows

Time for the first web link, [devkitPro.org](https://devkitpro.org/).

There's still a fairly active community on this site. I personally haven't gotten involved yet because I already have waay too many social sites to focus on. However it would be a great place to go if you have issues.

In our case, we need the ["Click Here for instructions on installing the tools and getting started"](https://devkitpro.org/wiki/Getting_Started) link. This should take us to the devkitpro wiki. Another resource you should have bookmarked.

On this page, we have the [Windows](https://devkitpro.org/wiki/Getting_Started#Windows) section that gives us a link to the [latest version](https://github.com/devkitPro/installer/releases/tag/v3.0.3). This will take you to the [github repository for the devkitpro developers](https://github.com/devkitPro), another valuable resource.

The latest version as of this article is 3.0.3, updated Jun 3, 2018. Remember if this has changed, this tutorial might not work. At the bottom is a link for the [devkitProUpdater-3.0.3.exe](https://github.com/devkitPro/installer/releases/download/v3.0.3/devkitProUpdater-3.0.3.exe). Download it and save it to a location where you'll be able to find it.

You will need an internet connection to run the installer, but hopefully you do as you also needed one to download it. When you run the executable you'll be taken through a few options. Defaults are all fine, I'd recommend not changing the install path from 'c:\devkitPro'. You'll also want to make sure that the Wii Development environment is checked. It is by default. You can uncheck other environments if you think they might confuse you, but the amount of space it takes up is fairly small, so for me it is easier to just install it all.

Once you reach the end of the user input phase of the installation, you'll have a typical installer with a progress bar. During this process it will open several console windows and run scripts. On the first one I had to hit enter a couple of times as it seemed to either be waiting on input, or it stalled. I hit enter to remedy this. So if it's sitting too long in one place, don't feel scared to hit enter. It won't interrupt the script if it isn't needed, and could help if it is.

I also don't recommend doing anything else while this is running. I was trying to take notes for this article, and the newly opened windows kept stealing my focus and I almost ended up typing in a few. Wait till it's done with the last one, and finish out the install.

Congratulations! You should now have a functional Wii development environment installed on your windows machine. But we still need to test it, eh?

So, to test that the functionality of our newly installed development environment, we'll compile the Wii examples that come with it. If you want to open up an explorer (and didn't change the install path), they should be installed to 'C:\devkitPro\examples\wii\'.

You can look at the code for them too! If you go into the directory 'C:\devkitPro\examples\wii\graphics\gx\triangle\source\' there will be a file 'triangle.c'. Open it up with a text editor. I recommend sublime 3, but use what you're comfortable with. Just make sure it's a *text editor* , and not a *word processor*. A text editor will read and write raw text files without including the meta-data that word processors use to store formatting and other information.

Press 'start' and type 'msys', or if you're on a different version of windows you should be able to find it in your start menu. You can use [this](https://devkitpro.org/wiki/Getting_Started#Windows) as a reference. If you're used to a Windows shell, this should look like it's opened up a funny looking shell. If you're familiar with a posix/linux/unix environment, you'll notice it's just opened a bash shell.

I'm assuming the development environment was originally setup in linux, but tools like msys and cygwin, even the new Windows 10 Bash functionality will allow us to use all the tools we need in Windows. It will then use that system to cross compile a PowerPC application that we can run on the Wii via the Homebrew Channel.

When the terminal opens, you should be in your home directory, 'C:\user\you'. If you type 'dir', or more appropriately 'ls' (yes, both will work), you'll get the directory listing for your home directory. What we want is in a different directory, but since this environment is simulated, it will be in a different location than the directory we just visited.

Type 'cd /opt/devkitpro' and it will take you to the root of the devkitPro install in msys. devkitPro uses the 'opt' (short for optional packages/software) in both the msys, and linux environments. If you type 'dir' again, we should see an 'examples' directory. What we want is in there.

Let's change directories again, 'cd examples/wii/' should take you into the directory for the Wii examples. If you installed all of the options during the initial install, you should have several more directories than just 'wii', but that's the one we want.

To see what is in here, type 'ls -alh' it should make a slightly different looking directory listing:

To explain the flags for how we changed the look of the directory, a - all entries, including hidden, l - long format listing, h - human readable. There will be different directories for each type of example that match the directories we went through in the file manager.

But most importantly, is the *Makefile*. What this is is a 'project file' or more accurately called a build system configuration for the build system 'make'. Make is part of the GNU tool chain, and is used to configure larger projects that use the GNU compiler suite to build themselves.

Feel free to open with a text editor it and inspect it. Unfortunately we won't be going over makefiles much as it's an older technology, and we haven't gotten to a point where we'll need to manage our projects. We'll worry about that later.

Okay, time to build the examples. From the '/opt/devkitpro/examples/wii' directory, type 'make all' and it should start to build all the examples. I have yet to do this and not have it work, so I don't really have any failure scenarios to run over. It should work if everything done up until now has been the same on your environment.

Last line you should see is './template/template.dol' -> 'bin/template.dol', and there should be no errors afterwards, just the command prompt. If everything went well, you just built your first Nintendo Wii application. Soon, you will have coded your first Wii application. But let's make sure they work first.

We're going test some of these applications in [Dolphin](https://dolphin-emu.org/), as it keeps us from having to have a Wii on hand for now. Another one you'll want to bookmark. When you click on the download button, it will take you to the download screen.

We will skip the developmental versions as they require a redistributable, and we can skip that since we don't really *need* the latest build. Stable will just be fine.

We will be using the [Stable Windows x64 Build](https://dl-mirror.dolphin-emu.org/5.0/dolphin-x64-5.0.exe). If you don't have a 64 bit system you can try the 4.02 build (x86), but I cannot guarantee that this will work on that version.

Download and install. Any issues, hit the Dolphin forums. It will put a desktop icon you can double click on, or find it in your start. Yes or no to the data usage and we should now have the Dolphin proper interface in front of us. Click 'Open' and it should bring up a file selection window. Click on 'This PC' on the left side. We're going to go to 'C:\devkitPro\examples\wii\graphics\gx\triangle' and open the 'triangle.elf' file.

What it should open is what we call the 'Hello World' of an OpenGL application. A multicolored triangle over a black background. It's the *same* code we were looking at earlier!

Wow, this got long. If you have any issues or corrections in the tutorial, please feel free to open an issue on the corresponding github. We've now preped our environment, and we've assured ourself that we can now get code from text to executable.

Next we'll be setting up our own project, and making some 'Hello World's that we actually write.

### When the next article is written, the link to it will be here.