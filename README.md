# Easier-items-datapck
![Github license](https://img.shields.io/github/license/NoComment1105/upgrade-everything.svg)
![Github Issues](https://img.shields.io/github/issues/NoComment1105/upgrade-everything.svg)
![Github Tag](https://img.shields.io/github/tag/NoComment1105/upgrade-everything.svg)
[![Discord Chat](https://img.shields.io/badge/Chat%20on-discord-7289DA)](https://discord.gg/28N2Eeq2tT)

Upgrade all tools/armour/weapon in the smithing table

### What is the purpose of this datapack?
You can get a lot of tool drops from Minecraft mobs. and usually they come on iron or gold tools/weapons/armour; and that can be a pain becuase it  renders then useless usually. But this pack here allows you to put any tool/weapon/armour piece in the smithing table and upgrade it to the next level


### Features
1. Inserting a Wooden item into the smithing table and adding a block of cobblestone returns a stone item
2. Inserting a stone/chainmail item into the smithing table and adding a gold ingot returns a gold item
3. Inseting a gold item into the smithing table and adding an iron ingot returns and iron item
4. Inserting an Iron item into the smithing table and adding a diamond return a diamond items
5. *NETHERITE RECIPE IS UNAFFECTED*

### The Developers

| Author   | Role   | Links   |
|:---------|:-------|:--------|
| NoComment1105 | Pack Lead | [Contributions](https://github.com/NoComment1105/Easier-items-datapck/commits?author=NoComment1105) |
| doglol99 | Pack Assistant Lead | [Contributions](https://github.com/dabigaaa/Easier-items-datapck/commits?author=doglol99) |

### Versioning
This pack is 1.16.x at it's oldest. I am **NOT** going to back port any of these changes to any other versions
I will try my hardest to updates this pack, in its latest release at the time, on the day of the next version release and will add further features as i get a chance to evaluate the difficulty of the new items

### Compiling / Using this pack
If you choose to download the .zip of this repository, to correctly use this pack you need to do a couple of things
1. You need to separate upgrade_everything_vx.x from the rest of the .zip
2. Compress upgrade_everything_vx.x into a .zip file itself
3. Put into your data packs folder in your Minecraft save/server files and you're ready to use
## Contributing to this repo
If you want to contribute to this repo just follow the following steps
1. fork this repo
1. clone the repo to your local machine
1. set up a symbolic link so you dont have to keep copying the datapack to and from the datapack folder in your world saves. (the following method only works on windows and requires admin privaleges) (for more info just google symbolic link)
	1. search for command prompt
	1. right click command prompt
	1. click run as administrator
	1. windows may ask you if you want to allow command prompt to make changes to your device. If so allow it to.
	1. type `mklink /J "C:\Users\USERNAME games\AppData\Roaming\.minecraft\saves\MINECRAFTWORLDNAME\datapacks\upgrade-everything" "C:\PATH TO REPO CLONE LOCATION\upgrade-everything\upgrade_everything_v0.1"`
1. create the modifications you want
1. add yourself to credits
	1. create a new file with the name USERNAME.json (replace USERNAME with your username)
	1. paste the following code into it
```json
{
	"display": {
		"title": "USERNAME",
		"description": "",
		"icon": {
			"item": "minecraft:player_head",
			"nbt": "{SkullOwner:{Id:[I;0,0,0,0],Properties:{textures:[{Value:'SKIN URL'}]}}}"
		},
		"background": "minecraft:textures/block/black_concrete_powder.png",
		"show_toast": false,
		"announce_to_chat": false,
		"hidden":true
	},
	"parent": "no_comment_datapacks:easier_items",
	"criteria": {
		"trigger": {
			"trigger": "minecraft:impossible"
		}
	}
}
```
5.
	3. replace USERNAME with your username
	1. go to https://mcuuid.net/
	1. input your minecraft username
	1. copy your trimmed UUID
	1. go to https://sessionserver.mojang.com/session/minecraft/profile/TRIMMED_UUID (replace TRIMMED_UUID with your trimmed UUID)
	1. there should be a line that says '"value" : "LONGLISTOFRANDOMCHARACTERS"'
	1. copy the long list of random characters
	1. replace SKINURL with this long list of random characters
	1. save the file
1. commit your changes
1. create a pull request
