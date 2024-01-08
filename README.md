# Unreal-Top-Down-Shooter
I had been obsessed with a top down shooter on my phone, therefore, when I was tasked with creating my own game during my internship at Prosper IT Consulting, I decided to create one of my own. Since I was given just a 10 day sprint to complete a fully functioning game on Unreal, I thought a top down shooter/survival game was a challenging yet feasible project to tackle. My main goal in recreating this game was to give users a fast paced, yet fun experience that they want to play over & over again. It should be noted all of the animations in game were outsourced and freely licensed.  

## Scene Management
Scene management within this project is controlled by several blueprint widgets that swap between the main menu, game, and end screen. 

Example of scene transition: 

![SceneTransition](https://github.com/NickGuzi/Unreal-Top-Down-Shooter/assets/140576874/deaf0ea0-fe71-42d5-b94b-335108c89e5f)

Scene Transition Blueprint:

<img width="541" alt="SceneTransitionBP" src="https://github.com/NickGuzi/Unreal-Top-Down-Shooter/assets/140576874/d3008c98-ab9a-45ae-8a35-061f3f167f35">


## Player 
The player is the most complicated entity in this game. They possess their own animations, movement blueprinting, damage/health/collectible systems, and weapon capabilities.

Example of idle animation: 

![IdleAnimation](https://github.com/NickGuzi/Unreal-Top-Down-Shooter/assets/140576874/119c3cf1-3120-4019-89de-113e16e0463c)

Blueprinting for player health bar:

<img width="536" alt="PlayerBPEx" src="https://github.com/NickGuzi/Unreal-Top-Down-Shooter/assets/140576874/f841d4fd-9476-4c15-9d3c-17ef16a83b8b">


## Zombie & Zombie Spawner
AI in this game is wholly possessed within the zombie character. They possess their own animation, chase system, health system, and are able to be spawned in game through a separate spawner blueprint.

Example of zombie walk: 

![ZombieRun](https://github.com/NickGuzi/Unreal-Top-Down-Shooter/assets/140576874/53f7c142-72a1-4b8c-a485-81e2f2163afe)

Blueprinting for AI chase system:

<img width="637" alt="AiChase" src="https://github.com/NickGuzi/Unreal-Top-Down-Shooter/assets/140576874/05e70545-ef9c-4256-a827-9e149ed52b72">

Zombie spawner blueprint:

<img width="618" alt="ZombieSpawner" src="https://github.com/NickGuzi/Unreal-Top-Down-Shooter/assets/140576874/20ca35f1-d593-46dc-82aa-5fcb194ddeb2">


## Collectible & Collectible Spawner
This game possesses one jump boost collectible. It gives the player a jump buff for 10 seconds, produces a pop up on the game HUD utilizing a separate widget blueprint, and uses the same spawner system as the zombie character. The function that causes the player to jump is contained within the player blueprint.  

Collectible appearance:

![Collectible](https://github.com/NickGuzi/Unreal-Top-Down-Shooter/assets/140576874/9af9a736-4f2a-4367-ae53-918bf9acb504)

Jump boost function nested in player blueprint:

<img width="601" alt="JumpBoost" src="https://github.com/NickGuzi/Unreal-Top-Down-Shooter/assets/140576874/330f0f07-453f-4518-a2a2-11ba5b9ac0f6">


Collectible blueprint that calls upon jump boost function and collectible HUD:

<img width="565" alt="CollectibleHUDCall" src="https://github.com/NickGuzi/Unreal-Top-Down-Shooter/assets/140576874/dbe507ab-8424-49cb-ae27-7665d6f94249">


## Laser Bolt
The laser bolt projectile possesses the capability to kill zombies and fire upon the player's command. The laser's fire capabilities are wholly possessed within the player blueprint.  

Laser bolt blueprint:

<img width="628" alt="LaserBolt" src="https://github.com/NickGuzi/Unreal-Top-Down-Shooter/assets/140576874/a6960074-64ff-4533-aa76-f7a81e8d6d9e">

Fire weapon blueprint:

<img width="504" alt="FireWeapon" src="https://github.com/NickGuzi/Unreal-Top-Down-Shooter/assets/140576874/a01594e8-d7d7-4f8f-b39e-a158a03931d6">

