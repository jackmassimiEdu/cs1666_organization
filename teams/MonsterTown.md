# Monster Town

## Canonical game repo URL:

https://github.com/ZHZ110/cs1666-Team-monster_town

## Team Members
* Advanced Topic Subteam 1: Procedural Generation

	* Zhiyi Zhan
		* Pitt ID: zhz110
		* Github Username: ZHZ110
	
   	* Gurmail Mathon
		* Pitt ID: gsm18
		* Github Username: gmathon18
	
* Advanced Topic Subteam 2: Advanced AI

	* Azeez Hakeem
		* Pitt ID: azh15
		* Github Username: itsyourOOP
	
  	* Adam Wipprecht
		* Pitt ID: amw290
		* Github Username: wippra
	
  	* Burhan Bhatti
		* Pitt ID: bub3
		* Github Username: bhattiburhan3

## Game Description

Our game seeks to be a recreation of an older style Pokémon game. It would feature
the following basic things that go into one of these games: Turn-based battle and a ﬁxed, navigable overworld map for the user to explore

## Advanced Topic Description

### Procedural Generation

Wild monsters appear on the map in spawnable areas according to their type. They each has an assigned spawnable rate. We use random number generator to decide 
whether they can spawn or not.
Each gym contains a perfect maze. There are three mazes in total: two smaller mazes and one final larger maze. They are all going to be generated using eller's 
algorithm. The first maze is 9 passage(length) x 6 passages(width). The second is 16 x 9 passages, and the final maze is going to be 20x16 passages. Each passage
has the width of 1 block, the same as the wall, which covers the edge of the maze, so it's going to be one block more than the passage. Each block contains 16
pixels. The maze sizes will depend on the number of passages/walls.

### Advanced AI

The advanced AI is used for turn-based battle strategy. The player has 6 monsters in total for their party. Each has different skillsets and levels. The skillsets
contain skills that attack/reduce receved damage/add additional blocking/regen. Each skill and monster has a type, which has an impact on their defense and damages. 
Each battle is independent. The enemy AI will take into account the health, overall level and all the factors mentioned before, in order to make the optimal
decisions. It will also be able to switch monsters to get the best battle results when it comes to NPC trainers.

## Midterm Goals

* UI for a basic map is complete, which contains a single colored background and all the essential entities. The entities include four gyms, a pokemon center, and 
  a home entity. The entity will have simple coloring. Overworld map is going to be 80 x 45 blocks. Each block contains 16 px, which is also the size of the player 	character. 
* Artwork for the expected portions of the open-world map and monsters must be completed based on team member assignments.
* NPC trainers are scattered on the overworld map. They will be either standing still or moving back and forth. If the player approaches them, it gives the option
  to either battle or bail. The NPC players are all given random pokemons with uniform levels. The battle strategy is going to be random.


## Final Goals

* 20%: Turn-based battle system: 
  5% skill set design for each pokemon complete, 
  5% for UI, 
  10% for actual damages based on defense level and type
* 15%: A navigable overworld to explore: Road, home, pokemon center, gyms, spawnable places, final maze entry complete.
* 20%: The gyms within each town will contain mazes that the player must maneuver and reach the leader of the gym
* 20%: The enemy AI is able to take into account the factors mentioned above, and make the decision accordingly.


## Stretch Goals

* Monsters in the player’s party will gain experience points towards leveling up, therefore increase skill damage and be able to learn new skills. 
  The level of the enemy player will increase as the player navigate deeper into the map.
* The player would have the option to choose a difficulty based on the overall level of the enemy.
