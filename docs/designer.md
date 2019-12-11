
## Installation
* Install [Blender 2.8](https://www.blender.org/download/releases/2-80/) on your computer, Mac OS or Windows
* [Get Your Designer Software](https://www.vimdrones.com/contact)
* In Blender 2.8 **Edit** -> **Preferences** -> **Install**, Select downloaded Designer Software .zip

## Active License
* Select **License** Tab, type your email, token and click **Active** Button
![Vimdrones Desiginer Active License](/static/active-license.png "Vimdrones Desiginer Active License")
    * Press **N** to show/hide **Properties**

## From Blender To Real World
* Blender and Real World axis relationship shown as below
![Vimdrones Desiginer Geo Baisc](/static/geo-basic.png "Vimdrones Desiginer Geo Baisc")

* drone light show design is based on 24 FPS which means 1s run 24 frames, this value should not be changed unless you know what you are doing

## Geting started Blender
* Open Blender 2.8, **New File** -> **General**
* Press **A** to select all the objects in the 3D Viewport, then press **X**, **D** to delect the objects

## Create Drone Team
* **Vehicle** -> **New Team** -> **Create**
![Vimdrones Desiginer Create Drone Team](/static/create-drone-team.png "Vimdrones Desiginer Create Drone Team")

* What is x qty, y qty, qty mean? <br>
qty represent the total quantity of your drone team <br>
x qty and y qty define your a single block shape in ground, as the image shown below 
![Vimdrones Desiginer Drone Team Params](/static/drone-team-parms.png "Vimdrones Desiginer Drone Team Params")

* What we have after create drone team? <br>
    * drones Collection ([What is Collection?](https://docs.blender.org/manual/en/latest/scene_layout/collections/collections.html))
    * distance checker Collection(quick preview for min distance between drones)
    * effectors Collection
    * Begin Scene Collection
    * End Scene Collection

## Takeoff the Drones
* In the [Timeline](https://docs.blender.org/manual/en/latest/editors/timeline.html) window, Current Frame -> 0 <br>
  **Formation** -> **Append**, select formations **Begin Scene**, click **Begin** Button
* Current Frame -> 1 <br>
  **Formation** -> **Append**, select formations **Begin Scene**, click **Append** Button <br> 
  (the drones are reach the loction of the Empty Objects)
* Select Empty Objects in the Begin Scene Collection, insert [keyframe](https://docs.blender.org/manual/en/latest/animation/keyframes/index.html)
* Set the Current Frame -> 600 (25s, press ctrl/Command T to change )<br> 
  Move the Empty Objects to Z:50m, insert keyframe

## Change the Drone Formation
#### Create Drones Vertex Group
* Select the Mesh Object(E.g **Cube**),change **Object Mode** to **Edit Mode**
* In the **Properties** Editor, click **Object Date** tab, click the button "+" on the right Panel border to add a Vertex Group, double-click the "Group" name and edit to "drones"
* Select the Vertexs of the Mesh Object (one vertex represents one drone), click **Assign** button below the Panel<br> 
![Vimdrones Desiginer Add Vertex Group](/static/vertex-edit.jpg "Vimdrones Desiginer Add Vertex Group")
    * We could use the tools on the left to edit the vertexs. Or from the Menu Bar **[Vertex](https://docs.blender.org/manual/en/2.81/modeling/meshes/editing/vertices.html#)** to edit the vertexs. <br> 
    Add the vertexs:[Loop Cut](https://docs.blender.org/manual/en/2.81/modeling/meshes/editing/subdividing/loop.html#tool-mesh-loop-cut) is a very useful tool.<br> 
    Delete the vertexs: Selcet the vetrexs, press **X** key to Delete or [Dissolve the vertexs](https://docs.blender.org/manual/en/2.81/modeling/meshes/editing/basics/deleting.html?highlight=delete%20vertex).

    * We could know how many vertexs have been Assigned on the Status Bare(lower right corner)
![Vimdrones Desiginer Vertex Number](/static/vertex-number.jpeg "Vimdrones Desiginer Vertex Number")
    * In the Vertex Group Panal, we could click the **Remove** button to remove the vertexs which have been Assigned. And we could click the **Select**/**Deselect** button to check which vertexs have been Assigned.
* Change **Edit  Mode** to **Object Mode**

#### Change the Drone Scene
* **Formation** -> **New Formation**, selcet the Formations Scene(E.g **Begin Scene**) which need to be changed, then click the **Copy** button to copy a **New Formation** at in same loction. Double-click the **New Formation** in the outline Editor to edit the mane(E.g **Cube Formation**)
* **Formation** -> **New Material Collection** -> **New**, creat New Material Collection in the outline Editor. Double-click the collect to rename it(E.g **Cube Material**)
* Secect the Mesh Object(E.g **Cube**) which has the Drones Vertex Group, move it to the Material Collection(E.g **Cube Material**)
    * We could add more Mesh Objects to the Material Collection. These Mesh Objects should also have **drones** Vertex Group. That's much easier for us to design the drone scene.
    * **File** -> **Append/Import**  
    We can append/import the objects from other files and use them as the Material of drone scene. For example, if we import svg. files, we should convert them to Mesh(**Object** -> **Convert to** -> **Mesh from Curve/Meta/Surf/Text** in the Menu bar)
* **Formation** -> **Vertex Formation**, select the formations(E.g **Cube Formation**) and its corresponding material_collections(E.g **Cube Material**). Click the **Append** button. The Empty Objects in the formation will reach the location of the "drones" Vertex Group
![Vimdrones Desiginer Formation Changing](/static/formtion-changing.jpg "Vimdrones Desiginer Formation Changing")
* In the Timeline Editor, set up the Current Frame to begin the new scene<br>
**Formation** -> **Append**, select formations(E.g **Cube Formation**) , click **Begin** Button
* In the Timeline Editor, set up the Current Frame to finish the new scene changing<br>
**Formation** -> **Append**, click **Append** Button. Move the Playhead, we could how the drone scene change(makesure the **auto resign** have been "√")
![Vimdrones Desiginer Formation Append](/static/append-3d-eagle.gif "Vimdrones Desiginer Formation Append")

#### Transform the Drone Scene
* Select the Mesh Object in the material collections, **Item** -> **Transform**. You could add keyframe of Loction, Rotation or Scale to make the animation of teh Mesh Object, so the Drone Scene can been transform.
* You could also deform the Object vertices or control points, or add Inherited animation(E.g armature) to the Object to make the animation. The Object has the animation, then the Drones has the animation.

## Land the Drones
* When we finish all the Drone Formations, **Begin** **Append** the drones to the **End Scene**, set the drones to the same location of the Begin Scene at Current Frame -> 1
* When **Append** the drones to the **End Scene**, remove the "√" infrom of the auto resign, so drones will land at the same position of takeoff. But we have to ensure the drones won't bump together.


## Direct Drone Led Color Change
* **Vehicle** -> **Led Maigc** -> **Preview** <br>
Select your target drones in **drones** Collection, select your color in color picker, click Preview button, drone color will be changed 
* Select all the drones in **drones** Collection, make a "√" in from of the **is linear**, click **Add KeyFrame** button, we will the drone led color linear change<br>
![Vimdrones Desiginer Drone Led Color](/static/add-color.jpg "Vimdrones Desiginer Drone Led Color")    
   * remove "√" in from of the **is linear**, then **Add Keyframe**. In the Timeline, we can see we have inserted two keyframes, it means that the color of drones suddenly change.

## Add Effector to change Drone Led Color
* Click the **effectors** Collection in the Outliner. In the 3D Viewport, select Menu Bar **Add** -> **Mesh**, select the effector shape you like.
* In the Properties Editor, select **Materials** tab, click **+ New** button to Add a new material. <br>
In the Surface Panel, click **Use Nodes** to remove the property(gary blackground means unselect). Then we could chosse any effector color you like.<br>
![Vimdrones Desiginer Effector Color](/static/effector-color.jpg "Vimdrones Desiginer Effector Color") 
* **Vehicle** -> **Effector** -> **Add** <br>
We add a Empty in the effectors Collection. In the Properties Editor, select **Object Data** tab, we can change the Dispaly of the Empty. Usually, we make the same shape and size of the Empty and the Mesh.<br>
![Vimdrones Desiginer Empty Display](/static/empty-display.jpg "Vimdrones Desiginer Empty Display") 
* First select the Mesh, then select the Empty.   
In the 3D Viewport, select Menu Bar **Add** -> **Object** -> **Parent** -> **Object** (Shift + P ). We can click the eye of the Mesh in the effector Collection to Hide the it.   
![Vimdrones Desiginer Effector Patent](/static/effector-parent.jpg "Vimdrones Desiginer Effector Patent") 
* When we transform the Empty, so the Mesh transform. Now we can add some animation to the Empty Effector. When the drones inside the Empty, the color these drones will be changed to the color of the Mesh. 
![Vimdrones Desiginer Effector](/static/effector.jpg "Vimdrones Desiginer Effector") <br>

* If we add more Effector to the drones at the same time, the color of drones will depend on the lastest Effector
![Vimdrones Desiginer Effector](/static/effector-video.gif "Vimdrones Desiginer Effector") 

## Collision Check of the drones 
* **Vehicle** -> **Flight Cheack** -> **Collision Check**, make a "√" in from of the **collision**  
When we transform the Drone Scene, we can use this tool to check whether the drones collide together. If the distance between two drones is less than 2 meters， the timeline will be stoped and pop up error message  
![Vimdrones Desiginer Drone Collision Check](/static/collision-check.jpg "Vimdrones Desiginer Drone Collision Check") 

## Speed Check of the drones 
* Open the Vimdrones Designer Console Software and play the animation in Blender, we will see the Current Frame, Fastest Drone, Fastest Speed and Closest Distance(between which two drones)
realtime.  
![Vimdrones Designer Console](/static/designer-console.png "Vimdrones Designer Console") 
* The average speed of the drones is 2m/s, the fastest Speed is not more than 8m/s.

## Export the Drone Light Show data
**Vehicle** -> **Export**, select the file

## How to design a Drone light  Show
1. Draw down your minds on the picture book
2. Creat Material Objects in the Blender
3. Through Begin and Append to transform the drone scene
4. Add animation to the Material Objects
5. Have a Flight check to the animation
6. Add color & effector to the drones
7. Export the Drone Light Show data

Tips: If we select a music for the drone light show background music at first, we can create drone light effects based on the beat of the music. The music data could influce the size or color of the Effector Object. So, it is very easy to grab every beat of music and let sound, light and electricity blend together perfectly.
![Vimdrones Designer Music Effector](/static/music-bar.gif "Vimdrones Designer Music Effector") 




