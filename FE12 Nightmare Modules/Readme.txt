FIRE EMBLEM: NEW MYSTERY OF THE EMBLEM
HEROES OF LIGHT AND SHADOW
Nightmare Module Collection

This package contains some Nightmare modules for editing Fire Emblem 12.
In order to utilise these, follow the instructions I've shamelessly stolen from Blazer's FE11 modules.

How to Decompile Your Game:

1) Obtain the game. I cannot help you do this.
2) Obtain a program to decompile your game. I recommend DSlazy because it is simple.
If it does not work, make sure you have installed the .NET runtime.
3) Use your program and either load your ROM. For DSlazy, this means using the "..." button on the left side
and choosing your NDS game.
4) Hit "unpack" or "decompile". Wait a couple of minutes for the thing to do it's stuff.
5) Go to the place where the decompiled ROM is. For DSlazy, go to the folder with DSlazy and then go to
"NDS_UNPACK".
6) There are two folders from here. You will almost always use the "data" folder, unless mentioned otherwise.
7) In the data folder are bunch of other folders with tons of files. If this is what you have, then you have successfully decompiled your game. ^_^

Once you have done this, navigate to the next "data" folder and find FE12Data.bin.
This file contains the character, class, and item data. I recommend using BatchLZ77 to decompress this file.
From there, edit the data as you wish. Be sure to recompress and reinsert the file before rebuilding the rom to test the hack.

To use the Chapter Unit Editors, instead navigate to the dispos folder and decompress the file for the chapter you wish to change.


Version History:
25/09/20: Initial release.

I presume this will be the only release of this package, for hope that it will be obsoleted by HeartHero's FE12 tools in development. (https://feuniverse.us/t/accessible-fe12-hacking/9459)

Credits:
Darrman: Assembling this package and editing the pre-existing FE12 modules in the interest of filling in most unknown bytes.
Blazer: Created the FE11 modules which most of this work is ultimately based upon.
Purple Mage: Made some earlier attempts at porting Blazer's FE11 modules to FE12 that these modules were based upon.
VincentASM: Creator of the Chapter Unit Editors. And the translation patch, though that cannot be found here.

Notes:
Blazer has a good amount of notes in his FE11 modules. Some of this can be applied towards FE12 as well.
FE12 growth rates are encrypted; the decryption methods can be found here.
(https://feuniverse.us/t/fe12-growth-cyphers/6380)

Enjoy modifying FE12.
- Darrman