# Lesson08 - Unreal Engine Physics

* Here is the link to the video demo for this lesson: [link](https://drive.google.com/drive/u/1/folders/1C7_Q5CtlSeE-fFxhuSKNWZQ80T-PIe2u)

## Asset packs used:
* Infinity Blade: Effects
* Starter Animation Pack
* FPS Weapon Bundle

## Project info
* Used different forms of replication to create a online multiplayer first person shooter.
* Learned and utilized Event Pointdamage to apply damage to clients through a server.
* Used line trace as bullets. Line trace only shows in server.
* Added a real-time kill/death scoreboard along with health bars. It updates when variable changes for the client character or Player State.
* A respawn mechanic is also added. (5 seconds) A custom event (PlayerDied) is made with Multicast to manage player death and respawn in the third person character.
* Added a game timer (1 min) to the entire session. The timer is set on the server, and clients receives updates. When the timer ends, the entire session ends. 
