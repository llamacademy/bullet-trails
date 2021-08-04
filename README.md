https://youtu.be/
# Bullet Trails in Unity
In this tutorial you will learn how to create TrailRenderer bullet trails that can be configured on a Bullet level. This is an intentional design choice with the following assumptions:
1. Your game you will have more than 1 gun.
2. Each gun will have a different bullet prefab it shoots (different models/configurations).

This tutorial is not part of the AI Series since it's kind of a separate topic, but it's using [8 How to Make a Ranged Attacking Enemy](https://github.com/llamacademy/ai-series-part-8) as the foundation, with an auto expanding Object Pool that was implemented in [AI Series Part 18](https://github.com/llamacademy/ai-series-part-18)
If you want to follow along with the below tutorial step by step, check out AI Series Part 8 and copy/paste the [ObjectPool.cs](https://github.com/llamacademy/ai-series-part-18/blob/master/Assets/Scripts/ObjectPool/ObjectPool.cs) from AI Series Part 18. If you just want the end result, you can clone this repository.

[![Youtube Tutorial](./Video%20Screenshot.png)](https://youtube.com/watch?v=_ujeHhvOlZU)

## Patreon Supporters
Have you been getting value out of these tutorials? Do you believe in LlamAcademy's mission of helping everyone make their game dev dream become a reality? Consider becoming a Patreon supporter and get your name added to this list, as well as other cool perks.
Head over to https://patreon.com/llamacademy to show your support.

### Gold Tier Supporters
* YOUR NAME HERE!

### Silver Tier Supporters
* YOUR NAME HERE!

### Bronze Tier Supporters
* Bastian
* Jacob Martin
* YOUR NAME HERE!

## Requirements
* Requires Unity 2019.4 LTS or higher. 
* Utilizes the [Navmesh Components](https://github.com/Unity-Technologies/NavMeshComponents) from Unity's Github.
