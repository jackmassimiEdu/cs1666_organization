# Street Code Fighter

## Canonical game repo URL:

https://github.com/kem243/Fighting-Game

## Team Members
* Advanced Topic Subteam 1: Physics Engine

	* Carly Sills
		* Pitt ID: CPS41
		* Github Username: cps41
	* Kenneth Meier
		* Pitt ID: KEM243
		* Github Username: kem243
	* Nick Pilotti
		* Pitt ID: NSP29
		* Github Username: NickPilotti
	* (Fernando) Zixin Yang
		* Pitt ID: ZIY13
		* Github Username: ziy13

* Advanced Topic Subteam 2: Multiplayer Network

	* Alexis Sanders
		* Pitt ID: ALS429
		* Github Username: als429
	* Ethan Dewit
		* Pitt ID: ERD56
		* Github Username: Ethan-Dewit
	* (Steve) Khairat Ullah
		* Pitt ID: KSU5
		* Github USername: ksu5

## Game Description

Networked multiplayer platform fighter using physics engine to fight with our favorite programming languages. A 
throwback that lets us literally fight it out with our top programming languages. Design will resemble the game 
Street-Fighter while gameplay will resemble Super Smash Bros.

## Advanced Topic Description

### Physics Engine

Physics engine will simulate movement and collisions in a rigid-body format. Basic principles of kinematics will be applied for interactions to allow movement on an XY plane. This includes concepts such as gravity, momentum, etc. Hardware efficiency will be essential to reduce lag and maintain functional gameplay across networks.
    
### Multiplayer Network

Creating the ability for players to fight one another across a network. 

## Midterm Goals

* Characters can move with keyboard input
* Characters will not collide
* Network multiplayer started
* Physics engine started

## Final Goals

* 15%: Networking allows multiplayer interactions to occur as close as possible to real-time by efficiently 
relaying data between user devices, gameplay lag is minimized so characters interact as expected by the user (i.e. 
when their view shows that their punch just hit another user, the game movement and health stats will react 
accordingly)
* 15%: Physics Engine allows rigid body movement around the XY plane in an efficient manor, calculates pixel 
location accordingly, manages forces such as gravity, character weight, and impact due to combat
* 10%: Keyboard input controls character movement in all directions and performs combat moves, game interprets simultaneous key presses appropriately and responds quickly
* 10%: Health logic per user affected by their collisions and falling off the platform, triggers game to end when 
one user's health reaches 0%
* 12.5%: Combat Hits and Other Collisions Detected based on object location and dimensions, collision point and 
forces are relayed across network and connected devices update accordingly (i.e. player receives a packet 
indicating they were hit, that info will be relayed for interpetation by the health logic and physics engine)
* 12.5%: Game is displayed visually with at least 1 Character and 1 Stage designed

## Stretch Goals

* Wall collision/combo move logic
* Impact-Based Sound Effects

