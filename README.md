# Shin's GB Studio plugins
## Description
Plugins for GB Studio 3.1 and up. Plugins may or may not be compatible with later GB Studio versions.
## How to install
Download the plugins as a ZIP file from the green Code button in the top right.
Further information about installation can be found in each plugin's respective README.txt file.
## License
Plugins licensed under WTFPL, so you can do whatever you like with them. Attribution to Shin or https://gbstudiolab.neocities.org/ in credits is appreciated, but not necessary.
## Engine plugins
#### Actors Pass Through Actors (3.2.0, 3.1.0)
This plugin allows for all actors to pass through other actors, including the player, even when collisions are enabled in a move event.
Moving actors will no longer stop moving when colliding with another actor.
This is useful for when you want enemy actors to collide with the player.
The only edit this plugin makes is commenting out the actor collision checks in vm_actor.c.
#### Top Down Followers (3.2.0)
This plugin allows 0-3 actors to follow the player in a Top Down scene. The plugin adds an engine field called 'Number of Followers' that can be changed from the settings or at runtime from the 'Engine Field Update' event. The plugin selects that number of actors in the scene as followers, starting with the first actor.
#### Load Sprite (3.1.0)
This plugin loads a sprite into memory in the current scene.
It does not compile to any GBVM instructions.
It only tells the GBS compiler to include the sprite in the current scene.
The sprite can then be referenced by engine code, such as when dynamically loading projectiles.