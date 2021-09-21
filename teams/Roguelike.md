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
The game will be a Top-Down Roguelike shooter game with 8-directional movement. The player will be a slime that can absorb abilities, and will navigate through a procedurally generated maze to get to a boss. The hud will display the player’s current health, mana, and gold. There will be 3 levels of the dungeon, each level getting larger and more difficult. For each level, there will be a boss room, some obtainable upgrades. and a maze of rooms that have enemies, or upgrades. The player will be forced to think consciously and intelligently about where to travel in the level, which abilities to absorb, how to unlock secret rooms, and how to fight the boss.



## Advanced Topic Description

### Procedural Generation

Description: The procedural generation team will implement this idea to generate random maps to make each dungeon run a bit different from each other. This will make it so that the game feels more dynamic to the player.
    
### Physics Engine

Description: A physics engine which will simulate rigid body physics with friction, mass and force. There will be barrels that explode and send shrapnel that bounces off of objects and some weapons will have projectiles that bounce. In addition explosions and specific weapons will produce knockback. 

## Midterm Goals

* Fully playable, simplified first stage, the first stage will be 20 tiles x 20 tiles, with each tile be 64 pixels
* Sprites (Player + Enemies) displayed on screen
    * 1 simple barrel, 1 enemy
* Implement a health/damage system
* Display a HUD that contains:
    * Character health + mana bar
    * Currently equipped weapon and abilities
    * Currently held gold (currency)
* Base-level abilities functional:
    * Character melee attack that damages enemies
    * Enemy projectile attack that damages character
 


## Final Goals

* 10% 2-3 weapons and abilities and 5 enemies
* 15%: Implement a mechanic where when an enemy is destroyed the player can acquire abilities or stat buff by absorbing them
* 25%: Implement procedural generation
* 10%: Add the rigid body physics collision and force vector simulation
* 5%: Add mass and friction values to all objects which will have inertia
* 10%: Add projectile ricochet/bouncing and friction and barrels which explode sending objects which bounce and deal damage. 


## Stretch Goals

* Add in an extra warrior class which does 10% more damage with attacks but has less mana and health. Also has a unique skill to the class. (Other classes will follow the same format of +stat, -stat, and unique skill).
* Add a persistent currency for unlocks that carries over between runs such as hats that give starting stat modifiers and a more powerful starting weapon.

