# A Manual Archipelago for You Have to Win The Game

Requirements
* Archipelago 0.6.5 or later
* Manual Client for Archipelago
* A Steam installation of You Have to Win The Game (don't worry, it's free!)

Setup
* Find your personal folder for YHTWTG.
* As an example, mine is in here C:/Users/blitzashspear/Documents/My Games/You Have To Win The Game.
* This folder should contain a bunch of other folders.
* This is NOT the same as the folder where the executable is.
* Take everything in Maps and place all of the files into the Maps folder.
* Take everything in Mods and place both files into the Mods folder.
* Take everything in Saves and place it into the Saves folder. Alternatively, you can edit your save manually as you play.
* If everything was installed correctly, when booting the game, you should have the option to continue from a save called Archipelago.
  Connect your Manual Client like any other manual and enjoy!

Playing
* Since I've given you all of your major items in the save file, it is your responsibility to not use them until you have recieved the check in the client.
* In the original game, once you get all 4 of your major items you can go directly to the goal.
* I have changed the goal condition. In order to goal you must find the letters that make up the magic word. These are E, P, R, S, and U.
* The rest of the letters are mixed in as filler for funsies.

Changes
* The map mod has extra platforms and teleporters to prevent softlocking and allows you to backtrack to the start.
* The orbs have been replaced with the money bag item.
* The texture mod replaces all of the money bags and pirate hearts with the Archipelago logo.

Editing Save Data Manually
* If you did not replace Autosave.vsg, you will need to follow these instructions.
* Save your game and exit to the title screen.
* Open up Autosave.vsg in your hex editor of choice.
* Find the consecutive bytes 80 40. For me they are on 0x4020 and 0x4030. It may be different for you.
* The next 4 bytes after that are your major items. Left to right are Cerulean Aura, Crimson Aura, Springheel Boots, Spider Gloves.
* Just change 00 to 01 for the corresponding item. Make sure you are overwriting the byte and not inserting it. You will brick your save otherwise.
* Save Autosave.vsg, exit your hex editor and re-enter the game.
* Double check you have exited the hex editor. Saving multiple times in quick succession while having your hex editor open may cause your game to crash. 
