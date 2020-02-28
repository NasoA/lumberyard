![lmbr](http://d2tinsms4add52.cloudfront.net/github/readme_header.jpg)

# Survival Scape barebones (FYI... WINDOWS DEV REQUIRED)
Goal: Use AWS Lumberyard to re-create a "Rust" like game, but stable.
Something to consider is AWS Lumberyard is free, no royalties and tied directly in with twitch. Meaning the players of this game will not use their own bandwidth to stream.
It is NOT cry engine, it was cry engine 5 years ago, they've been putting a lot of work into this. Check out Star Citizens for more info.
I wont list all the advantages of choosing this platform, but we can open up a panel for discussion with any questions.

## Clone this branch
git clone -b SurvivalScape https://github.com/NasoA/lumberyard.git


## TODO: add git modules for Custom Gems we make
A gem is the equiv of creating a package, it can be imported to any future projects and allows us all to work in a parellel fashion.

## Git bootstrap
Be sure to have git installed on your machine, if you dont run the git-2.25.1-64-bit.exe
Then run git_bootstrap.exe (this installs the default gems and setup assistant required for the next step


## Running the Setup Assistant
```git_bootstrap.exe``` will launch the Setup Assistant when it completes. Setup Assistant lets you configure your environment and launch the Lumberyard Editor. click custom install, select all the options beside android dev. Then, install the REQUIRED packages. You will see AutoCAD has a checksum missmatch, just re-install by clicking the install button and it will solve your issue.


## Launch
Create a project or use the one provided, your call

## Create a branch to PR against the SurvialScape branch
Do not PR against master, we will use this to re-base when AWS updates the engine to a next version, then we will apply the changes to our dev branch. Hopefully.
For more information about branching, see the [GitHub documentation](https://guides.github.com/introduction/flow/).

## Some helpful terms to remember

Actor –
An actor is an entity that is created in a game to create a character.
Asset–
Any file-based component that can be included in a final game, aside from code, scripts, and documentation. For example: meshes, textures, audio files, and in-game text files are all considered “assets.”
Brush–
A method of instantiating a visual element in a game. A brush is a 2D or 3D primitive shape, such as a circle, text, or volume represented as a template, and which can be "painted" into a scene.
Collider–
A computed 2D shape or 3D volume primitive associated with an in-game entity that is used to determine physical contact with it. Colliders can also be represented as meshes for more complex collision detection.
Component–
Features or groups of features that can be assigned to an entity, like “Collider” (which provides a collider volume) or “RenderMesh” (which provides the basic mesh).
Gem–
Prepackaged assets, scripts, and code that you can use to add functionality or features to your game project. Using them can save you having to write a lot of support code.
Entity–
An in-game object with a unique ID and a container. An entity contains one or more components, such as a mesh for rendering, light emitter, or sound files to play. An entity contains one or more components.  
Environment–
The visual components of a world or level, including the mesh, texture, shader, and lighting assets.
Event–
An in-game behavior that triggers when specified gameplay criteria are met. An event might be triggered by a collision, a value reaching a certain threshold, or an action taken by the player or an AI.
Level–
A discrete world or world segment that has its own specific sets of assets, events, scripts, and slices. Gameplay may differ between levels; for example, one level may be a shooter, while another may be about racing.
Mesh–
A list of vertices that represents the basic shape of an in-game object, usually supplied in a specific format. Meshes are developed in external tools like Blender or Maya 3D, and exported as assets for import into Lumberyard.
Node–
A discrete, self-contained part of a script that contains its own inputs and outputs, and which provides specific logic or calculation in response to those inputs.
Object–
Any entity in a game that has in-game interactions defined for it. The player is an object, as are projectiles, walls, items (such as weapons or loot), and non-player characters.
Slice–
A group of configured entities that are stored as a single unit in a reusable asset. Slices can also be grouped with other entities or slices to create a new slice. For example, four “wheel” entities can be combined with a “car body” entity to create a “car” slice. A slice that has animation associated with it is called an “actor” in some contexts.
World–
The greater area container in which all your slices reside. Typically, a world has its own coordinate system for slice and entity placement, as well as event triggers. “Worlds” can be anything from giant outdoor maps to discrete interior locations, such as a space station or a larger level for a building.

## Lumberyard Documentation
Full Lumberyard documentation can be found here:
https://aws.amazon.com/documentation/lumberyard/
We also have tutorials available at https://www.youtube.com/amazongamedev

## License
Your use of Lumberyard is governed by the AWS Customer Agreement at https://aws.amazon.com/agreement/ and Lumberyard Service Terms at https://aws.amazon.com/serviceterms/#57._Amazon_Lumberyard_Engine.

For complete copyright and license terms please see the LICENSE.txt file at the root of this distribution (the "License").  As a reminder, here are some key pieces to keep in mind when submitting changes/fixes and creating your own forks:
-	If you submit a change/fix, we can use it without restriction, and other Lumberyard users can use it under the License.
-	Only share forks in this GitHub repo (i.e., forks must be parented to https://github.com/aws/lumberyard).
-	Your forks are governed by the License, and you must include the License.txt file with your fork.  Please also add a note at the top explaining your modifications.
-	If you use someone else’s fork from this repo, your use is subject to the License.    
-	Your fork may not enable the use of third-party compute, storage or database services.  
-	It's fine to connect to third-party platform services like Steamworks, Apple GameCenter, console platform services, etc.  
To learn more, please see our FAQs https://aws.amazon.com/lumberyard/faq/#licensing.
