# Deathloop Saves

## Description 

Enjoy Deathloop, but hate having to track down trinkets or search for that one gun you're not sure you have? Having fun speedrunning the patched game, but wish you didn't have to spend so long fiddling with Egor's code? 

These save files come with full inventories of all trinkets, a collection of every exemplar weapon with every possible perk in the game, and an easy-to-spin code for Egor's machine. 


## Table of Contents


* [Features](#features)
    * [Who Should Use These?](#who-should-use-these)
    * [Who Shouldn't use these?](#who-shouldnt-use-these)
* [Installation](#installation)
    * [Steam](#steam)
    * [Game Pass](#game-pass)
* [Contributing](#contributing)


## Features

There are three sets of save files in this repo: a fresh save that starts you at the tutorial, a save post tutorial with most of the game unfinished, and a save with every document read and lead followed, but without having actually broken the loop.

Each save comes in two flavors: a new invasion mode with no unlocks, and a max rank Julianna (though one without every unlocked feat). 

If you want your save file to have a win/loss ratio that's 100% yours, you can. And if you prefer to start with everything unlocked, including the Colt skins, that's an option too.

Every save file has the same features and codes—except for the tutorial save file which obviously starts you with a Colt lacking any infused weapons, trinkets, or slabs. These features include:

* The easy-to-spin code `A220` for Egor's machine
* Every personal and weapon trinket in the game, including the elusive Vampire trinket
* Trinkets are sorted—all trinkets of the same name are next to each other when equipping trinkets, and personal trinkets are loosely organized by category.
* An organized collection of every exemplar weapon in the game
* Duplicates of most one-handed weapons for dual-wielding
* Rare weapon skins
* A couple of weapons with perks given only to Julianna—they aren't found on Blackreef

What this collection of save files doesn't include:

* A collection of each weapon with a give perk in both possible skins of that weapon
* Non-Exemplar weapons
* Exclusive premium weapon skins
* Exclusive premium Colt/Julianna Skins
* In the mostly unfinished save, several early Julianna conversations are already complete, and all passwords to the RAK have been acquired—I avoided what I could but some interactions are necessary to collect all the guns and trinkets
* Save files from the unpatched pre-GoldenLoop version of the game (sorry speedrunners!)


### Who Should Use These?

* People who have played Deathloop, and want a conveniently organized and complete version of their inventory
* People who have broken the loop, but don't want to have to engage with the online mode to access the extra Colt skins
* People that enjoy having all of their infused gear, but want to revisit one-time missions,like hacking 2-bit, without having to do without their stuff
* People that enjoyed leveling up their Julianna's Hunter Rank and want to repeat the process without having to play the Colt side of the game all over again
* Speedrunners who want to break the loop glitchless, and enjoy having a guaranteed good code for Egor's machine

### Who Shouldn't Use These?

* People who have organized their own inventories just how they like them
* People with exclusive premium items and skins; I have no idea if these will be retained when using these save files and it's entirely likely that such exclusive content may be inaccessible with these saves
* Anyone who doesn't know how to make use of these save files for their particular platform; console players in particular may simply be unable to use these files at all, due to the closed nature of their filesystems


## Installation

In this case, installation refers to the process of downloading these files and using them to replace your existing Deathloop save file. This is easiest on Steam, but is also possible for Game Pass players.

While it may be possible to use these save files on other platforms, I don't know how. Also, it may not be possible. 

Regardless of what platform you're on, installation always starts with downloading this repository, or the specific folder you want to use. 

You can download a zipped folder of this repository by clicking the green `Code` button, and selecting `Download Zip` from the dropdown menu. 

If you have Git, you probably don't need any instructions on cloning or forking the repo. 

It is highly reccomended you make a backup of your original save file before trying to replace it with one of these. If something goes wrong, you don't want to lose all your progress. 

### Steam

To use these saves on Steam, you just need to locate your existing saved game and overwrite the file `save.dloop` with the appropriate save file from this repo. 

The steam save file is usually located here: 
`%USERPROFILE%\Saved Games\Arkane Studios\Deathloop\base\savegame\<user-id>\SLOT01`

`%USERPROFILE%` is your username on your computer, `<user-id>` stands in for your Steam ID. Once you find the Deathloop save folder inside `/Arkane Studios/`, it's pretty straightforward. 

Remember to make a backup of your save file, and then simply drag and overwrite your existing save file with whichever of these saves you wish to use. 

### Game Pass

Transferring these Steam save games to Game Pass is a little more complicated. Luckily, some people have already worked out the kinks. 

You'll just need a file editor, like Notepad++ (not regular Notepad), that can correctly read and save the Null characters in the save game. 

I've linked the original guide below, but in short, you need to open the file in Notepad++, or something similar, and delete the first few lines of text. 

You'll be deleting everything until the characters 'OOD', which should follow a string of NULLs. 

Then you'll need to locate your Game Pass save, which by default can be found here: 

`%USERPROFILE%\AppData\Local\Packages\BethesdaSoftworks.ProjectPrism_3275kfvn8vcwc\SystemAppData\wgs\<user-id>\<user-id>\`

There are three files in there. One is a small 1kb file with a bunch of random numbers and letters as the file name, along with a `container.#` file. You want the largest file though,also with a bunch of random numbers and letters as a name, and missing a file extension.

Backup the file somewhere (that's your save), copy the name of the file, and then drop your modified Steam save (`save.dloop`) file in the save game folder. 

Rename the Steam save to random letters and numbers you copied from the other file name, and make sure you remove the `.dloop` file extension. You may have to change your file explorer preferences so that file extensions are visible. 

Congratulations! Start up Deathloop, and your save file should be successfully overwritten. If it doesn't work for some reason, check out the original guide below, and remember, you can always drop the backup of your original save back into the save game folder to return to your original game. 

[Here's a link to the guide](https://www.reddit.com/r/Deathloop/comments/xl6snh/guide_transfer_steam_saved_game_to_game_pass/)

[And an archived link](https://web.archive.org/web/20230317100708/https://www.reddit.com/r/Deathloop/comments/xl6snh/guide_transfer_steam_saved_game_to_game_pass/)

Although the guide suggests copying over the files `title.data` and `steam_autocloud.vdf`, it shouldn't be necessary to copy those over—just the main `save.dloop` file.

## Contributing

Contributions to this repository, like interesting save files you want to share, are welcome. 

Want to add instructions for using this save file on other platforms? Have a code even better than A220? Like your collection of guns better, and think others will too?

Submit a pull request!

--- 
