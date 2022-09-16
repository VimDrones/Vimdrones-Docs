## Introduction

Vimdrones Ground Control Station(GCS) Software could control thousands of drones in flight to have the drone light show. In GCS, open the Design Project(designed and exported in Vimdrones Designer) and upload the data to all drones. It could display real-time data on the drone's performance and position. When drone status is ready and setting parameters, click Takeoff to start our Drone Light Show.

**Feature Highlights**

* Easy Usage - Control thousands of drones just need one person
* Efficient Drone Dashboard
* Can run on multi PC for teamwork
* One click to take off and land
* RealTime 2D position view
* RealTime 3D position view
* Takeoff Countdown

## System requirements

System requirements for Ground Station Software:

* Operating system: Windows 10; Mac OS
* CPU: Intel Core i5 or better
* Memory: Minimum 8 GB of RAM or more
* Hard drive: SSD 120 GB. Recommended 256GB or more
* Network: TCP/IPv4 network stack, WiFi or Ethernet. Recommended Ethernet

Hardware requirements for Ground Station Software:
* Display Size at least 1280*800 pxl(at least 11 inch display)

## Installation
Install Vimdrones GCS on your computer, Mac OS or Windows

**Download**

* Open our website [Vimdrones](https://vimdrones.com/en/),click **Login**
* Already has an account, please **Sign In**. Don't have an account, Please **Sign Up** and then **Sign In**

![Vimdrones Designer Installation](/static/login.png "Vimdrones Designer Installation")  

* Select the version **Mac Os** or **Windows** to download the software

![Vimdrones Designer Installation](/static/download-software.jpeg "Vimdrones Designer Installation") 

**Mac**

* Double click the [Vimdrones_GCS-x.x.x.dmg], pull the **Vimdrones GCS icon** to the **Applications file**. 
* Double click the icon to open the Vimdrones GCS
![Installation Mac](/static/installation-gcs-mac.jpg "Installation Mac")

## Adding new Mazzy Star Drone™ to the system
By default the system shipped with pre config Mazzy Star Drone™, when you bought new Mazzy Star Drone™ in later orders to extend the business show scale, you will need to follow these steps to add it to current system

**Prepare**

* SD card (comes with drone, in the back position)
* SD card reader

**Make Drone Identification SD Card**

![Open SD Card Maker](/static/open-sd-card-maker.png "Open SD Card Maker")

* Open **SD Card Maker** from Tools
* Select SD card Device (click refresh, if you can not find it, also check whether it's mounted on your computer)
* Set Drone ID
* Set Wifi SSID (come with system document)
* Set Wifi Password (come with system document)
* Click **Make** button and pop up SD card

**Pair RC Transmitter**

* Click **RC Bind** button in Drone panel and see orange light flash inside the drone, press RC Transmitter bind button and power on the Transmitter, when heard a happy voice means it success 


**Pair 915/868 MHz or 2.4GHz Radio Channel**

![New Drone Setup](/static/new-drone-radio-bind.png "New Drone Setup")

* Insert SD card back to the drone
* Power up the drone, click **Radio Pair** button in Base panel and get "Drone X radio Pair Success" Notification

## Interface 

![Ground Station Interface](/static/gsc-interface-before-takeoff.png "Ground Station Interface")

**Top Bar**

![Ground Station Interface](/static/gcs-top.png "Ground Station Interface")

* Online: The number of drones online
* Open Realtime 3D View: Click to view drone's real time 3D position 
* Project: unselected -> the project name

**Drone Collection**

![Ground Station Interface](/static/gcs-drone-collection.png "Ground Station Interface")

* Top left number: Drone ID
* Top right number: Satellite Count
* Middle number: Drone's Heading Angle
* Left bar: Wifi Signal
    * High -> Low: Green -> Orange -> Red
* Right bar: Radio Signal
    * High -> Low: Green -> Orange -> Red
* Button bar: Battery Status
    * High -> Low: Green -> Orange -> Red
* Background color: 
    * Red: Ready
    * Green: Not ready


**Satellite Count**

![Ground Station Interface](/static/gcs-satellite-status.png "Ground Station Interface")

* Satellite Count: Show the count of Satellite
* Cylindrical bar: Satellite signal, the unit is DB
* Satellite name
* Satellite flag

**RTK Base Status**

![Ground Station Interface](/static/gcs-rtk-base.png "Ground Station Interface")

RTK Base: (Error) -> (Connected)   
iTow: Satellite time   
Survey In: (Not Start Yet) -> (Process) -> (Success)   
Acc: Accuracy<2m -> Survey In(Success)   

* Radio Pair: Pair 915/868 Mhz Radio Channel to drone and RTK base
* Survey In: When the RTK Base is enter, click **Survey In** button


**Drone Status**

![Ground Station Interface](/static/gcs-drone-status.png "Ground Station Interface")

When we click Drone ID on the **Drone Collection**, we could see the stats of this drone. We could see the ID No. and Online/Outline on the Drone Icon

**GNSS(Global Navigation Satellite System)**  
Satellite Count 
Fix Type: Normal -> DGPS -> RTK Float -> RTK Fix(Ready to takeoff)  
HDOP: Horizontal dilution of precision 

* Poor -> Good: Red -> Orange -> Green 

VDOP: Vertical dilution of precision  

* Poor -> Good: Red -> Orange -> Green

**Global Position**  
lat: Latitude  
lon: Longitude  
alt: Altitude   
relative alt: Relative Altitude 
  

**Status Check**  
GNSS: False -> Ready  
Mode: False -> Ready  
Arming: False -> Ready  
Wifi Channel: OFF/ON   
Radio Channel: OFF/ON  


**Drone Status**  
RTCM:  Sending Frequency

* RTCM Version V3 , provide broadcasted GNSS real-time differential corrections and raw
data

Mode:    

* 0 Stabilize: Drone is flying by Remote Control  
* 1 Altitude hold: Drone is flying by Remote Control
* 2 Guided:  Drones are flying by autopilot
* 3 RTL: Automatically return to home position
* 4 LAND: Automatically landing in current position


HEADING: Drone's heading angle degrees against north  
IP: Drone's ip address in network


**Vibration Status**  
When in the guided mode or manual control by RC, please check in the GCS  
    --Drone X/Y/Z axis Vibration value should be under 30   
    --Clip value should be under 50 | 200 |   
Otherwise may have propeller/motor broken issue!         

**Battery Status**  
Voltage: When the voltage drops to 7.2V, the drone will automatically return to launch  


**Trajectory**  
Status: False -> Ready   
Token: The same as the Project Token


**Button**   



* Reboot (Reboot the drone)
* Mag Cal (drone mag calibration) 
* ESC Cal (drone esc calibration)
* Motor Test (drone motor testing)
* RC Bind (binding drone to the RC controller)
* Rescue (Enable drone's RC control to manual control by RC controller)
* RTL (Set drone to RTL mode)
* Land (Set drone to LAND mode)
* Upload (Upload single trajectory design to the drone)




---
**Project**

![Ground Station Interface](/static/gcs-project-data.jpg "Ground Station Interface")

Current: The current project name   
Rotation: The current project Rotation status   
Music: The current project music name    
Token: The project token  
Qty: The quantity of drones   
Time: The drone light show duration

* Open: Click **Open** button, Select Design Project 
* Upload: Click **Upload** button, upload trajectory Design to the drones (white light flashing) 
* Upload: Click **Upload(skip success)** button, upload trajectory Design to the drones which 

**Set Home**

![Ground Station Interface](/static/gcs-set-home-data.png "Ground Station Interface")

lat/lon/alt   

* Copy From Drone: When Drone Status Check Pass, select Drone 1, click **Copy From Drone** button, copy drone 1 location, it shows the latitude(lat), longitude(lon) and altitude(alt) of Drone 1  
* Set Home: Click **Set Home** button, set home location to all drones (LED lights change to green, mean the drones are ready to fly) 


**Log System**

![Ground Station Interface](/static/gcs-log-system.png "Ground Station Interface")

It shows the select drone's log system


**LED Control**

![Ground Station Interface](/static/gcs-led-control.jpg "Ground Station Interface")

Select the color, set the diffuse color(LED brightness), click **Update** icon. We could control the LED Control Realtime when having the drone light show.

Light Mode：  
1. Long  
2. Breath  
3. Flash  
4. Quick  

**Takeoff**  

![Ground Station Interface](/static/gcs-takeoff.png "Ground Station Interface")

* Reboot All: Reboot all the drones
* Land: The drones will automatically landing in current position (do not click it unless you know what it is!)

* Turn On: Click the time to set the takeoff time, then click the **Turn On** button to finish the setting. The **Turn On** button will change to **Turn OFF** button, you could it to shut down the countdown setting.  
* Takeoff: When everything id Ok, Click the **Takeoff** button to begin your drone light show


**Overview**  
![Ground Station Interface](/static/gcs-overview.jpg "Ground Station Interface")

**PreArm Fail:** The drone Fail to PreArm(takeoff). Please check LOG system of fail drones. The refresh rate of PreArm fail is 1 minute. 
**Token Fail:** The drone'project upload fail or Empty. Please try to upload(skip success) again. 
**RTK Fail:** The drone is not RTK fixed yet. Please wait for RTK fixed.  
**Set Home Fail:** Please set home again.  


## Settings

![Ground Station Interface](/static/gcs-setting.jpg "Ground Station Interface")  

* **Safe Fence**  
* **Grid Settings**  
* **RTK Settings**  


---

## Realtime 2D position view
Click **Map** to view drone's real time 2D position 
When you click the drone in the view, it will show its Status in the map
![RealTime 2D position view](/static/gcs-map.jpg "RealTime D position view")


---
## RealTime 3D position view
Click **3D** to view drone's real time 3D position 

![RealTime 3D position view](/static/real-time-3d-position-view.png "RealTime 3D position view")



## Takeoff Countdown 
* Click the time In the lower right corner, set the takeoff time
* Click the **Turn On** button, then it begin to countdown. Drones will takeoff when reach the set time
    * If the set time is less than now, it will give you a notice.
    * You could Turn off the countdown before the set time  

![Takeoff Countdown Setup](/static/coundown-setup.png "Takeoff Countdown Setup")

**Operation Video**

* [YouTube](https://youtu.be/nBi81nieGS8)
* [bilibili](https://www.bilibili.com/video/av87958242/)

<iframe width="560" height="315" src="https://www.youtube.com/embed/nBi81nieGS8" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
