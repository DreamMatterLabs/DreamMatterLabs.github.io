---
layout: post
title: "Designing ONEiRA's First Boss Fight"
author: Max
banner: /assets/img/blog/blogpost_3.jpg
preview: "A retrospective in the boss fight's environmental design."
---
<h2 class="post-h2">Early Conceptualization</h2>

Initially, when I started working on this area, all we had was this prompt:  

*“Descend from the Temple of the Mother into the Dreamer’s subconscious.”*  

Additionally, this area would serve as the climax of the entire level and it needed to visually convey that. As a result, I started conceptualizing!

Firstly, I repurposed one of our “temple wall” generators and created a giant stone tube that would serve as the base for a tower. The general goal of the player here would be to descend the tower and reach the subconscious as an anomaly tries to stop you. 

To make it look visually interesting and also intimidating, I used one of the weirder splines we had and used it to spawn a mish-mash of assets for the player to walk on. Toss in a point light, some fog, and a glowing halo, and the prompt was coming to life!

<img class="img-fluid post-image w-100" src="/assets/img/blog/repo.jpg">

<img class="img-fluid post-image w-100" src="/assets/img/blog/repo.jpg">

With all this, we had a pretty decent start, but the team and I got pulled away from this area onto other priorities that were related to ONEiRA’s first trailer (coming soon!). As a result, this prototype remained untouched until it was time to return…  

<h2 class="post-h2">The Big Tower Tool</h2>

<h3 class="post-h3">Fast-forward a couple of months</h3>

I gained a good deal of new PCG skills; and a new level designer joined us. By collaborating with him, we solidified a plan to create a fight that was broken into 3 phases and where the environment would change in each!

This then sparked an idea in my head for creating a big tool that would allow us to spawn a complete tower at once 😎. By doing so, we’d be able to segment the tower and make each layer unique during each boss fight phase.

<img class="img-fluid post-image w-100" src="/assets/img/blog/repo.jpg">

<img class="img-fluid post-image w-50" src="/assets/img/blog/repo.jpg">

Without getting into too complex details of how this actually worked under the hood, the basic idea is that we would provide an array of so-called LevelSpawningData to determine the size of the layers, as well as the offset of each relative to its predecessor.

As a result, by simply giving this tool a height and an offset, it would generate a level that seamlessly fit within the tower. I then set this up to spawn trigger boxes around each layer that would sync the gameplay (work in progress) directly to the environment!  

Then, with our Unreal Generalist’s help, I added floors, ceilings, and walls to this tool until it could create a fully procedural temple chamber. Ultimately, by combining it with some columns and some pretty lighting, I created the chamber room as shown below!

<img class="img-fluid post-image w-50" src="/assets/img/blog/repo.jpg">

<h2 class="post-h2">Highlighting the Narrative</h2>

During this process, I wanted the area to be imbued with ONEiRA’s story and reflect aspects of it visually. Specifically, without giving away too much, this area represents conflict and I wanted to highlight that aspect through the environmental design.

By using a material mapping plugin that maps meshes to a material instance using a datatable, I was able to achieve this. By simply adding two material instances to each mesh, the conflict could be highlighted in the very foundation of the tower.

<img class="img-fluid post-image w-100" src="/assets/img/blog/clair-obscur-expedition-33.jpg">

<h2 class="post-h2">Putting it Together (& Breaking it Apart)</h2>

Originally, I had planned on making new modules for the lower levels of the tower, but I started experimenting with just destroying them. This result was so compelling that we decided to use it through some simple noise destruction.  

<img class="img-fluid post-image w-100" src="/assets/img/blog/schedule-1.jpg">

Lastly, I added some glowing boxes to the tower that would somewhat embrace its general structure as you went down. This approach created a sense of drama and really helped with making the tower come to life in a way that fit the world of ONEiRA.

<img class="img-fluid post-image w-100" src="/assets/img/blog/schedule-1.jpg">

<img class="img-fluid post-image w-100" src="/assets/img/blog/schedule-1.jpg">

<img class="img-fluid post-image w-100" src="/assets/img/blog/schedule-1.jpg">