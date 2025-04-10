# 🎮 DeadZone - FPS 

### Game Design and Development: 3D Shooter Game

---

![Unity](https://img.shields.io/badge/Unity-100000?style=for-the-badge&logo=unity&logoColor=white)  

📌 **Live Game (Version 1.0)**:  
[Behance Link](https://www.behance.net/gallery/223414589/DeadZone-FPS-(3D-Shooter-Game))  
[Itch.io Link](https://priyanshi-singh.itch.io/deadzone-fps)

![Platform](https://img.shields.io/badge/Platform-PC%20&%20Web-blue?style=for-the-badge)  
![Status](https://img.shields.io/badge/Status-Completed-green?style=for-the-badge)  
![Version](https://img.shields.io/badge/Version-2.0%20Coming%20Soon-orange?style=for-the-badge)

---

🚀 From Game Player to Game Developer. The only thing more fun than playing games is making them. 

---
Built From Scratch👩🏻‍💻 
Added my own notes below for understanding the development process 📝


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
<summary>🧩 <strong>Module 1: Concept</strong></summary>

  
-  Using ProBuilder to help in blocking out levels (aka, grayboxing or level design prototyping)
-  Using ProBuilder: Understanding a bit about 3D modeling concepts such as vertices, edges, faces, extruding, and edge loops
-  Practicing a typical level design pipeline from grayboxing to an art pass
-  Level Design in 3D space
-  Creating particle effects
-  Using NavMesh to create Enemy movement
  


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


<details>  
<summary>🧩 <strong>Animation & Visual Effects</strong></summary>

1. Setup Imported Animation-
   
   - fbx file in our assets
   - setting up animation which comes from fbx file
   - Setting up pistol animations : idle and shoot mode

   ![Screenshot 2025-04-10 at 02 21 35](https://github.com/user-attachments/assets/76820208-327d-49e7-a753-f80358336faf)

3. Creating Particle Systems
   
   -  A particle system allows you to simulate non-solid, fluid-like entities such as smoke, fire, explosion, splashes, and dust clouds.
   -  Particle systems work by emitting mini-particles made up of either 2D sprites or 3D meshes, in the scene, over time.
   -  Particle systems are a great way to add further visual polish and feedback for the player.
   -  In this Game Scene -  I created a visual effect when I shoot the pistol, using a particle system.
   -  goto 'prefab' -> PistolFireEffect -> double click to enter prefab edit mode -> edit puffofmoke or pistolfireeffect based on the requirement
   -  added new partcile 'puffofsmoke'
   -  added and set the emission rate and figure of the smoke
   -  adjusted the 4 explosion strokes and rate
   -  changing the size of the particle 'size over lifetime' - turn on
   -  size is setup as large to small (particle system curves)
   -  setting up color of the smoke dark grey to light grey (transparency to 50)

</details>


<details>  
<summary>🧩 <strong>Shooter Game Animation and Visual Effects</strong></summary>

  
1. Level Management

-  Setting up some global-level management elements such as the lighting, music, user interface, cursor control, and the game manager. 
-  Hierarchy > Level Management > 
-  Hierarchy > Directional light > turn off
-  Setting up multiple directional light > prefabs > lighting > indoor lighting
-  setting up cursor manager
-  adding UI and Music and Lightning
-  Testing out the game

2. Enemy AI

-  Added some enemies into our level to heighten the challenge for our players.
-  Many of my game enemies will be driven by artificial intelligence to navigate the level toward the player.
-  I'll be using Unity's AI navigation system to allow our enemy to navigate our scene.
-  I added 3 enemies to my scene and made 1 change in their script
-  select enemy > inspector > groundenemy script > LineOfSightHitLayer > Environment,Player

3. Pickups
   
-   Providing Players with some pickups to aid them on their journey across the level.
-   added 2 health pickups in both rooms and increased health life to 2

4.  More Prefabs

-  added props
-  added checkpoint

5.  Audio Mixer

-  Unity Provided an Audio Mixer Tool
-  project > Audio > right-click > create audio > Create NewAudioMixer > re-name 'In-Game Audio Mixer'
-  created 3 audio mixers and added those into the prefabs music setting for:
     -  prefabs > effects > pistoleffect
     -  prefabs > effects > UI > UISwitchEffect
     -  test the audio and adjust accordingly
     -  next - > giving the player a UI to adjust the volume of an audio group, such as music versus sound effects. via something like the setting pop up.

6.  Adding More Levels

-  add a main menu and level1 scene on build profile scene list > exit
-  open main menu scene > test the buttons
-  add new level2 > add more prefabs > props in the level2 scenes
-  added more enemies
-  back to level1 > level management > uimanageringame > victory page > next level button > inspector > onclick (set level2)
-  back to  main menu > uimanagermainmenu > levelselectpage > onclick (level2)
-  add level2 scene to build profile scene list

</details>

<details>  
<summary>🧩 <strong>Programming C#</strong></summary>

**1. Coding Standards:**
  
unity > project > right-click > open C# Project

-  PlayerController.cs Script   (ad-hoc programming)
  
-  A coding standard is an agreed-upon structure of how to write code. Helps to review the code individually or working in teams.
-  You can have different coding standards across different projects, teams, and companies.
-  But the point of having one is to make the code more readable and easy to understand by having the same rules followed by everyone on the team for every script in the project.
-  In this project, all the provided scripts were written using the same coding standard. Like class headers ->
  
-  Rule 1: One of the rules we followed in this coding standard was to have class headers like this one at the top of each script. This is a summary block comment that provides additional description about what a class does so that anyone new to the script would have an easier time understanding what the script does beyond just the class name.

  
-  Rule 2: Another rule that we had was to put tooltips above every public variable in this class. This makes the code more readable and it helps you understandable. I like to say it makes your code more designer-friendly.

  
-  Rule 3: I followed to have distinct casing used between our classes and functions versus our variable names. Our classes and functions have every first letter in a word capitalized, which is called upper camel casing. Whereas the variables use lower camel casing, where the first word is lowercase and then the first letter of every word past that is uppercase.

  
-  Rule 4: I followed - was to have headers for any distinctive grouping of variables like this, so that the variables would be labeled in the inspector. Once again, this makes the script more designer-friendly. It also means we group related variables together in our code, which is another rule in our coding standard.

  
-  Rule 5: There are two lines of thought with organizing class variables within my script. I like to put variables near where they are used in the code. This is called the principle of proximity.

  
-  Rule 6: Another rule I followed to make the code easier to understand is to have a function header above every function that describes what the function is meant to do, what inputs it takes, and what it returns, if anything.


**Learning to reverse engineer someone else's code is an important skill in learning to program. The coding standard should help you in this process.**



**2. Ad Hoc vs. Generalized Code**

-  The health script handles the health state of the game object it is attached to, including health points and lives.
-  Having a general health script written in a robust manner to cover all the use cases made sense.
-  We write it once and use it many times.
-  It allows us to leverage our previous work to create games smarter and faster.
-  Ad hoc programming is writing code for a specific purpose rather than a generalized purpose.
-  Generic script - this script only does what it needs to do for controlling a first-person character, and that conciseness makes it both easier to create and easier to understand.

 </details>
</details>


<details>  
<summary>🧩 <strong>Module 2: Game Assets</strong></summary>

1.  Game Graphics
2.  Game Audio
3.  Asset Pipeline
4.  Programming Best Practices 

</details>


<details>  
<summary>🧩 <strong>Version 2.0 (In-Progress 80%)</strong></summary>

___

1. 3 significant modifications
2. new name of the game
3. new UI of the game
4. ScreenshotUtility
5. iterative testing to fix bugs and code issues
6. include all scenes in the Unity "Build Settings"
7. create and test Windows, MacOS, and WebGL builds
8. upload game on itch.io

---

**Ist Modification: Design Modifications (these are more design intensive), such as:**

1. Create a complete interesting, comprehensive, and coherent level.
2. Add multiple additional levels and tie them in to create a logical progression in your game. (NOTE: Each level should be unique in some way, such as different type of challenges for the player.)
3. Modify the out-of-game menus in some significant and meaningful way.

---

**IInd Modification: Aesthetic (Visual/Audio) Modifications (these are more art intensive), such as:**

1.  Reskin the existing graphics in some significant way, such as change the player or an enemy to a completely different character.
2.  Add additional significant and coherent graphical elements to the game, such as new enemies or environmental challenges, complete with animated states.
3.  Replace sound effects in the game to update the sound design of the game. (NOTE: You will need to change ALL the sound effects for this to be significant. Don't just change one.)
4.  Add custom music to your game. (NOTE: Custom meaning you created the music with a tool such as Garage Band or Fruity Loops. If you just swap out the music for another track you find, this is not considered a significant change ... though you can do it without it counting as a significant modification.)

---

**IIIrd Modification: Gameplay Modifications (these are more system/programming intensive), such as:**

1.  Add new player abilities, such as modified controls, additional moves, or additional power ups.
2.  Add new enemies with their own behavior. (NOTE: This can be considered two modifications if you create unique behavior AND create the art and animation.)
3.  Add new obstacles and challenges. (NOTE: This can be considered two modifications if you create unique behavior AND create the art and animation.)
4.  Modify the in-game GUI in some significant way.

</details>

</details>
