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

In this project we have 6 Scenes:

**SampleScene**:
1. Simple click to move. [AI Series Part 1](https://youtube.com/watch?v=aHFSDcEQuzQ)
2. An enemy that follows the player - [AI Series Part 1](https://youtube.com/watch?v=aHFSDcEQuzQ)
3. NavMeshLinks to allow the player and enemy to jump from one platform to another, and on top of some walls. - [AI Series Part 2](https://youtube.com/watch?v=dpJUc_BpChw)
4. AgentLinkMover to control how NavMeshAgents will traverse NavMeshLinks - [AI Series Part 2](https://youtube.com/watch?v=dpJUc_BpChw)
5. Animated 3D Model based on NavMeshAgent's movement - [AI Series Part 3](https://youtube.com/watch?v=wLZPM46zgUo)
6. Dynamically spawned enemies at random points on the NavMesh - [AI Series Part 4](https://youtube.com/watch?v=5uO0dXYbL-s)
7. 4 Enemy types, configured via a ScriptableObject, that path differently based on Agent Configuration - [AI Series Part 5](https://youtube.com/watch?v=PoglGJoDcZg)
8. Enemies and Player attack the other when they near each other, until dead. - [AI Series Part 6](https://youtube.com/watch?v=Aee01YxQIsw)
9. Ranged Attacking Enemies - [AI Series Part 7](https://youtube.com/watch?v=QzitQSLhfG0) and [Part 8](https://youtube.com/watch?v=Aee01YxQIsw)
10. Configurable Homing Bullet Mechanics for Ranged Enemies - [AI Series Part 7](https://youtube.com/watch?v=QzitQSLhfG0) and [Part 8](https://youtube.com/watch?v=Aee01YxQIsw)
11. Improved ScriptableObject Configurations - [AI Series Part 9](https://youtube.com/watch?v=lRdetRvi8FA)
12. Flying Enemies - [AI Series Part 10](https://youtube.com/watch?v=cN837GYgxUI)
13. State Machine AI with 3 options - idle, patrol, chase, including line of sight checking - [AI Series Part 11](https://youtube.com/watch?v=3hXkdARwREo)
14. Bullet Trails configured via a ScriptableObject - [Bullet Trails](https://youtube.com/watch?v=_ujeHhvOlZU)

**NavMeshLink Demo**: [AI Series Part 17](https://www.youtube.com/watch?v=PD6VFD1a21g)
1. Small scene with several NavMeshLinks with different configurations to showcase customization of NavMeshAgent movement over a NavMeshLink based on Area Type.

Additive Loading Scenes: - [AI Series Part 16](https://www.youtube.com/watch?v=ygr5YyTRsBY)

**Additive Scene 1**:
1. SampleScene below with a trigger to load a new scene when the player gets to a particular zone of the level
2. Additively load "Additive Scene 2"

**Additive Scene 2**:
1. Connects to "Additive Scene 1" with a NavMeshLink to allow players and enemies to travel to the new scene uninterrupted

Progressive NavMesh: - [AI Series Part 13](https://youtube.com/watch?v=QPv_V4TCi8o)
1. A procedurally generated world and NavMesh so it can be navigated by NavMeshAgents
2. Enemies spawn as the player runs throughout the world, becoming disabled when they are too far away from the player.

Bake NavMesh in Bounds: - [AI Series Part 14](https://youtube.com/watch?v=RuoK7w1OIT0), [AI Series Part 14.5](https://youtube.com/watch?v=bCC5pqNT000), and [Part 15](https://youtube.com/watch?v=0V99OBWmCHk)
1. A Player-only scene baking a NavMesh around the player as they move
2. Spawning enemies as the player moves throughout the large world

## Requirements
* Requires Unity 2019.4 LTS or higher. 
* Utilizes the [Navmesh Components](https://github.com/Unity-Technologies/NavMeshComponents) from Unity's Github.
