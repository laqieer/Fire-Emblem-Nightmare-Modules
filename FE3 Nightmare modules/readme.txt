Hello!
This a nightmare module pack used for editing FE3!
This can be used with the lastest translation patch, or even with a vanilla FE3 rom. Make sure the ROM has a header!
The pack has been created using a bunch of docs on the FE3 rom created by the japanese community, without them this wouldn't be possible.
Also credits to the original creators of the english modules first available on the FEShrine, and P33RL355 in FEU for updating it in 2018.

Contents:

->Chest and Buried Treasure Editor
You can edit the contents of a buried treasure (ex: Like in desert maps, waiting in a certain tile can reward you a item), what chapter it appears in, and where it is.
There is not much information on chests, but you can edit some items. Some of them for some reason has a different byte that doesn't change for a bunch of entries, 
and some weird items like the Falchion are present, even though you don't get them from a chest.

->Event Tile Editor
Edit where houses, stores, arenas, villages, seize points, doors, bridges, chests and secret shops are in the map, and their restrictions.

->Support Editor
Without repointing anything is possible to create new supports, while not replacing the old ones. Basically, the game stops reading the support list when it reaches a 0xFF byte,
so just make sure that aren't any blank support entries between the start and the end.
Supports uses names to identify which character it is, so for example, if the name Sedgar supports Hardin, that still will happen when he is a enemy in book 2, since
he uses the same name as the book 1 Hardin.

->Astral Shard editor
Edit the growths bonuses of the Astral Shards. Pretty simple.

->Arena Weapon Editor
Edit what weapons that can be used in the arena per class.

->Map Data Editor
Edit the tileset, color, X size, Y size of the map.
Also edit if the map is Outdoor/Indoor and the enemy classes.
Classes past 1D will display messed up sprites unless they are in this list!

->Death Quote Editor
Change the pointer of dialogue that a character uses when they kick the bucket. Also change the flag check.

-> Enemy Recrutable Character Editor
Change what character recruits and what character is recruited via talking while it is a enemy.
Ex: Caeda recruits Castor if she talks to him while he is a enemy.
Also change the map in what this can happen, event flag condition and event number.

------ Changelog ------
v1.0

- This started existing. Yay!
- Fixed wrong pointer in the Astral Shard module.