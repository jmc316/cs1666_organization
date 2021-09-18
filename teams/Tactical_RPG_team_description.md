# Team Castle Quest

## Canonical game repo URL:

https://github.com/KalebRaymond/CS1666-Tactical-RPG

## Team Members
* Advanced Topic Subteam 1: AI

	* Kaleb Raymond
        * Pitt ID: 4268953
        * Github Username: KalebRaymond
    * Alexander Kwiatkowski
        * Pitt ID: 4363559
        * Github Username: AlexKwi
    * Colin Woelfel
        * Pitt ID: 4352147
        * Github Username: cjw102
    * Jared Carl
        * Pitt ID: 4190195
        * Github Username: jmc316


* Advanced Topic Subteam 2: Networking

	* Bianca Finamore    
        * Pitt ID: 4297373
        * Github Username: BiancaFinamore
    * Jake Baumbaugh
        * Pitt ID: 4180882
        * Github Username: JakeBaumbaugh
    * Shane Josapak
        * Pitt ID: 4266181
        * Github Username: shjosa
    * James Fenn
        * Pitt ID: 4262575
        * Github Username: fennifith

## Game Description

Castle Quest is a tactical RPG in the same style as games like Fire Emblem and Advance Wars.

* Grid-based Tactical RPG across one large map
    * Top-down view, at least 48x48 tiles
* Opposing teams start in opposite corners of map near their team's castle
* Third, AI-controlled team (barbarians) located throughout map in small groups
    * Either the player or the enemy can defeat them to gain additional party members
* Each team (player 1, player 2/enemy AI, and barbarians) takes turns with the ability to move and attack opposing units within attack range
* Game continues until either player or enemy defeats the other
    * Defeating all of the other team’s units (Total Party Kill)
    * Capturing the other team’s castle (Placing a unit on their castle for three consecutive turns)
    * Barbarians do not contribute to win/lose conditions


## Advanced Topic Description

### AI

* Simple implementation for barbarians (melee and ranged with no magic)
    * Pursues ttacks any non-barbarian unit that comes into aggro range
    * Otherwise remains idle
* More complicated enemy AI for singleplayer (melee, archer, and magic)
    * Enemy AI must decide between pursuing the player or attacking barbarians to gain additional units


### Networking

* Upon selecting the multiplayer game mode from the menu, the player will be able to enter a server join code.
* When two players have connected to a server, they will enter a game on opposite sides of the map where they will try to defeat the other player.
    * The second human player replaces the enemy AI of the singleplayer mode 


## Midterm Goals

* Single player: starting the game spawns players, enemies, and barbarian units on 48x48 map
* Basic movement implemented for player and barbarians
    * Player: Clicking on a unit and then clicking on any tile teleports the unit to that tile. After moving, a context menu appears that allows you to end the unit's turn.
    * Barbarian AI: If at least one player unit is within a certain range, barbarian units will move towards the closest player unit. Otherwise, the barbarian unit will not move.
    * Enemy team will simply skip turn
* Implement basic turn order functionality
    * Turn order goes player -> enemy AI -> barbarians, continues indefinitely 
    * “End turn” button for player skips remaining units & continues the game
* Multiplayer room creation and joining
    * Successfully joining the room alerts both players


## Final Goals

* 20% - Completed AI for enemy team & barbarians
    * Barbarians roam within a small radius until a player or enemy enters within their aggro range, upon which, depending on unit type and number of other barbarians, the barbarian will pursue the player/enemy and attack them
    * Enemy AI will be more advanced. Enemies should choose whether to prioritize attacking barbarians that are out of the way versus going directly for the player.
* 20% - Functioning multiplayer
    * Joinable rooms with keys
    * Communicate turn order & character actions
    * The winning team receives a win message, while the loser receives a lose message
* 5% - Implement archer and mage classes for player and enemy teams. Implement archer for barbarian team
* 5% - Complete map design with all objectives (player/enemy castles, obstructions, predetermined barbarian spawnpoints)
* 5% - Additional unit spawning
    * After killing a barbarian, there is a random chance that the player will receive an additional unit spawned at their castle
    * Player can choose which class that unit will be
* 15% - Implement combat system & user interaction
    * Hovering over player's unit highlights their movement range
    * Clicking on unit and then clicking on a tile in range moves that unit to the selected tile
    * Display the unit’s attack range after moving
    * Add attack button to context menu that allows player to select an enemy unit that is in range and deal damage to them
    * After moving unit, unit is greyed out and cannot be selected again until player’s next turn
* 5% - Implement win & lose conditions
    * Entire team is defeated or player keeps one unit in opposing team’s castle for three consecutive turns


## Stretch Goals

* Additional Classes
    * Two new classes that offer different strategic advantages over other classes, allowing for more varied approaches to combat.

* Additional Objectives
    * Barbarian encampments as well as a central barbarian fort (instead of having lone barbarians randomly placed throughout the map) to allow for more chances to recruit new units
    * Utilizes the same capture mechanic as the player castles
    * When captured would provide some benefit to the player
