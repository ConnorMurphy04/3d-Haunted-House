# Escape the Haunted House

**Escape the Haunted House** is a spooky first-person adventure game where the player must navigate a haunted mansion, avoid ghosts and gargoyles, and escape before being caught.

---

## Table of Contents

1. [About](#about)  
2. [Gameplay & Features](#gameplay--features)  
3. [Controls](#controls)  
4. [How to Run / Build](#how-to-run--build)  
5. [How to Play](#how-to-play)  
6. [Assets & Credits](#assets--credits)  
7. [Known Issues](#known-issues)  
8. [Roadmap](#roadmap)  

---

## About

This game is my first 3d game I have created so I wanted to create a game design that felt immersive, but also had a level of difficulty to it. It uses fun, silly character and object designs to make this game fun and captivating. 

---

## Gameplay & Features

- Third-person exploration in a haunted mansion    
- Multiple room layout with halls and doorways  
- Scary audio design: ambient sounds, whispers, footsteps
  including jumpscare audios for failure
- Audio noises for winning conditions
- WASD functionality to move around
- Moveable and static enemies for difficulty

---

## Technical Implementations
In this game, many new features and technical implementations were utilized. To start, my scene was created with a preset layout that created an entire map of a haunted house, not just box collider restrictions. Next, when creating both the main character player object and the enemy player objects, multiple forms of animations were used. When the players or enemies were idling they had "idle" animations that saw them bouncing around or floating. This animation was connected through animator components with "walk" animations that saw a change in movement style when one of the controls mentioned below were pressed and they entered a walking or moving state. The next big implementations was the adding of a third person follow camera, while it does have an issue as mentioned below, as you see in many 3d games. This game also includes the use of Waypoint markers that create set points that enemies within the mansion can freely travel between, while they do include some bugs. The mansion itself does also include ambient music and sounds. Also, when a game state is reached, such as an escape or a being caught, there is mathing audio effects and visual effects that let you know what state in the game you are currently in. 

## Controls

| Action | Key / Input |
Move Forward | W |
Move Backward | S |
Move Left | A |
Move Right | D |

---

## How to Run / Build

**Requirements:**
  
- Platform: WebGL via link: https://play.unity.com/en/games/5ed760e6-f728-4979-8178-c1192c42f6f8/escape-the-haunted-house
 
 ---
  
## How to Play

1. Start the game from the main menu.  
2. Explore the haunted house to find new rooms and hallways  
3. Discover where hidden enemies lurk
4. Avoid the traveling ghosts blocking certain rooms  
5. Your goal is to escape the house before one of the enemies find you.

---

## Assets & Credits

This game was created through step-by-step following of a Unity Learn 3d tutorial. The tutorial is named 3D Haunted House Tutorial. 

---

## Known Issues

There are a few known issues that need to be mentioned because they do heavily impact the playability and functionality of this game. The first main issue is with the main character. The character should be able to rotate towards the direction that the player is trying to walk. However, the in-game character is locked facing forward for a reason I could not figure out. The next issue is with the third-person follow camera. The camera should be directly behind the player as is seen in most third-person games. However, the camera is staggered off centered to the right and I was unable to figure out why. The next known issue comes with the ghost enemies. I tried to implement waypoint features where the ghosts would have two set locations they traveled between. This was implemented seemingly correctly as the ghosts do move, but they move in the wrong location. Once the game begins they seem to forget their bounds within the game scene and travel between locations that they did not originally spawn into, some within the mansion, and some not. The last main issue that I know of comes with certain caught states. The caught states are when the player object travels into the collider of an enemy, this should end the game. However, not every time a player walks into the vision of an enemy does the game end. Sometimes it does, sometimes it does not. 

---

## Roadmap

- [ ] Add more rooms / haunted areas  
- [ ] Implement a save system
- [ ] Create locked rooms
- [ ] Create solvable puzzles
- [ ] Create dialogue options
- [ ] Add UI for inventory and puzzle hints  

---
