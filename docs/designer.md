## Introduction

The Vimdrones Designer is an Add-on of Blender that uses for Dorne Light Show Flight Path Design. It could create any figures, like 2D or 3D animation, even with music beats. For its efficiently handling the transformation between drone formations and lighting effects, we could focus more on the drone light show design itself. 

**Feature Highlights**

* One-click Formation
* Smart Formation Transform
* Flight Check to Avoid Collision
* 3D Animation
* Rich Color Design
* Support Multiple file formats Import
* With Sound Track System to Synchronize
* Music and Light
* Easy Marketing Design

## System requirements

System requirements for Vimdrones Designer Software:

* Operating system: Windows 8; Windows 10; Mac OS
* CPU: Intel Core i5 or better
* Memory: Minimum 8 GB of RAM or more
* Hard drive: SSD 120 GB. Recommended 256GB or more
* Network: TCP/IPv4 network stack, WiFi or Ethernet. Recommended Ethernet


## Installation
* Install [Blender 2.8](https://www.blender.org/download/) on your computer, Mac OS or Windows
* [Get Your Designer Software](https://vimdrones.com/en/products/7125cd54-c5ff-48b9-9e5c-bddf17875926--Vimdrones-Drone-Light-Show-Designer-Software)

**Download**

* Open our website [Vimdrones](https://vimdrones.com/en/),click **Login**
* Already has an account, please **Sign In**. Don't have an account, Please **Sign Up** and then **Sign In**

![Vimdrones Designer Installation](/static/login.png "Vimdrones Designer Installation")  

* Select the version **Mac Os** or **Windows** to download the software

![Vimdrones Designer Installation](/static/download-software.jpeg "Vimdrones Designer Installation") 


**Mac**

* Double click the [Vimdrones Designer-x.x.x.dmg], pull the **Vimdrones Designer icon** to the **Applications file**. 
* Double click the icon to open the Vimdrones Designer  
![Vimdrones Designer Installation](/static/installation-mac.jpg "Vimdrones Designer Installation")  


## Active License
* Type your emaiL and token, click **Active** Button
![Vimdrones Designer Active License](/static/active-license.png "Vimdrones Designer Active License")
    *  Click [DOCUMENT](https://docs.vimdrones.com/gcs) to open Vimdrones Designer Doc
    *  Click [ABOUT](https://vimdrones.com/) to open our official website


* Click the file icon on the Upper right corner to open the Blender Path where you installation 
* Then click **OPEN BLENDER** Button  
![Vimdrones Designer Open Blender](/static/open-blender.jpg "Vimdrones Designer Open Blender")    
    *  Click **LOGOUT** to logout   
    *  Click **CONSOLE** to open the flight check console
  
* Press **N** to show/hide **Properties**
![Vimdrones Designer Open Blender](/static/blender_interface.jpg "Vimdrones Designer Open Blender")
  
## Getting started Blender
* Open Blender 2.8, **New File** -> **General**
* Press **A** to select all the objects in the 3D Viewport, then press **X**, **D** to delete the objects

More details about [Keymap](https://docs.blender.org/manual/en/latest/interface/keymap/blender_default.html)

**From Blender To Real World**  

* Blender and Real World axis relationship shown as below
![Vimdrones Designer Geo Basic](/static/geo-basic.png "Vimdrones Designer Geo Basic")  
     ![Vimdrones Designer Geo Basic](/static/drone-placement-direction.jpg "Vimdrones Designer Geo Basic")

* drone light show design is based on 24 FPS which means 1s run 24 frames, this value should not be changed unless you know what you are doing


## Create Drone Team
* **Vehicle** -> **New Team** -> **Create**
![Vimdrones Designer Create Drone Team](/static/create-drone-team.png "Vimdrones Designer Create Drone Team")

**What is x qty, y qty, qty mean?** <br>

qty represent the total quantity of your drone team <br>
x qty and y qty define your a single block shape in ground, as the image shown below 
![Vimdrones Designer Drone Team Params](/static/drone-team-parms.png "Vimdrones Designer Drone Team Params")

**what is the distance**   

* Distance between two drones, the default value is 2m. 

**What we have after create drone team?**  

* drones Collection ([What is Collection?](https://docs.blender.org/manual/en/latest/scene_layout/collections/collections.html))
* distance checker Collection(quick preview for min distance between drones)
* effectors Collection
* Begin Scene Collection
* End Scene Collection

**How to set the LED glow strength?**  

* **Led** -> **Settings**, set the strength value, click **update**. The higher the value, the stronger the glow 

**How to remove the LED glow?**  

* If your computer configuration is not high, we suggest you to remove LED glow effect
* **Led** -> **Settings**, remove the "√" in from of use_nodes, then click **update**  
![Vimdrones Designer Create Drone Team](/static/create-drone-team-no-use-node.png "Vimdrones Designer Create Drone Team")

**Pay attention(very important!)** 

 Once you select use_nodes to start a project, don't change it to no use_nodes. Similarly, once you select no use_nodes, don't change it to use_nodes. These two modes are not compatible in a same project.

**Operation Video** 

* [YouTube](https://www.youtube.com/watch?v=J3wu86SJ_ho&t=9s)  
* [bilibili](https://www.bilibili.com/video/av87493547/)

<iframe width="560" height="315" src="https://www.youtube.com/embed/J3wu86SJ_ho" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>  

---


## Takeoff the Drones
* In the [Timeline](https://docs.blender.org/manual/en/latest/editors/timeline.html) window, Current Frame -> 0 <br>
  **Formation** -> **Append**, select formations **Begin Scene**, click **Begin** Button
* Current Frame -> 1 <br>
  **Formation** -> **Append**, select formations **Begin Scene**, click **Append** Button <br> 
  (the drones are reach the location of the Empty Objects, and they will follow the animation of the Empty Objects)
* Select Empty Objects in the Begin Scene Collection, insert [keyframe](https://docs.blender.org/manual/en/latest/animation/keyframes/index.html)
* Set the Current Frame -> 600 (for example; 600 means 25s, press Ctrl/Command T to change time form)<br> 
  Move the Empty Objects to Z:50m (for example), insert keyframe

What is Begin and Append

* **Begin**: The frame that the drones begin to change the formation
* **Append**: The frame that the drones reach the location of the new formation(Empty Objects collection)

**Operation Video** 

* [YouTube](https://youtu.be/Y_rdntjSmb8)  
* [bilibili](https://www.bilibili.com/video/av87541449/)

<iframe width="560" height="315" src="https://www.youtube.com/embed/Y_rdntjSmb8" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe> 

---


## Change Drone Formation

**Create Drones Vertex Group**

* Select the Mesh Object(E.g **Cube**),change **Object Mode** to **Edit Mode**
* In the **Properties** Editor, click **Object Date** tab, click the Button "+" on the right Panel border to add a [Vertex Group](https://docs.blender.org/manual/en/latest/modeling/meshes/properties/vertex_groups/assigning_vertex_group.html), double-click the "Group" name and edit to "drones"
* Select the vertices of the Mesh Object (one vertex represents one drone), click **Assign** Button below the Panel<br> 
![Vimdrones Designer Add Vertex Group](/static/vertex-edit.jpg "Vimdrones Designer Add Vertex Group")
    * We could use the tools on the left to edit the vertices. Or from the Menu Bar **[Vertex](https://docs.blender.org/manual/en/2.81/modeling/meshes/editing/vertices.html#)** to edit the vertices. <br> 
    Add the vertices:[Loop Cut](https://docs.blender.org/manual/en/2.81/modeling/meshes/editing/subdividing/loop.html#tool-mesh-loop-cut) is a very useful tool.<br> 
    Delete the vertices: Select the vertices, press **X** key to Delete or [Dissolve the vertices](https://docs.blender.org/manual/en/2.81/modeling/meshes/editing/basics/deleting.html?highlight=delete%20vertex).

    * We could know how many vertices have been Assigned on the Status Bare(lower right corner)
![Vimdrones Designer Vertex Number](/static/vertex-number.jpeg "Vimdrones Designer Vertex Number")
    * In the Vertex Group Panel, we could click the **Remove** Button to remove the vertices which have been Assigned. And we could click the **Select**/**Deselect** Button to check which vertices have been Assigned.

* Change **Edit Mode** to **Object Mode**




**Change the Drone Scene**

* **Formation** -> **New Formation**, select the Formations Scene(E.g **Begin Scene**) which need to be changed, then click the **Copy** Button to copy a **New Formation** at in same location. Double-click the **New Formation** in the outline Editor to edit the name(E.g **Cube Formation**)
* **Formation** -> **New Material Collection** -> **New**, create New Material Collection in the outline Editor. Double-click the collect to rename it(E.g **Cube Material**)
* Select the Mesh Object(E.g **Cube**) which has the Drones Vertex Group, move it to the Material Collection(E.g **Cube Material**)
    * We could add more Mesh Objects to the Material Collection. These Mesh Objects should also have **drones** Vertex Group. That's much easier for us to design the drone scene.
    * **File** -> **[Append](https://docs.blender.org/manual/en/latest/files/linked_libraries/introduction.html)/[Import](https://docs.blender.org/manual/en/latest/files/import_export.html)**  
    We can append/import the objects from other files and use them as the Material of drone scene. For example, if we import svg. files, we should convert them to Mesh(**Object** -> **Convert to** -> **Mesh from Curve/Meta/Surf/Text** in the Menu bar)
* **Formation** -> **Vertex Formation**, select the formation(E.g **Cube Formation**) and its corresponding material_collections(E.g **Cube Material**). Click the **Append** Button. The Empty Objects in the formation will reach the location of the "drones" Vertex Group

What's the **Append** mean in here?  
The Empty Objects in the select formation will copy the location of the vertices in the "drones" group of the select Material 

![Vimdrones Designer Formation Changing](/static/formation-changing.jpg "Vimdrones Designer Formation Changing")

* In the Timeline Editor, set up the Current Frame to begin the new scene<br>
**Formation** -> **Append**, select formations(E.g **Cube Formation**) , click **Begin** Button
* In the Timeline Editor, set up the Current Frame to finish the new scene changing<br>
**Formation** -> **Append**, click **Append** Button. Move the Playhead, we could see how the drone scene change(make sure the **auto resign** have been "√")

![Vimdrones Designer Formation Append](/static/append-3d-eagle.gif "Vimdrones Designer Formation Append")


**Transform the Drone Scene**

* Select the Mesh Object in the material collections, **Item** -> **Transform**. You could add keyframe of Location, Rotation or Scale to add animation of teh Mesh Object, so the Drone Scene can be transformed.
* You could also deform the Object vertices or control points, or add Inherited animation(E.g armature) to the Object to make the animation. The Object has the animation, then the Drones have the animation.

More details about [Animation](https://docs.blender.org/manual/en/latest/animation/introduction.html)

**Operation Video** 

* [YouTube](https://youtu.be/hvQPp3ziviU)  
* [bilibili](https://www.bilibili.com/video/av87798888/)

<iframe width="560" height="315" src="https://www.youtube.com/embed/hvQPp3ziviU" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe> 

---


## Smart Land
![Vimdrones Designer Drone Smart Land](/static/smart-land.jpg "Vimdrones Designer Drone Smart Land")

* **Formation** -> **New Formation**   
Copy the **Begin Scene** as the **End Formation**. If we don’t set the time frame, it will copy its last status. Adjust the location and Scale of the **End Formation**. It needs below the last scene in the view.  
* **Formation** -> **Smart land**  
Select the **begin_formations** as the last scene of the show. Select the **End_formations** as the **End Formation**. Click **Create Safe Queues** Button. When the calculation is finish, it shows the INFO: “? safe queues create(? means the Quantity)” and “Calculation processing. It will take a while”. The larger the Scale of End Formation, the smaller of the quantity of safe queues create. It also create two new Collections: **Smart Landing Path**(show the path of landing) and **Smart Landing Formation**(copy the location of last scene). Set the time frame to **Begin** and **End** the **Smart Landing Formation**. The Empties of the **Smart Landing Formation** will follow the path to the **End Formation**.  
* **Formation** -> **Append**   
Before begin Smart Landing Formation, set the time frame to **Begin** and **Append** the **Smart Landing Formation**. We must remove the “√” on from of **auto resign**. So the drones will append the The Empties in order. Now the drones will follow the path to the End Formation. We could still adjust the **Smart Landing Formation** in Timeline.  
* Finally, we copy the **Begin Scene** at frame 1 as **Land Formation**. **Formation** -> **Append**, set the time frame to **Begin** and **Append** the Land Formation.  

**Operation Video** 

* [YouTube](https://youtu.be/hvQPp3ziviU)  
* [bilibili](https://www.bilibili.com/video/BV1bZ4y1j7Lj/)

<iframe width="560" height="315" src="https://www.youtube.com/embed/nOcmqNEDKWg" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe> 

---



## Add Color to Drones
* **Led** -> **Led Magic** -> **Preview** <br>
Select your target drones, select the color you like in color picker, click **Preview** Button, the drones color will be changed. (Select other drones, same operation as above)
* Select all the drones in **drones** Collection, make a "√" in from of the **is linear**, click **Add KeyFrame** Button, we will the drone led color linear change<br>
![Vimdrones Designer Drone Led Color](/static/add-color.jpg "Vimdrones Designer Drone Led Color")
   * remove "√" in from of the **is linear**, then **Add Keyframe**. In the Timeline, we can see we have inserted two keyframes, it means that the color of drones suddenly change.

**Operation Video** 

* [YouTube](https://youtu.be/zKzyAkC0M3o)  
* [bilibili](https://www.bilibili.com/video/av88039381/)

<iframe width="560" height="315" src="https://www.youtube.com/embed/zKzyAkC0M3o" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe> 

---



## Add Effector to Drones

**Add Effector Color**

* Click the **effectors** Collection in the Outliner. In the 3D Viewport, select Menu Bar **Add** -> **Mesh**, select the effector shape you like.
* In the Properties Editor, select **Materials** tab, click **+ New** Button to Add a new material. <br>
In the Surface Panel, click **Use Nodes** to remove the property(gary background means unselect). Then we could choose any effector color you like.<br>
![Vimdrones Designer Effector Color](/static/effector-color.jpg "Vimdrones Designer Effector Color") 


**Add An Empty Object to Parent with effector shape Mesh**  
(This part could be skipped, it isn't affect the final effect)

* **Led** -> **Effector** -> **Add** <br>
We add a Empty in the effectors Collection. In the Properties Editor, select **Object Data** tab, we can change the Display of the Empty. Usually, we make the same shape and size of the Empty and the Mesh.<br>
![Vimdrones Designer Empty Display](/static/empty-display.jpg "Vimdrones Designer Empty Display") 
* First select the Mesh, then select the Empty.   
In the 3D Viewport, select Menu Bar **Add** -> **Object** -> **Parent** -> **Object** (Shift + P ). We can click the eye of the Mesh in the effector Collection to Hide the it.   
![Vimdrones Designer Effector Patent](/static/effector-parent.jpg "Vimdrones Designer Effector Patent") 


**Transform Effector**  

* When we transform the Empty Effector, so the Mesh transform. Now we can add some animations to the Empty Effector. When the drones inside the Empty, the color of these drones will be changed to the color of the Mesh. 
![Vimdrones Designer Effector](/static/effector.jpg "Vimdrones Designer Effector") <br>

* If we add more Effectors to the drones at the same time, the color of drones will depend on the latest Effector
![Vimdrones Designer Effector](/static/effector-video.gif "Vimdrones Designer Effector") 

**Operation Video** 

* [YouTube](https://youtu.be/e1_7dmeRi2c)  
* [bilibili](https://www.bilibili.com/video/av88166427/)

<iframe width="560" height="315" src="https://www.youtube.com/embed/e1_7dmeRi2c" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe> 

---


**Set the Effector LED Type**

* What are the types of the Effector LED?
    * DEFAULT: one color
    * RANDOM: two or more different colors change randomly
    * ORDERED: two or more different colors change in order  
![Vimdrones Designer Effector](/static/effector-type.png "Vimdrones Designer Effector") 
    * duration: the higher the value, the faster the color changes
    * linear: two color change gradual，if remove the "√" ,two colors change suddenly 
    * order: if the drones are inside two or more Effectors at the same time, we could set the valve to change the effector order. The higher the value, the higher the priority is to affect the color of the drone.

* Select the effector mesh, add one or more material and set the colors
* **Led** -> **Effector**
* Choose selected_effector, set the duration, if linear, set the order, choose effector type
* Click update
* Play the animation

**Operation Video** 

* [YouTube](https://youtu.be/6l_fUSTwbMQ)  
* [bilibili](https://www.bilibili.com/video/av88538932/)

<iframe width="560" height="315" src="https://www.youtube.com/embed/6l_fUSTwbMQ" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe> 

---


## Flight Check

* **Vehicle** -> **Flight Check**, make a "√" in from of the **enable**  
![Vimdrones Designer Drone Flight Check](/static/flight-check.jpg "Vimdrones Designer Drone Flight Check") 

* Open **Vimdrones Designer**, Click **CONSOLE**, open the **Vimdrones Designer Console**

* we could set the Distance Limit, Speed Limit, Horizon Speed Limit, Vertical Speed Limit and Chart Duration, then click the **Update Settings** Button

* Play the animation in Blender, we will see those Limits realtime. When the value reach the Limits, it will appears in the window. It shows that two drones reach the limit at that frame  
When we don't need those information, we could click the **Clear** Button
![Vimdrones Designer Console](/static/designer-console.png "Vimdrones Designer Console") 

**Operation Video** 

* [YouTube](https://youtu.be/sy3q5i0HcNo)  
* [bilibili](https://www.bilibili.com/video/BV1QK411L72L/)

<iframe width="560" height="315" src="https://www.youtube.com/embed/sy3q5i0HcNo" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe> 

---


## Export Animation

![Vimdrones Designer Export](/static/export-panel.png "Vimdrones Designer Export") 

**Export Settings**

* Position Scale: scale factor to coordinate, default is 1, if you want to change the pattern size this would help (do not change it unless you know what it is!) 
* Z Axis Rotate: rotate degree in clockwise to coordinate, default is 0, if your flight field direction is different from your design, this would help (do not change it unless you know what it is!) 

**Export To Vimdrones GCS**

* **Vehicle** -> **Export** click Export button and select the your folder to save

**Export To Third Party Fly System**

* **Vehicle** -> **Third Party** Export button and select the your folder to save

* Support List

| Company        | Name           | Scene |  Sample Path  |
| ------------- |:-------------:| :-----:| :-----:|
| None      | Raw Format | Custom | <a download href="/static/third_party_path/vimdrones-third-party_-path-raw-format.zip">Download</a> |
| Ugcs      | Drone Show Software | Outdoor | <a download href="/static/third_party_path/vimdrones-third-party_-path-raw-format.zip">Download</a> |
| High Great | Fylo    | Indoor | <a href="#">Download</a> |

What to add your system to the list? please [contact us](https://vimdrones.com/contact)

Sample Path Video [Youtube](https://www.youtube.com/watch?v=N5A8r9rXA68&t=9s) | [Bilibili](https://www.bilibili.com/video/av79197730)
<iframe width="560" height="315" src="https://www.youtube.com/embed/Ax7skeVCrL0" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

* Raw Data Format

1.txt  -> drone id 1, fps equal blender settings
```
1 0.000 0.000 0.000 204 194 40
2 0.000 0.000 0.094 204 194 40
3 0.000 0.000 0.188 204 194 40
```
| frame number | x | y | z | r | g | b |

## How to design a Drone Light Show
1. Draw down your minds on the picture book
2. Create Material Objects in the Blender
3. Through Begin and Append to transform the drone scene
4. Add animation to the Material Objects
5. Have a Flight check to the animation
6. Add color & effector to the drones
7. Export the Drone Light Show data

Tips: If we select a music for the drone light show background music at first, we can create drone light effects based on the beat of the music. The music data could influences the size or color of the Effector Object. So, it is very easy to grab every beat of music and let sound, light and electricity blend together perfectly.
![Vimdrones Designer Music Effector](/static/music-bar.gif "Vimdrones Designer Music Effector") 
---

## Example

**Example 1: Add Line Font Text**

**Installation**

* Download [addstrokefont_2_8.zip](https://github.com/Shriinivas/blenderstrokefont)  
* Open Blender and select File->User Preferences  
* Click install Add-ons tab and then Install Add-on from File  
* Select the downloaded file  
* Make a “√” in front of the Add-on 
* Check the ‘Add Stroke Font Text’ option in the add-ons dialog  

**Add line font text**

* Add a Mesh
* Select ‘Add Input Text’ option in the ‘Action’ drop-down
* Input the text to be rendered in the text box
* Select the font
* Set Font Size
* Select the Mesh in the properties of box
* Select the font and click ‘Add Stroke Font Text

**Operation Video** 

* [YouTube](https://youtu.be/ZhzBpmudwIo)  
* [bilibili](https://www.bilibili.com/video/av96248595/)

<iframe width="560" height="315" src="https://www.youtube.com/embed/ZhzBpmudwIo" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe> 

---

**Example 2: Add Text**

* Open Blender through Vimdrones Designer. A -> X -> D, delete all the objects
* Add -> Text, we could see Text in the 3D view. R -> X -> 90 (Rotate 90 ° along the X axis)
* Change to Edit mode, delete and enter text
* Click Object Data Properties tab, Font -> Open Font, open the file to set the font. Geometry -> Extrude. Font -> Transform -> Size  
* Change to Object mode, Object -> Convert to -> Mesh from Text
* Click Modifier Properties tab, Add Modifier -> Remesh. Remove the “√” of Remove Disconnected Pieces. We could set the Octree Depth & Scale. Click Apply the Modifier

**Operation Video** 

* [YouTube](https://youtu.be/3Mx-XTYJFS4)  
* [bilibili](https://www.bilibili.com/video/BV18E411w7Ls/)

<iframe width="560" height="315" src="https://www.youtube.com/embed/3Mx-XTYJFS4" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe> 

---
**Example 3: Add QR code drone formation**

* Online Generate the QR code. Download the QR code image.   
  [QR Code generator](https://www.unitag.io/qrcode)
* Open Blender in Vimdrones Designer. Add -> Empty -> Image. Click Object Data tab in the Properties window. Open and browse to your image
* Add -> Mesh -> Plane. Choose Display the Object as wire edges. Scaling the QR code makes it as big as Plane. Press tab to Edit Mode. Loop Cut the Plane and make one edge correspond to a row/column of dots
* Now we could add a drones Vertex Group. Select those vertices on the QR code dots and Assign the vertices to the drones Vertex Group. Add a New Material Collection and rename it as QR code. Drag the Plane to the QR code Collection. Save the Blender file.
* File -> Append, append the QR code Collection to Blender which it’s designing the show. We to start to make the QR code drone formation.

**Operation Video** 

* [YouTube](https://youtu.be/wfewJdC3OhE)  
* [bilibili](https://www.bilibili.com/video/BV1k54y1Q77C/)

<iframe width="560" height="315" src="https://www.youtube.com/embed/wfewJdC3OhE" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe> 