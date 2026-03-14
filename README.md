# Deathloop Saves

## Description 

Enjoy Deathloop, but hate having to track down trinkets or search for that one gun you're not sure you have? Having fun speedrunning the patched game, but wish you didn't have to spend so long fiddling with Egor's code? Want to play through the main game again, but hate the idea of having to painstaking recollect all your gear?

These save files come with full inventories of all trinkets, a collection of every weapon with every possible perk in the game (though not in every skin), and an easy-to-spin code for Egor's machine. 


## Table of Contents


* [Features](#features)
    * [Who Should Use These?](#who-should-use-these)
    * [Who Shouldn't use these?](#who-shouldnt-use-these)
* [Installation](#installation)
    * [Steam](#steam)
    * [Game Pass](#game-pass)
* [Additional Details](#additional-details)
    * [Protect the Loop](#protect-the-loop)
    * [Sorted Gear](#sorted-gear)
    * [Weapons](#weapons)
    * [Personal Trinkets](#personal-trinkets)
    * [Reference Files](#reference-files)
    * [Colt Facts](#colt-facts)
* [Contributing](#contributing)


## Features

There are three sets of save files in this repo:

* New Game: Starts at the opening cutscene
* Mid Game: Starts after the tutorial with most of the game undiscovered
* End Game: Starts after almost everything has been discovered, completed, and read, but before the first time you break the loop. Hacking 2-bit, beating the Moxie, and talking to Pick Rexly are the only missions left untouched since they involve one-time events that I wish to repeat.

Each set of save games includes a fresh invasion mode, a Julianna without any matches but which includes favorable starting gear, and a max rank Julianna with every feat (except `Double Vision` and `You Lose Some`) unlocked. Unfortunately, the `Double Vision` feat for Julianna is bugged and apparently unobtainable. 

The `Mid_Game_Save` collection also includes intermediary saves from just after the tutorial and infusion lead with an empty inventory to a full and complete inventory with all slabs, upgrades, weapons, and trinkets.

Additionally, the saves have the following features on Colt:

* The easy-to-spin code `A220` for Egor's machine
* Every personal trinket in the game, including the elusive Vampire trinket, neatly sorted
* Every weapon & weapon trinket in the game, neatly sorted
* Duplicates of all one-handed weapons for dual-wielding
* Rare weapon skins—like the black Heritage Gun
* A couple of weapons with perks given only to Julianna—these aren't found on Blackreef
* Every document and cassette, neatly sorted
 

What this collection of save files doesn't include:

* A collection of each weapon with a given perk in both possible skins of that weapon
    * Notably, this collection includes only the purple variant of the Time Sensitive Heritage Gun
* Exclusive premium weapon skins
* Exclusive premium Colt/Julianna Skins
* Save files from the unpatched pre-GoldenLoop version of the game (sorry speedrunners!)
* A completely fresh Colt game with a full inventory—simply put, in order to acquire certain items, some story progression is required:
    * Most early Julianna conversations are already complete (this applies to all `Mid_Game_Saves`)
    * All passwords to the RAK have been acquired
    * The Time Sensitive Heritage gun is only available to Colt by completing the lead
    * Colt is on good terms with 2-Bit
    * Wenjie gets invited to the party every evening

### Who Should Use These?

* People who have played Deathloop, and want a conveniently organized and complete version of their inventory
* People who have broken the loop, but don't want to be forced to engage with the online mode to access the extra Colt skins
* People that enjoy having all of their infused gear, but want to revisit one-time missions, like hacking 2-bit, without having to recollect their gear
* People that enjoyed leveling up their Julianna's Hunter Rank and want to repeat the process without having to play the Colt side of the game all over again
* Speedrunners who want to break the loop glitchless, and enjoy having a guaranteed good code for Egor's machine

### Who Shouldn't Use These?

* People who haven't yet broken the loop—the `Mid_Game` and `End_Game_Saves` skip over story, dialogue, and gameplay experience and should be set aside until you've played through the game on your own
* People who have organized their own inventories just how they like them
* People with exclusive premium items and skins; I have no idea if these will be retained when using these save files, and (if it matters to you) the aesthetics of the weapon sorting won't take into account these premium items
* People who want to achievement hunt—I don't know how these save files might interact with Steam's achievment tracker
* Anyone who doesn't know how to make use of these save files for their particular platform; console players in particular are probably unable to use these files at all, due to the closed nature of their filesystems

## Installation

Installation refers to the process of downloading these files and using them to replace your existing Deathloop save file. This is easiest on Steam, but is also possible for Game Pass players.

While it may be possible to use these save files on other platforms, I don't know how. It also may not be possible. 

Regardless of what platform you're on, installation always starts with downloading this repository, or the specific folder you want to use. 

You can download a zipped folder of this repository by clicking the green `Code` button, and selecting `Download Zip` from the dropdown menu. 

If you have Git, you probably don't need any instructions on cloning or forking the repo. 

It is highly recomended you make a backup of your original save file before trying to replace it with one of these. If something goes wrong, you don't want to lose all your progress. 

### Steam

To use these saves on Steam, you just need to locate your existing saved game and overwrite the file `save.dloop` with the appropriate save file from this repo. 

The steam save file is usually located here: 
`%USERPROFILE%\Saved Games\Arkane Studios\Deathloop\base\savegame\<user-id>\SLOT01`

`%USERPROFILE%` is your username on your computer, `<user-id>` stands in for your Steam ID. Once you find the Deathloop save folder inside `/Arkane Studios/`, it's pretty straightforward. 

Remember to make a backup of your save file, then simply drag and overwrite your existing save file with whichever of these saves you wish to use. 

### Game Pass

Transferring these Steam save games to Game Pass is a little more complicated. Luckily, some people have already worked out the kinks. 

You'll just need a file editor, like Notepad++ (not regular Notepad), that can correctly read and save the Null characters in the save game. 

I've linked the original guide below, but in short, you need to open the file in Notepad++, or something similar, and delete the first few lines of text. 

You'll be deleting everything until the characters 'OOD' (non-inclusive), which should follow a string of NULLs. 

Then you'll need to locate your Game Pass save, which by default can be found here: 

`%USERPROFILE%\AppData\Local\Packages\BethesdaSoftworks.ProjectPrism_3275kfvn8vcwc\SystemAppData\wgs\<user-id>\<user-id>\`

There are three files in there. One is a small 1kb file with a bunch of random numbers and letters as the file name, along with a `container.#` file. Ignore both of these. You want the largest file, also with a bunch of random numbers and letters as a name, and missing a file extension.

Backup the file somewhere (that's your save), copy the name of the file, and then drop your modified Steam save (`save.dloop`) file in the save game folder. 

Rename the Steam save to random letters and numbers you copied from the other file name, and make sure you remove the `.dloop` file extension. You may have to change your file explorer preferences so that file extensions are visible. 

Congratulations! Start up Deathloop, and your save file should be successfully overwritten. If it doesn't work for some reason, check out the original guide below, and remember, you can always drop the backup of your original save back into the save game folder to return to your original game. 

[Here's a link to the guide](https://www.reddit.com/r/Deathloop/comments/xl6snh/guide_transfer_steam_saved_game_to_game_pass/)

[And an archived link](https://web.archive.org/web/20230317100708/https://www.reddit.com/r/Deathloop/comments/xl6snh/guide_transfer_steam_saved_game_to_game_pass/)

Although the guide suggests copying over the files `title.data` and `steam_autocloud.vdf`, it shouldn't be necessary to copy those over—just the main `save.dloop` file.

## Additional Details

This section exists just to provide some background and my reasoning for various choices I made collecting these saves. 

My original motivation for these save files was to have a Colt with an organized inventory that need never use Residuum for anything ever again. 

Admittedly, things may have gotten slightly out of hand. 

### Protect the Loop

The save files for each section of the game contain invasion modes in various stages of completion. Players who want their save files to have a win/loss ratio that's 100% theirs have the option to start fresh, and those who would rather have everything unlocked can do that too. 

The online experience can be challenging at times, and many would prefer not to engage with it, or at least not work through Julianna's level-locked loot system. For those of you who want access to Colt's skins without suffering the travails of rubberbanding, the level 70 Juliannas provide that option.  

Additionally, I included two versions of a fresh Julianna. The post-cutscene save file has some desirable starting gear to give players who like to level their Juliannas an easier start, as well a guaranteed black/grey Echolocation gun.  

However, the random starting gear and the order of the unlocks is not predetermined on a save file like Colt's codes are. For those who might want to expirement with rerolling Julianna's starting gear, or just want to be able to access the opening cutscene again, I also included pre-cutscene Juliannas alongside the post cutscene level 1 Juliannas. 

### Sorted Gear

The biggest reason I started these save files is because I like my trinkets and weapons sorted. There were two obstacles to this. 

Firstly, although the infusion menu offers the ability to sort weapons and trinkets by all sorts of filters, when you actually go to equip any of your gear it's sorted only by oldest to newest. Thus, in order to have a sorted list, I had to pick up the gear in the order I wished it to appear. 

Secondly, I encountered a bug where deleting items from my inventory scrambled the sorting of my gear in unpredictable ways. As a result, while creating these save files I could never risk deleting anything, lest my work be undone. You may or may not encounter this bug, but having these save files means you can always go back if it does happen to you.

### Weapons

The weapons included and their sorting is based primarily on my own aesthetic taste.  

While the original plan had me collecting a relatively small number of weapons, I ended up deciding to include every weapon perk and most skins. There are 168 weapons in total, which makes scrolling to find a specific weapon inconvenient. The option to sort by weapon helps with this, but isn't a perfect solution. Ultimately I would rather have a lot of weapons than miss out on some and regret it. 

I simply will not tolerate the orange Limp-10s, and have chosen to exclude them entirely from the collection. The white Constancy is on thin ice. 

Some weapons (like the shotguns) come in every skin, while others (like the Rapiers) have some perks in both skins and other perks in just one. Ultimately, this was down to personal preference and what worked best for my aesthetic arrangement. For example, I like to switch between the blue and green skins for the Explosive Rapier, but rarely make use of the Boomreef Rapier and so included only one skin for it. 

The most difficult to obtain skin in the game is the black Time Sensitive Heritage gun. This perk is not accessible to Julianna, so it must be found by Colt in the wild. I was unable to get it to spawn and so in this collection it is violet. 

In general, weapon skins are tricky on Colt. Many weapons that remain in the same place through multiple times of day will change their skins. Examples include Fia and Charlie's weapons and the Lights's Out Spiker—though the Echolocation gun is inconsistent at this. However, some weapons are only available once in a day. Some, such as the Silver Bullet Rapier, appear to occur in their rarer variety the very first time you encounter them. Others, like the Heritage, seem to only show up in one skin. It seems that the developers wanted Colt to be able to find each skin of a weapon, but if there is some secret (other than getting Julianna to drop one), I don't know it. 

### Personal Trinkets

Personal trinkets are sorted by type, and then arranged so that the golden trinkets and exemplar counterparts are prettily arranged. 

My plan was to leave the game entirely unplayed for the `Mid_Game_Save` files. Unfortunately, several Colt-exclusive trinkets meant I could not rely on Julianna—I had to go find those trinkets myself. 

One Colt-exclusive is found in Frank's fireworks container. The Survivalist trinket is only acquirable from Wenjie in the evening—she has to be invited, which means following her lead, talking to 2-Bit, reading some documents, etc. 

And of course, the Vampire trinket, offically patched out of the game, can only be acquired by killing your alternate self inside the RAK hangar or Karl's Bay bunker. 

[Here's the guide to that btw](https://www.reddit.com/r/Deathloop/comments/yjah8b/vampire_hunting_for_fun_and_profit_or_how_i/)

However, I held off on pursuing these objectives until after collecting all the slabs, weapons, and weapon trinkets. If you want to play through those sections of the story for some reason, they are still accessible in the `Mid_Game_Saves` that don't include the complete inventory of personal trinkets. Of course, many Julianna conversations have unavoidably played by that point, so to access the completed content in these saves simply starting from the tutorial may be a better option.

### Reference Files

To build these save files I needed to create some organization. The `Reference_Files` folder contains the max rank Juliannas I used to build out my weapon collection, as well as the spreadsheet where I kept my neatly sorted lists of weapons, trinkets, notes, cassettes, minicom logs, and profiles. 

There may be some out there who find the information useful, or wish to build their own collection, organized differently, and would appreciate a place from which to start.

### Colt Facts

Here are some fun facts about Colt this playthrough:
* Colt has lived through 232 days of the loop in the mid game `slabs_weapons_weaponTrinkets` saves (including the tutorial)
* Colt has lived through 358 days of the loop in the mid game `complete_inventory` saves
* Colt has lived through 386 days of the loop in the `End_Game_Saves`
* Colt has never been detected by any eternalists through the `Mid_Game_Saves`, except for the one time nessecary for the Vampire trinket.
* Colt never kills any eternalists through the `Mid_Game_Saves`
    * The infusion mission can be completed by sneaking through the level with the harvestamajig and collecting residuum from random items rather than Wenjie's corpse ([yes this was quite difficult, especially as I did it without any slabs or trinkets other than Springheeled](https://www.youtube.com/watch?v=cP_Ty-GEGB4))
    * Almost all gear was collected by a friendly suiciding Julianna
    * Julianna did also kill some individuals for me—most notably Gabe the Garbage Collector (the Fugue slab must be found and does not drop from Julianna until found) and Wenjie (who holds the Survivalist trinket)
    * The last word Colt hears in an audio log is "Goodbye". It's said by Lila Blake. 

## Contributing

Contributions to this repository are welcome. 

Some potential ideas:
* Adding instructions for using these save files on other platforms
* A collection of saves pre-edited to work with Game Pass
* Adding a save file with a shorter-to-enter code than A220
* Your own collection of guns, ordered in the way you like
* Documenting every passcode in this version of the game in the `deathloop_inventory.ods` file
* Edits or additions to my `deathloop_inventory` spreadsheet

If you feel motivated and want to contribute, submit a pull request! 

--- 
