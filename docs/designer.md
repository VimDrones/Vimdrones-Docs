## Installation
* Install [Blender 2.8](https://www.blender.org/download/releases/2-80/) on your computer, Mac OS or Windows
* [Get Your Designer Software](https://www.vimdrones.com/contact)
* In Blender 2.8 Edit -> Preferences -> Install, Select downloaded Designer Software .zip

## Active License
* Select License Tab, type your email, token and click Active Button
![Vimdrones Desiginer Active License](/static/active-license.png "Vimdrones Desiginer Active License")

## From Blender To Real World
* Blender and Real World axis relationship shown as below
![Vimdrones Desiginer Geo Baisc](/static/geo-basic.png "Vimdrones Desiginer Geo Baisc")

* drone light show design is based on 24 FPS which means 1s run 24 frames, this value should not be changed unless you know what you are doing

## Create Drone Team
* Vehicle -> New Team -> Create
![Vimdrones Desiginer Create Drone Team](/static/create-drone-team.png "Vimdrones Desiginer Create Drone Team")

* What is x qty, y qty, qty mean? <br>
qty represent the total quantity of your drone team <br>
x qty and y qty define your a single block shape in ground, as the image shown below 
![Vimdrones Desiginer Drone Team Params](/static/drone-team-parms.png "Vimdrones Desiginer Drone Team Params")

* What we have after create drone team? <br>
    * drones Collection
    * distance checker Collection(quick preview for min distance between drones)
    * effectors Collection
    * Begin Scene Collection
    * End Scene Collection

## Direct Drone Led Color Change
* Vehicle -> Led Maigc -> Preview <br>
Select your target drones in drone Collection ([What is Collection?](https://docs.blender.org/manual/en/latest/scene_layout/collections/collections.html)), select your color in color picker, click Preview button, drone color will be changed 
