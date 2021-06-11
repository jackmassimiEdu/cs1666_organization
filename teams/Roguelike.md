# Rogue-Like (Blob-Like)

## Canonical game repo URL:

https://github.com/CS1666-RogueLike/roguelike-repo

## Team Members
* Advanced Topic Subteam 1: Procedural Generation

	* Joe Cavanaugh
		* Pitt ID: joc133
		* Github Username: joecavanaugh27
	* Trae Yelovich
		* Pitt ID: tay31
		* Github Username: tay31
	* Tyler Sheinberg
		* Pitt ID: tys25
		* Github Username: tys25
	* Jagr Krtanjek
		* Pitt ID: KJK110
		* Github Username: jeepy33

* Advanced Topic Subteam 2: Advanced AI

	* Dan Rothman
		* Pitt ID: der57
		* Github Username: Dan-Rothman
	* Keyon
		* Pitt ID: keh204
		* Github Username: keyonzi
	* Connor Halloran
		* Pitt ID: cjh138
		* Github Username: connorjohnhalloran

## Game Description

Level is generated grid-based and character/enemies operate off of grid.   The character can move in numerous directions, with WASD, at one base speed. No vertical movement.  Defeating enemies will be damage-based; once you bring their health to 0, they die. Each room will have enemies, locking the doors upon entering - the player must kill all of the enemies to leave the room. Enemies will consist of 3 different types, each correlating with the statistics that the player has: health, speed, and attack damage. The player will also have the ability to obtain and use consumable items such as a health potion or buff potion to improve their statistics.
General Goal: Explore rooms of a dungeon to get to the next level, then reach the final boss to win
Other Gameplay Information:
Player has 3 stat bars: Health, speed, attack damage
Killing an enemy last in a room adds a stack to its associated bar
Once enough stacks are reached, player gets permanent buff
Player goes through rooms looking for key to next floor exit
Attack: short range melee and charged range attack
WASD to move character, Up Down Left Right to attack in each direction
Player has to complete three floors
Art style is pixel art with only black and white with colors denoting enemy buff type



## Advanced Topic Description

### TOPIC1 Procedural Generation

Level/floor is generated grid-based
Our procedural generation implementation will be mostly based on the level layout.  Room generation will be random in some aspects and also part of the procedural generation . 
Levels will be 8x8, but not every room is filled.
Rooms will be 9x15 tiles (16x16px, 1x1 internal representation)
Implementation Plan: (possible algorithms)
Recursive DFS/Prim’s with modifiers.
Potentially using a modified maze algorithm for the level.  
Perlin noise/ white noise (or a different algorithm) can be used to generate random numbers; use said numbers to determine tile positioning based on specified intervals.  Could be used for room generation

    
### TOPIC2 Advanced AI

How the enemies move and attack.  Will be based on character stats/ level/character behavior, enemies working together
Implementation Plan:
Enemies coordinate attacks based off of other enemies
React based off of player stats and player health
-Low health
Responds to player action
-Charging up attack
-Running away
-Focusing an enemy
-Each enemy will have a unique decision tree


## Specific milestones
Gameplay mechanics to implement:
Hearts system with extra regenerating shield heart
Rooms are generated on a grid system, but the rooms and floors are individually procedurally generated.
Absorbing enemies for buffs
Different types of enemies, each associated with a stat increase
Last enemy that is killed gets absorbed and transformed into stat bar progress
Health buff fully heals the player and gives a temporary heart if below full health and gives another permanent heart if at full
Speed upgrade
Attack damage
Attacking
Short-ranged attack and charged long-range, melee
Rooms lock upon entry and unlock when you defeat the last enemy

Scope of the game:
3 floors
Three colors of enemies, each color with a 2-3 enemy types, each enemy unique and not shared between colors

Advanced topics milestones:
Procedural Generation:
Generates completely empty level
Generation of a single room working
Successfully generate level that fully connects with "correct" tile placement
Advanced AI:
Gets single reactive AI in the room
Gets multiple AI to coordinate
Enemies react as expected for each gameplay scenario

## Midterm Goals

* Test rooms used to demonstrate mechanics 
* Player model moving/ interaction/ attack
* Character can attack and kill enemies
* Enemy models moving/ attacking
* 1 enemy for each stat type designed
* Final enemy is “absorbed”
* Character able to die
* UI is complete

...

## Final Goals %75

* 15%: 3 levels procedurally generating
* 5%: Character can enter new rooms
* 10%: Enemies coordinate attacks based off of other enemies
* 10%: Enemies React based off of player stats and player health
* 15%: Enemies Respond to player action
* 10%: Doors lock until all enemies are defeated
* 10%: Final mob in room defeated drops buff/ buffs correctly add

## Stretch Goals

* Final boss for the game with advanced AI based on player stats
* Complex consumables (bomb blowing up door?), procedurally generated per floor or an upgrade room

