# Roguelike

## Canonical game repo URL:

https://github.com/dannystirl/CS-1666-Project 

## Team Members
* Advanced Topic Subteam 1: Procedural Generation 

	* Daniel Stirling
		* Pitt ID: dgs36
		* Github Username: dannystirl
	* Marshall Lentz
		* Pitt ID: mal341
		* Github Username: MAL341
	* Yihua Pu
		* Pitt ID: yip11
		* Github Username: YihuaPu
	* Joshua Friedman
		* Pitt ID: jmf206
		* Github Username: jofried206

* Advanced Topic Subteam 2: Physics engine

	* Adam Wachowicz
		* Pitt ID: Amw298
		* Github Username: Amw298
	* Zirui Huang
		* Pitt ID: zih17
		* Github Username: angel4576
	* Davon Allensworth
		* Pitt ID: dja52
		* Github Username: davon-allensworth
	* Victor Mui
		* Pitt ID: vim43
		* Github Username: victormui

## Game Description

The game will be a Top-Down Roguelike shooter game with 8-directional movement. The player will be a slime that can absorb abilities, and will navigate through a procedurally generated set of rooms to find and defeat a boss using the weapons and abilities they obtained along the way. There will be 3 levels of the dungeon, each level getting larger and more difficult. Each level will contain a random number and layout of rooms, an upgrade shop, and random items or upgrades for their character. Enemies will drop gold the player can spend in the shop. The player will be forced to think consciously and intelligently about where to travel in the level, which abilities to absorb, how to unlock secret rooms, and how to fight the boss. 



## Advanced Topic Description

### Procedural Generation

Description: The procedural generation team will implement this idea to generate random maps to make each dungeon run a bit different from each other. Each level will have 10-20 playable rooms, a shop and/or healing room, and a room to the next level or final boss room. Each room will have at most 4 doors (including the entrance) to another room, a random number/types of enemies, and a possible item or upgrade. Our current plan is to use something similar to  [this](http://www.roguebasin.com/index.php?title=Dungeon-Building_Algorithm#The_algorithm) algorithm to build the dungeon and [this](http://www.roguebasin.com/index.php/Template_Dungeon_themeing/generation) algorithm to fill each room with enemies, items, and obstacles. 
    
### Physics Engine

Description: A physics engine which will simulate rigid body physics with friction, mass and force. There will be barrels that explode and send shrapnel that bounces off of objects and deals damage based off of the speed they were moving. Depending on the speed of the projectiles the player and enemys might take damage during collision. Some weapons will have projectiles that bounce. In addition explosions and specific weapons will produce knockback. 

## Midterm Goals

* Simplified, non-generated, static test stage. Rooms on this stage will be 20 tiles x 10 tiles, with each tile being 64 pixels. The player will be able to fight through the level and find the entrance to the next level, although since the test stage stands alone, the entrance to the next level will be non-functional.
* Sprites (Player + Enemies) displayed on screen
    * 2 simple obstacles such as barrels and crates. 
    * 1 ranged and 1 melee enemy type
* Implement a health/damage system, allowing the player to take and deal damage. Upon losing all health, the run will end and they’ll lose any items gained during the run. 
* Display a HUD that contains:
    * Currently equipped weapon and abilities
    * Character health + mana (ability energy) bars
    * Currently held gold (currency)
* Base-level abilities functional:
    * Character melee attack that damages enemies
    * Enemy melee and ranged attack that damages character
    * One fireball ability that damages enemies
 


## Final Goals

* 10% 2-3 weapons and abilities and 5 enemies
* 15%: Implement a mechanic where when an enemy is destroyed the player can acquire abilities or stat buff by “absorbing” them. This buff will be different depending on the type of enemy. Simply, the enemies bodies will be items after destruction.
* 10% Create a set of diverse rooms the player can explore. For example, regular rooms with enemies, a shop/healing, a room to the next level, and a boss room. We will use a variant of [this](http://www.roguebasin.com/index.php/Template_Dungeon_themeing/generation) algorithm to fill each room with enemies, items, and obstacles.
* 15%: Implement procedural generation for the rooms and levels. From a starting room, players will be able to search through a web-like map to find the boss. Each room will have at most 4 doors, and the layout will be generated using a variation of [this](http://www.roguebasin.com/index.php?title=Dungeon-Building_Algorithm#The_algorithm) algorithm. 
* 10%: Add the rigid body physics collision and force vector simulation. Create 2-3 objects that the player can push around such as a box or debris. 
* 5%: Add mass and friction values to all objects which will have physics
* 10%: Add projectile inertia ricochet/bouncing and explosive barrels that create projectiles/bounce and deal damage. Add bouncing to one of the weapons projectiles. 


## Stretch Goals

* Add in a “Warrior” slime class (as opposed to the standard “Jelly” class) which does 10% more damage with attacks but has less mana and health. Also, has a unique starting ability to the class. (Other classes will follow the same format of +stat, -stat, and unique skill).
* Add a persistent currency that carries over between runs. The currency can be used to unlock items such as hats that give starting stat modifiers, new abilities, or more powerful weapons. There will be approximately 3 hats and 1-2 alternative starting weapons and abilities. 
