---
layout: post
title:  "Art Direction - An analysis"
category: game-development
tags: week-5 spark 
---

The week 5 spark challenge is to review the art direction on a high impact game, and then to find another game with a very low art budget and compare. 

## Analysis 

Firewatch, having won the unity award in 2016 for best 3d visuals, feels like a strong contender for a visually interesting game. It's very stylised but also realistic and immersive. It's art style and direction is also well documented and inspired by the national parks posters from the 1930s.

### Character Design 
- First-person
- Full body awareness - you can see your legs, feet, hands, belly.
- You don't see yourself, aside from a sketch during the narrative pre-amble at the start. There is no visual character customisation.
- Stubby square-ended fingers, providing some comic relief every time you pick up the walkie talkie. 

### Colour Palette
- The concept art, box covers, and game splash screen all use strong, bold colours to set the right tone for a mystery in the woods. 
- The colour palette changes based on the mood and emotion in the scene. 
- The design team created a colour script for each story element or game area. Starting with a grey box, then a paint over, and then rebuild the scene using the colour over as a more detailed colour script.

### Environment Design
- Open world, lots of challenges with world streaming
Forces utilisation of changing terrain and environment to mask loading. Gulleys, densely overgrown forests, large rocks, cliff faces, narrow canyons with sharp corners. These all help to block off areas for later discovery, as well as optimise scene streaming.
- A small number of modular assets are far more useful and easier to update when changes are needed. Each rock was crafted to have interesting characteristics from every angle so it could be reused easily. 
- For a game based in a forest, only 23 different trees were created, 14 of which were used commonly. Particular attention was paid to the lower branches in the trees, as these were at the player height. 
- Dynamic wind response for trees was also custom-built, with different types of movement aligned to parts of the tree, including trunk sway and branch flap.

### Post Processing
Game lighting is derived from the sky as it is an outdoor game. Dynamic lighting is based on time of day and weather. 
A custom fog shader is used, as they want finer colour control over distance to match their original concept art. 
Alpha cutoff was modified in conjunction with LOD models to create a more silhouette style for distant objects.

## Minimal Art Style

I dug deep through my steam collection for a game with impact and minimal art style. Darwinia was a contender for a while as I love the retro, almost TRON like styling. Dwarf Fortress needs an honourable mention, having some of the lowest fidelity art in a still actively maintained game. 

I finally settled on shapez.io. A little known game released initially as an open-source, HTML based incremental game, later released on steam with some premium features.  The game is loosely based on Factorio. You are designing a factory, but instead of building rocket ships to escape an alien planet, you're making coloured icons out of components. Each level introduces new mechanics and increasingly complicated goals, including layered icons and multi-coloured segments. 

The game doesn't have a character and has a minimal UI. The art style is sharp and clean, feeling more like a mathematical chart or architectural drawing. You are drawn in by the increase in difficulty and complexity and the myriad of upgrades available. Not everything unlocks with a level, and for example, multiple icon types are required to increase the painter block's speed.  

Something is rewarding about working in detail on a small segment of an icon, then clone it out to increase the scale and performance of that piece of the factory and then zoom out to see the sizeable interconnected spaghetti monster you have created. 

I feel the game is successful through the use of in depth game mechanics, with short and long term achievements to keep you focused on what to build next, rather than a strong narative or high production value art. 

### References

- BENNETT, Jay. 2016. 'The Forgotten History of Those Iconic National Parks Posters'. Popular Mechanics [online]. Available at: https://www.popularmechanics.com/adventure/outdoors/a22536/national-parks-posters/ [accessed 19 Feb 2021].

- NG, Jane. 2016. Making the World of Firewatch [Film]. Available at: https://www.youtube.com/watch?v=hTqmk1Zs_1I [accessed 19 Feb 2021].

- NG, Jane. 2019. The Art of Firewatch [Film]. Available at: https://www.youtube.com/watch?v=SdxQ3HlhTE8 [accessed 19 Feb 2021].

- NG, Jane. 2021. 'Campo Santo'. Campo Santo [online]. Available at: https://blog.camposanto.com/post/100680711679/i-asked-twitter-if-anyone-had-questions-about-the [accessed 19 Feb 2021].

- UNITY TECHNOLOGIES. 2021. 'Unity Awards 2016'. [online]. Available at: https://awards.unity.com/archive/2016 [accessed 19 Feb 2021].
