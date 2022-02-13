---
title: 'lang Folder / global.gxt2 files'
date: '02/13/2022 10:49'
media_order: obraz_2022-02-13_134726.png
---

## lang Folder and global.gxt2 files

### What do these gxt2 files do?
> In this case, they are responsible for displaying names instead of hashes/slot names. 
><br> For example if you have a _Police BMW M5_ on `police5` slot, you can make a gxt2 file for it so it will display "_BMW M5 Police_", instead of `police5`.
><br>The same applies for `vehicleMakeName` in vehicles.meta. Lang files are for pretty much everything in the game.

### How do I actually make such folder and files?
> First you need to make a `dlctext.meta` file, and then reference it in content.xml of your RPF file. [Here](http://wafelowski.pl/grav/en/game-setup/lang-folder/dlctext-meta)'s how you do it.
> <br>Then you need a folder to keep RPF files that contain the `global.gxt2` files. Recommended path is `<RPF>/x64/data/lang`
> <br>Now the longest part (technically), making the RPF and gxt2 files.

#### Making the GXT2 file.
Make a `global.oxt` file, yes an `.oxt`, not `.gxt2`. You can do it normally, just like making a `.txt` file Open it with Notepad++/VS Code/Any text editor other than Notepad.
<br>Use this template:
```xml
Version 2 30
{
	0xC52827A7 = Name One
	0x9D8AD861 = Name Two
}
```
On the left side you put Hash generated using Hash Generator in OpenIV using Default Algorithm and Hex format. On the right side you put the name, that should be visible to the user.
<br>That's all for this step.

#### Making a RPF file
You do it the same way as other RPF files, right click with Edit Mode enabled and select `.rpf` file. Here's the list of names (languages) you can use:
* `americandlc.rpf`
* `chinesedlc.rpf`
* `frenchdlc.rpf`
* `germandlc.rpf`
* `italiandlc.rpf`
* `japanesedlc.rpf`
* `koreandlc.rpf`
* `mexicandlc.rpf`
* `polishdlc.rpf`
* `portuguesedlc.rpf`
* `russiandlc.rpf`
* `spanishdlc.rpf`
<br>Each of these RPF files needs to contain a `gxt2` file. How to import it? Inside the RPF, right click on the empty space and choose "Import openFormats" and select the `global.oxt` file.
<br>That's all. There's no need to reference the RPF file anywhere. 

#### Result of our work
`vehicleMakeName` set to _"Opel"_
<br>`gameName` set to _"InsigniaVMS"_
![obraz_2022-02-13_134726](obraz_2022-02-13_134726.png "obraz_2022-02-13_134726")

#### FAQ
- **Can I use the same gxt2 file for each RPF file?** 
<br>Yes
- **Do I have to do all the RPF files?** 
<br>Yes
- **Do I have to include shared names in gxt2 file for each dlcpack?** 
<br>No, if you have two dlcpacks of for example BMW cars, only one of the dlcpacks needs to contain hash of `BMW` if you wish to use it. 
<br>Remember, that you will need to **have both dlcpacks** at the same time to make it work.