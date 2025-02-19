# Glossary

## Mod
* **Dimension Delvers**: Current project working name. Not final.
* **Rift**: Current working name for the randomly generated dungeons that the player will enter.
* **Rift Key**: Current working name for the item that can open a portal to a rift.
* **Theme**: The visuals and general content that is applied to a rift. Utilizes processors.

## Features
* **Gear Sockets *(PoC)***: The current working system to manage the modifiers on our weapons and armor.
* **Modifier *(Feature)***: Any powerup applied to a player or to something else, will be implemented using the modifier system. This system is comparable to enchantments, but much more advanced and under our control.
* **RiftMapper *(PoC)***: An attempt to create a map of the Rift. Will allow us to remove the minimap while in a rift. 
* **Runegem *(PoC)***: The current working system for crafting your items into better items. Specifically, when applied to a gear socket, it applies a modifier to the related item.
 
## Project Management
* **Contributor**: Any person who requested the role in the discord. These people are the amazing group that intend to bring you this mod.
* **Coordinator**: Per subteam, two coordinators are assigned by popular vote. These coordinators have additional responsibilities within the project. They are responsible for ensuring all topics in their area are summarized and followed up on. You can contact your coordinator for any questions and challenges you face. Their role is purely assistance, they do not have any decisive power.
* **PM Group**: The small group of Project Managers. Their role is to ensure the project moves forward. They break ties and they ensure the team remains on focus.

## Dev Technical
### General terms
* **Java**: The programming language used by the team and by Mojang, to make Minecraft and our mods.
* **JSON**: The language used by datapacks to load data into Minecraft.
* **Mojank**: A word used by modding people when they refer to a piece of code written by mojang, that causes us to question their and sometimes our own sanity.
* **Project Board**: An overview of all open tasks for the Mod, you can asses it [HERE](https://github.com/orgs/Dimension-Delvers/projects/1).
### Project Board Tasks
* **Feature**: Something that is already decided or we have to do this either way. *Example: Rift Generation, Structure Generation, Modifier System (our better version of enchantments)*
* **Proof of Concept (PoC)**: One of the suggestions given by people. By creating a PoC, we will be able to test it out. If we only have 1 implemented PoC and we are all satisfied, then we might as well make it core. If we have a PoC and people have clear issues with the gameplay it brings, we must spend time on another PoC. *Example: Gear Sockets, Skill Crystals, Cost of dying*
* **Spike**: A spike is something we know we need, but we have not yet discussed how to do it, or maybe we have discussed it, but no clear path to implementation. Spikes can be very exploratory, sometimes even involving a mini PoC. Spikes generally should not be too long, just enough time to prove it might work. *Example: Multiblock Altar, Wireframe Minimap, Abilities*
* **Datapack**: A task to add a set of jsons as per [the datapack formats](code/datapack/datapack-formats.md). This task usually follows up on a relevant code ticket. This can be picked up by people with no skills in java.

## Build Technical
* **JigSaw**: The technical vanilla minecraft system that is used to place a structure into the world.
* **Processors**: The technical vanilla minecraft system that allows a Structure Piece in a JigSaw to be modified and drastically change its looks.
* **Structure Piece**: A single piece of a JigSaw structure, in our case, one room.
