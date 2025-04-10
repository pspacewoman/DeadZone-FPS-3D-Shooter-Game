# Game Design and Development: 3D Shooter
---

![image](https://github.com/user-attachments/assets/c19036a2-93b5-473b-8178-721c87d76677)

<details>
<summary>🧩 <strong>Goal</strong></summary>
-   To develop a 3D game for FPS (First-Person Shooter) in UNITY
-   Games Asset Creation and Concepts
-   Level Design
-   Game Balancing
-   Prototyping
-   Playtesting

![Screenshot 2025-04-09 at 15 08 02](https://github.com/user-attachments/assets/0ba00415-a1b1-4200-a3fe-a1663b52ac1f)

</details>

<details>  
<summary>🧩 <strong>Project Objectives</strong></summary>

1. Created 3D games in Unity
2. Implemented typical 3D shooter (FPS) mechanics
3. Level design in 3D space
4. Practiced a typical level design pipeline from grayboxing to an art pass
5. Understood a bit about 3D modeling concepts such as faces, vertices, extruding, and edge loops (using ProBuilder)
6. Using ProBuilder to help in grayboxing levels (aka, level design prototyping)
7. Further understanding the asset pipeline and 3D asset setup
8. Created particle effects
9. Learning to use the Unity Audio Mixer
10. Used NavMesh to create Enemy movement
11. Creating more elaborate UI
12. More complex game systems
13. Understand good coding practices such as creating and following a coding standard
14. Understanding ad hoc programming vs. generalized programming

</details>

<details>  
<summary>🧩 <strong>Concept</strong></summary>
-  Using ProBuilder to help in blocking out levels (aka, grayboxing or level design prototyping)
-  Using ProBuilder: Understanding a bit about 3D modeling concepts such as vertices, edges, faces, extruding, and edge loops
-  Practicing a typical level design pipeline from grayboxing to an art pass
-  Level Design in 3D space
-  Creating particle effects
-  Using NavMesh to create Enemy movement
  
</details>


<details>  
<summary>🧩 <strong>FPS</strong></summary>
-  Featuring First Person Point
-  Sees action through eyes of the player character
-  Designing 3D game for FPS in UNITY

##Unity Rendering Pipeline
-  The Rendering Pipeline is the steps the game engine goes through to draw or render the scene.
-  Different rendering techniques can create higher quality or lower quality graphics, and may be more optimized or less optimized depending on the graphics hardware of the computer.
-  Unity provides support for three different Rendering Pipelines, including the Built-in Rendering Pipeline, the Universal Rendering Pipeline, and the High Definition Rendering Pipeline.
-  Using URP for this project

</details>



<details>  
<summary>🧩 <strong>Level Design through Grayboxing</strong></summary>
  
##Creating a 3D URP (Universal Rendering Pipeline) Project
Steps-
1.  create URP assets
2.  import Unity's input system package
3.  download and import project assets
4.  import ProBuilder:
      a.  ProBuilder is a 3D-level design tool now owned by Unity.
      b.  It adds tools to build, edit, and texture custom 3D geometry right inside Unity, so you don't need to go to an external 3D tool such as Blender or Maya.
      c.  ![Screenshot 2025-04-09 at 15 40 36](https://github.com/user-attachments/assets/359530e7-c99e-454b-8007-840a7dd08a36)
5.  add probuilder to mesh settings
6.  Graybox Level Design: Floor and Walls
    -  Greyboxing is a level design technique where you rapidly prototype the level using basic visuals, such as greyboxes, to get the level into a playable state as quickly as possible.
    -  Probuilder is an excellent tool for Grayboxing in UNITY.
  ![Grayboxing](https://github.com/user-attachments/assets/636902e6-da13-4648-a2c5-07de6356a816)

7.  Drawing on paper using a pencil the levels first
    Top-down map of simple level design and greybox in Unity.
8. create scene
9. create layout on paper with pencil -> draw levels of your game and mention challenges which will be cleared to move to next level
10. create cube shape > excrude the faces and tilly axis 17 (face selection tool)
11. Graybox Level Design our first level: First Room-
    -  Block out room 1 with Level 1
    -  Divide the cube into 2 rooms separated by a door
    -  room 1 - create cube1 (platform 1)
    -  create cube2 (platform 2)
    -  create a key to door
    -  create a player
12. Finishing up Graybox our first level: Second Room-
    -  blocking out second room
    -  create pillar 1 and pillar2 cylinders
    -  create moving platfrom
    -  create a goallocation cone
13.  Test Grayboxed Level
    -  created a 'test player' from prefab in the place of playerstartposition
    -  deleted main camera ad 'test player' has its own camera for FPS
    -  tested the game levels across 2 rooms
14.  Enhance the Grayboxed Level-
    -  Added waypoint1 and waypoint2 to movinfplatform to move b/w two pillars (waypointmover script)
    -  Downloaded new assets WorldMaterialFree
    - Applied the new material on floor and platforms

  
</details>

<details>  
<summary>🧩 <strong>Level Design Art Pass</strong></summary>

**Steps-**

1.  Art Pass: Floor
    -  adding production art
    -  1st - starting with replacing the floor
    -  add floor environment from prefabs
2.  Art Pass: Outer Walls
    -  created 4 outer walls using prefabs > environment > walls
3. Art Pass: Middle Walls
    -  focused on door and middle wall b/w two rooms
    -  added a window
4. Art Pass: First Room
    -  replaced platform box with prefab platfroms
    -  added key to door
5. Art Pass: Second Room
    -  added moving platfrom
    -  added goal location
    -  added pillar1&2

</details>

<details>  
<summary>🧩 <strong>The Player Setup</strong></summary>

6. Full Player Setup
    -  TestPlayer replaced by > prefab > player > FPS Player
    -  Test the game
7.  Player Prefab Walkthrough
    -  Understanding FPS Player > Settings on Inspector Mode
    -  FPS player > camera > Inspector setting
    -  FPS player > camera > Shooter > Inspector setting


</details>
