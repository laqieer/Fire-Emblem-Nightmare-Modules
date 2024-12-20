Hey there, thanks for downloading my Nightmare modules! Here I'll describe all the new modules I've made as well as a few pre-existing ones that I've just modified a bit.

New Modules:


Character Editors:

	Character Stat Cap Editor - This one lets you modify the personal stat caps for HP/Str/Mag/Skl/Spd/Def/Res/Lck. Unfortunately, increasing them is a bit limited since your personal+class stats still can't go above 30 for practical use, so it's mostly better to use this to lower caps if you wanted to for some reason. When modifying these caps, you change Cap 1 and Cap 2 to the same new value you want, and then Cap + 1 is that new value plus 1.

	Level Cap Editor - This one is similar to the stat cap editor, not very good for increasing the level cap (from what I've read you can bring it up to 33 safely but anything past that will cause issues when relaoded), and as such serves more use if you want to lower the cap.

	Player Character Reload Authority Star Editor - This one lets you modify the amount of Authority Stars Sigurd, Quan, Seliph, Altena, and Hannibal have when you save and reload the game (think about how in base FE4 Seliph goes from 2 to 3 stars upon a reload). Quan, Altena, and Hannibal's stars only matter when they're not player-controlled units, this won't give them stars when they are on your side.

	Seize Editor - This one isn't really a sensible module that should exist, I mostly just made it so if you're deathly afraid of hex-editing you can make it so Sigurd and Seliph seize regardless of their class. Just select the other option in all the dropdowns and you should be set! (I promise hex-editing isn't as scary as it sounds, though, give it a shot!)

	Class Change Screen Portrait Pointer Editor - This one lets you modify the portraits that appear in the Gen 1 and Gen 2 promotion screens. The portrait pointers used here are the same as the ones used in the portrait editor that comes with the original nightmare package.

	Portrait Definition Editor - This one lets you modify where the game looks for graphics data for portraits, which is different from where portraits are assigned to the characters themselves (the Portrait Pointer Editor in the base Nightmare package). This is most useful when you're wanting to add a portrait that would take up too much space to fit in the space of whatever portrait you're replacing. To get the bytes you want to put in the editor, I suggest using Lunar Address and selecting the ExHiROM - PC setting, making sure that "Include $200 Copier Header" is checked if the rom you're working with has a header.

	Combat Palette Definition Editor - This one lets you modify where the game looks for the color palettes used by combat sprites, which is different from where those palettes are assigned to the sprites themselves (Custom Battle Palette Editor and Battle Sprite Editor in the base Nightmare package). This behaves similarly to the Portrait Definition Editor, although now each entry also has a length value assigned to it (1E for 15 colors for palettes for unmounted classes, 3E for 31 colors for palettes for mounted classes). Additionally, the entries in this table are not the pointers used in the mentioned editors (refer to the Combat Palette Re-Index Editor). To get the bytes you want to put in the editor, I suggest using Lunar Address and selecting the ExHiROM - PC setting, making sure that "Include $200 Copier Header" is checked if the rom you're working with has a header.

	Combat Palette Re-Index Editor - This one lets you modify what entry within the Combat Palette Definition Editor the combat palettes refer to. For example, Lene's unique Dancer palette, 0x27, is entry 0x27 in this table, which has the value of 0x21, meaning that palette 0x27 refers to the data at entry 0x21 in the Combat Palette Definition Editor.

Children Editors:

	Seliph Blood Editor - This one lets you modify Seliph's holy blood, since it's hardcoded despite him being a dynamic unit.

	Gen 2 Initial Authority Star Editor - This one lets you modify the amount of Authority Stars that Seliph and Altena have before you reload the game once they exist (like how Seliph starts with 2 stars [unless you've applied the Project Naga patch, which just changed this value to 3]), since they're stored differently from units like Sigurd and Hannibal on account of Seliph and Altena being dynamic units.

	Inheritance Lock Editor - This one is weird and I'd honestly advise against using it just because I haven't had the chance to experiment much with it yet. Unlocking Seliph with this makes it so his Blood is properly determined by his parents (so he'll get Deirdre's minor Loptous blood), and also seems to make him start with no Authority Stars, ignoring the value assigned in the previously described module. I assume Altena's lock behaves similarly, but I haven't checked personally.


Class Editors:

	Terrain Avoid Editor - This one lets you modify the avoid given by all the types of terrain. The first table corresponds to the avoid given to non-flying units, and the second table corresponds to the avoid given to flying units.

	Class Weakness Editor -	This one lets you modify what weapon effectiveness types a given class is vulnerable to. There's even two effectively unused vulnerability types that seem to correspond to Wyverns and Infantry Mages that you can have fun with using this and the modified Weapon/Staff Editors.

	Class Sound Editor - This one lets you modify the sounds used when a unit in each class moves in battle animations.
	
	Class Map Battle Sprite Editor - This one lets you set the sprites used for combat with animations turned off for all classes. This looks scary, but basically you can just swap out all entries from one class for another. For example, if you wanted the map battle sprites for Lance Knight to look like Sword Master's for some reason, copy all the entries in the Sword Master page to the Lance Knight page, and set the Class Type to Infantry (I honestly don't know what the class type designator does, if anything, but I'd just do it to be safe).
	Do keep in mind that using weapon types that sprites were not intended to use can cause issues, so a class you gave the Sword Master map battle sprites to would probably cause issues when using Lances. This does go the other way though, so if you want to give a class access to new weapon types you can use the map battle sprites from a class like Baron or Master Knight to avoid any issues when it comes to animations-off combat.

	Female Map Battle Sprite Editor - This one lets you modify what, if any, sprites are used instead of a class' normal sprites for combat with animations turned off when a unit in that class is Female. With this one, you have to have the class you want to change in the entry corresponding to its class ID, (so if you wanted to make an entry for Social Knights, it would have to be in the very first slot in the editor) or it will have no effect. The sprite IDs here are the ones modified in the Class Map Battle Sprite Editor, so changing them there will change what they appear like when assigned here as well.

	Custom Map Battle Sprite Editor - This one lets you modify the sprites used when a specific unit in a specific class engages in combat with animations turned off. Sadly there's only one entry, which is used for Seliph's custom Lord Knight map sprites, but you can use it for something else if you want to.

	Class Map Receiving Sprite Editor - This one determines the weapon held in the sprite used when a unit is being healed, receiving gold, or in the special glowy animation when they receive a Holy Weapon. Make sure each class uses a weapon type their Map Combat sprites are compatible with, or things will get all weird.


Item Editors:

	Player Weapon Sound Editor - This one lets you modify the sounds used when player characters use weapons.

	Enemy Weapon Sound Editor - This one lets you modify the sounds used when non-player characters use weapons, because it's managed separately for some reason.

	Minimum Damage Editor - This one lets you modify the amount of damage dealt when someone's attack is less than or equal to their enemy's defending stat. If you set it to 0 you even get the little "tink"!

	Weapon Battle Sprite Definition Editor - This one lets you modify where the game looks for graphics data for weapon sprites, which is different from where those sprites are assigned to the weapons themselves (Lorena's Item Sprite Editor in the base Nightmare package). This is most useful when you're wanting to add weapon sprites that would take up too much space to fit in the space of whatever sprite you're replacing. To get the bytes you want to put in the editor, I suggest using Lunar Address and selecting the ExHiROM - PC setting, making sure that "Include $200 Copier Header" is checked if the rom you're working with has a header.

	Weapon Map Sprite Editor - This one lets you modify the sprite and palette each weapon uses in combat with animations turned off. As far as I can tell there is no Definition table for these like there is for Portraits and Weapon Battle Sprites, but fortunately the graphics (stored at $2CCC17 unheadered, being $705 bytes long) are rather poorly compressed, so any modifications you make to the graphics should fit in the original space once re-compressed.



Modified Modules:


Class Editors:

	Class Editor by Camus - This one has been modified to better indicate what all entries in the table correspond to. Most notably are the Promotion-Into Level and Terrain Avoid Type entries. The Promotion-Into Level determines the level at which a class can be promoted into (Note: this is NOT the level at which the class can promote), and the Terrain Avoid Type determines which of the two tables in the Terrain Avoid Editor the class uses to determine their Terrain Avoid bonuses.
	

Item Editors:

	Weapon Editor 1/Weapon Editor 2 - I didn't even really change the module for these, just gave more options for the Critical entry, which determines what effectiveness the weapon has (refer to the Class Weakness Editor for the other end of how to handle weapon effectivess).