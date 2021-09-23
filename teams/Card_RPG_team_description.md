# Card RPG

## Canonical game repo URL:

https://github.com/Jake-Bon/card-rpg

## Team Members
* Advanced Topic Subteam 1: Enemy AI

    * Emilio Filippi
        * Pitt ID: eaf53
        * Github Username: emifi
    * Louisa Li
        * Pitt ID: lol25
        * Github Username: Xiao-Suda
    * Max Niederer
        * Pitt ID: man153
        * Github Username: maxniederer
    * David Bieler
        * Pitt ID: dab285    
        * Github Username: davidrbieler

* Advanced Topic Subteam 2: LAN Network Multiplayer

    * Derek Halbedl
        * Pitt ID: djh118
        * Github Username: DcaveDerps
    * Jacob Bonhomme
        * Pitt ID: jcb169
        * Github Username: Jake-Bon
    * Merrick Johnston
        * Pitt ID: mmj40
        * Github Username: zimores321
    * Gabriel Balannik
        * Pitt ID: gib24
        * Github Username: GBalannik

## Game Description

* A card battling adventure game where you, the pirate captain, strive towards the goal of conquering the seas. Explore the world and fight foes along the way.
* Ships battle each other in a turn-based system using themed cards until one emerges victorious.
* Each card allows the caster to attack, defend, heal themselves, or inflict a status effect.
* Some cards are designed to synergize well together, leading to devastating combos.
* The player moves around an overworld, traveling the seas to move to and from a few key locations.
* The overworld will be populated by NPCs, which the player can talk to or battle.
* The size of the overworld will be twice as wide and tall as the game’s window, and the camera will scroll to allow the player to explore all of it.

[Concept Art](https://imgur.com/a/WP2DnC6)

## Advanced Topic Descriptions

### Enemy AI

* Each opponent will have their own specially crafted deck, usually revolving around some sort of mechanic or gimmick, and will need to be able to pilot it effectively. This means they will need to be able to recognize combos and be able to play them correctly at opportune moments, while also responding to the player’s cards in the correct ways. AI will pick a move using Minimax with Alpha-beta pruning.
    
###  LAN Network Multiplayer

* 2-Player PvP, instanced battles with friends over network.

## Midterm Goals

* Playable Combat System
* Each player will have a deck size of 20 cards
* Starting hand size of 5, max hand size of 7
* Drawing/Synergistic attack mechanics
* Mana/Energy management
* Win/Lose conditions - Namely HP or running out of cards
* Assortment of cards
    * 4 standard attack cards
    * 2 status attack cards
    * 3 defend cards
    * 2 heal cards
    * 2 distinct status effects
* Scripted Enemy
    * There will be a scripted boss fight. This fight will simply show how the combat system will work.

## Final Goals

* 25%: Card Based Battle System
    * Battle system should function without issue - The system of utilizing cards should be understandable and functional, while all traditional battle elements (win/lose conditions, hp/energy etc.) should work as expected.
    * Expands on midterm goals, now with:
      * 12 standard attack cards
      * 6 status attack cards
      * 7 defend cards
      * 4 heal cards
      * 3 distinct status effects
      * Only 2 or 3 attacks will be synergistic (examples include cards that improve as more cards are discarded, cards that bump up attacks of subsequent cards, etc.)
    * If a player wins a battle, they will also receive one card from the enemy’s deck.
* 5%: User Interface (Menus, etc)
    * Battle interface - HP and energy displays, card display, status information, and button to end turn
    * Main menu - Start, options
    * Pause menu - Options, quit
    * Options menu - Volume settings
* 10%: Overworld
    * Overworld should be at least 2x2 game windows in size, or 1440x1440 px, assuming a 720x720 px window size. It should be populated with structures and NPCs. The map should have bounds, and the player should not clip into structures or NPCs.
* 17.5%: Enemy AI
    * The AI will have effective strategies that will become more difficult for the player to win against as they battle more and more opponents. As stated in the advanced topics, enemies will be able to adapt their strategy depending on how the player’s turn unfolds.
* 17.5%: LAN PVP Battle Mode
    * There should be little to no latency between players when playing cards. The game instances should be able to send battle information back and forth. 

## Stretch Goals

* Second Map - Same size as first map with new layout. Due to asset scope, the enemies in this section may be reused for rematches. This map’s difficulty will be boosted somewhat as to scale with the player’s adventure.  
* Advanced Card Engine - Implement mulligan system, card graveyard(can recover/reuse cards from the discard pile, possibly have cards that utilize the number of cards discarded (like increasing attack power or something of the sort)), 2 new status effects, and 10 new cards to balance the updated system 
