# Lesson06 - Unreal Engine Physics

* Here is the link to the windows build and video demo for this lesson: [link](https://drive.google.com/drive/folders/1oKM3RulUD8sfqgDCLWlh0WnROfr1iCht?usp=sharing) I also added my project files as backup. (LFS is running out of space...)

## Asset packs used:
* Infinity Blade: Effects
* Starter Animation Pack
* FPS Weapon Bundle

## Project info
* I used my animation project as starting point.
* I changed the camera to first person and added a very long *spring arm* with an *aim object* attached. This makes sure that all the line trace hits can be at the center of the screen when the gun is firing. 
* I added three different physics materials for footsteps: Wood, Grass, and Concrete. Each material will cause the footstep to sound different.
* I added three different physics materials for enemies as well: wood, dirt, and steel. Each material will cause the enemy object to be affected by the bullets differently
* The footstep sound is created through *line trace* with *animation notifies*. 
* The bullet hit registration is also created through *line trace*. Everytime the player fires, a new line trace will happen and check if the player has hit an enemy and what physics material the player is hitting. 
* Weapon pickup is also added. This is done through a *Sphere Collision component* with *line trace*. When the weapon overlaps with the sphere collision component, a boolean variable allows the line trace check to occur. If the player is aiming at the weapon, the player can press e to pick it up. 
