
## Mazzy Star Drone Introduction
Mazzy Star Drone is designed for drone light show, featuring a full-colour RGB LED, intelligent flight mode and high precision positioning system. It equips with RTK GPS positioning system and multiple control channels communication system to ensure a stable and safe formation flight.
Mazzy Star Drone has full size propeller guard and only 0.46kg armed weight. The maximum time hover time is up to 18 minutes. For the revolutionary design, Mazzy Star Drone significantly reduce safety risks compared to other drones on the market.

[Drone Light Show Play list](https://youtube.com/playlist?list=PL0yTwW_bnpPIzh5wLbhtXvQPJ0GY6Isgl)

<iframe width="560" height="315" src="https://www.youtube.com/embed/Lm-ZsTvbPis" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

</br>

**Feature Highlights**

* Compact, durable and light airframe, full-size propeller guard
* Only 0.46kg armed weight, up to 18-min flight time
* Full-colour RGB LED in high brightness, up to 640LM
* Ground control software with Realtime 3D video preview
* High precision RTK GPS, 2 cm precision with RTK fixed
* Radio transmit, 915MHz/868MHz/2.4GHz, 3km Long Range Control
* WIFI transmit, 2.4G, 120m Long Range Control
* Remote Control, 2.4G, 1km distance
* Drone light show Ground Control Station Software “Vimdrones GCS” --with efficient drone dashboard, Realtime 2D&3D video preview, enables flexible configuration and development
* Drone light show design software “Vimdrones Designer”--Blender Add-on

**Aircraft Diagram**

![Mazzy Star Drone](/static/aircraft.png "Mazzy Star Drone")

**Technical Specifications**

<style>
table th:first-of-type {
    width: 22%;
}
table th:nth-of-type(2) {
    width: 78%;
}
</style>

| Drone Specs        |Details           |
| : --------------------- |:-------------|
| Airframe      | Compact, durable and light airframe, full size propeller guard | 
| Weight      | 460± g with 2S 3000mAh battery |
| Body Dimension | 340x340x80 mm | 
| Motor and Prop | 2300 kV brushless motors; 6 inch carbon fiber propeller |   
| Max Hover Time | 18mins |
| Wind Resistibility | < 7 m/s |   
| Positioning System | RTK GPS (GPS+GLONASS+Beidou), 2 cm precision with RTK fixed |  
| Battery | LiPo2S, 7.6V, 3000-mAh |  
| Remote Control | 6-channel 2.4G radio remote controller (1km distance, optional) |  
| Ground Antenna | 915MHz/868MHz/2.4GHz 1000 mW, communication range 3km |
| Drone Antenna | 915MHz/868MHz/2.4GHz 20 mW, communication range, 2km <br>2.4G, communication range, 120m |
| LED | Integrated full-color RGB LED, 4W |
| Charger | high-power 2S LiPo battery balance charger <br>10 charging holes <br>Input: AC100~240V 50/60Hz,3A(Max) <br> Output: DC8.7 V 1.5A 10 groups | 
| Accessory | Foam box 1 (420x420x148mm) |  


## Ready To Fly List
* Mazzy Star Drone
* Mazzy Star Drone Battery
* Mazzy Star Drone Battery Charger
* Vimdrones Drone Light Show System     
    * 1 Vimdrones Smart RTK Base Station
    * 1 Wifi Router, 220V
    * 1 Spektrum Transmitter 
    * 1 Tripod
    * 1 915MHz/868MHz/2.4GHz Antenna
    * 1 Feeder
    * 1 PoE power supply, 220V 
    * 3 Network Cables
* Vimdrones Drone Light Show Designer Software
* Vimdrones Ground Station Software

![Ready To Fly List](/static/drone-light-show-equitment.jpg "Ready To Fly List")

**Other Additional Equipment**    

* May need 220V power supply from mobile power bank  
* Some of the Power Strips  
* A set of foldable desk and chair (would be very good) 

Download <a href="/static/vimdrones-drone-light-system.pdf" target="_blank" >Vimdornes Drone Light Show System.pdf</a>


</br>

## Pre-Flight Preparation
* Battery preparation
    * Please prepare a sufficient number of batteries（more than the number of drones）
    * Please charge the battery fully（according to the flight time, the voltage is at less 8.2V)    

**Here are some tips for using batteries at low temperatures**
1. Make sure the battery is fully charged before the flight.
2. Fully preheat the battery to over 20 degrees.   
3. Battery preheaters are recommended.

* Drone preparation
    * Please check the number the drones 
    * Please check the airframe of the drones, especially for the propeller guard, propeller and the motor    

    How to check the propeller/motor?
    When in the guided mode or manual control by RC, please check in the GCS.  
    GCS -> Vibration Status  
    --Drone X/Y/Z axis Vibration value should be under 30  
    --Clip value should be under 50 | 200 |  

<//br>

* Flight Path preparation
    * Export *Vimdrones GCS*  flight **project**   
    Use Vimdrones Designer to design the Flight path, save the .blend file and export the *Vimdrones GCS* flight data


    * **Usage Warming:**   

    Do not let the drone collide when design the Flight path. It is recommended that the distance between drones is above 2m. If the distance is larger, the formation looks more stable. If the distance is close, the airflow generated by the drone will affect each other.      

    Do not let the drone exceed the speed limit when design the Flight path   
    1. Max Horizontal Velocity (Up To) is 4m/s  
    2. Maximum Descent Speed (Up To) is 3m/s  
    3. Maximum Ascent Speed (Up To) is 5m/s   
    4. It is recommended that the flying speed of the drone is below 5m/s  
    5. It is recommended that the takeoff/landing speed of the drone is below 2m/s   

    Do not let the drone beyond the fence when design the Flight path   
    1. Height: 120m  
    2. Radius: 500m  

    When the drone takes off at an altitude of about 5 meters, it will start to execute the flight path and quickly fill in the altitude. It is recommended to take off as a whole, or take off in a row. Of course, it’s not a problem to turn into graphics after takeoff, as long as it doesn’t reach the restricted speed and distance



**Warming:**    
If it is raining, snowing or the wind speed is above 7m/s（bad weather）, please stop the drone light show.

</br>


## Pre-Flight Setup Procedure

**Drone Light Show System Communication:**  

* Power the wifi router, connect the wifi router and PoE power supply with a network cable 
* Place the tripod，setup the RTK Base and the antenna, use the Feeder to connect the RTK Base and the antenna
* Connect the RTK Base to PoE power supply with a network cable  (so the wifi router can communicate with the RTK base)
* Power the RTK Base through the PoE power supply
* Place the Remote Controller(Backup)

**Pay attention!!!**   
Please first power the wifi router, then long press the button to turn on the RTK Base. It will make sure the GCS works properly on the computer.

![Drone Light Show System](/static/drone-light-show-system-communication-diagram.jpg "Drone Light Show System") 

**Operation Video**

* [YouTube](https://youtu.be/iSv-nGm3Wn8)
* [bilibili](https://www.bilibili.com/video/BV1Xz411e7Wh/)

<iframe width="560" height="315" src="https://www.youtube.com/embed/iSv-nGm3Wn8" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
----

**Drone Light Show System Layout:**  

* According the design to place and locate drones
* Insert the batteries to the drones, but not power the drones   

**Usage Warning:**  

* Do not have the show near people too close or over people’ head   
* Should have the show in an open space without high obstacles   
* Should make sure of good order inside the venue without any interference or disruption when having the show  

Drone layout: 
![Drone Light Show System](/static/drone-layout.jpg "Drone Light Show System") 

-----

When change in Z Axis Rotate in Vimdroens Designer(Real world layout)
![Drone Light Show System](/static/drone-layout-angle.jpg "Drone Light Show System")

![Drone Light Show System](/static/Z-Axis-Rotate_-40.jpg "Drone Light Show System")

*  In default, the orientation of the formation is North. The GCS couldn't change the orientation of the drone formation. The drone will totally fly according to the designed path. If you want to change the orientation. It needs to be set in the designer software before you export the data.   
*  Vehicle -> Export Setting -> Z Axis Rotate(degree in clockwise).    
*  Z Axis Rotate: rotate degree in clockwise to coordinate, default is 0, if your flight field direction is different from your design, this would help.    
*  Pay attention: if you change the Z Axis Rotate, the drone' head need to change the same degree.  




**Operation Video**

* [YouTube](https://youtu.be/ZKN7bdUU3XM)
* [bilibili](https://www.bilibili.com/video/BV1uC4y1t7iV/)

<iframe width="560" height="315" src="https://www.youtube.com/embed/ZKN7bdUU3XM" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


----

## Flight Procedure
0. Connect the wifi on computer, run Vimdrones GCS  
1. When the RTK Base is enter, click **Survey In** button   
2. Waiting for Survey In ready, **Survey in(Success)**  
3. Click **Open** button, Select Design Project   
4. Power on Mazzy Star Drones, white light fast flashing -> red light flashing    
5. Mazzy Star Drone online, we can see the Drone Status on GCS  
6. Drone Status Check Pass(RTK Fix), yellow light flashing  
7. Click **Upload** button, upload trajectory Design to the drones, white light fast flashing  
8. Select Drone 1, click **Copy From Drone** button, copy drone 1 location  
9. Click **Set Home** button, set home location to all drones, green light  
10. Click **Takeoff** button, start your Drone Light Show 




**Operation Video**

* [YouTube](https://youtu.be/N5A8r9rXA68)
* [bilibili](https://www.bilibili.com/video/av79197730/)

<iframe width="560" height="315" src="https://www.youtube.com/embed/N5A8r9rXA68" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

---


## Post-Flight Setup Procedure
* Unplug the batteries of the drones to the package
* Put the drones into the packages, then stack up the packages and tie them up with a buckle
* Pack up the Drone Light Show System into the package
* Pack up the remaining equipment



## Remote Control

Remote Control(RC) is the backup control system（another two are: 915HMz/868HMZ/2.4GHz radio & 2.4G WIFI). By default, we will not use the remote control in the drone light show.    
In some emergency situations, we could use the remote control to control the drone to Land/RTL during the show. Please select the drone you want to manual control by RC controller in the GCS software, then click **Rescue** button.   
Also, remote control could test the drone after the repaired.

**Note**: Generally, we control one drone at a time by RC.

**Rescue**: Enable drone's RC control to manual control by RC controller. During the flight, the RC control channel is closed. When we click the **Rescue** button, the channel is opened.

**How to manually control a Drone**  
Please set up the drone light show equipment at first, we could check the statues on Vimdrones GCS.

**Take Off** 

1. Align the heading of the drone with your heading
2. Power the drone
3. Power the remote control and check the switch  
Flight Mode - **0: Stabilize** （we could check the MODE in GCS）  
FLAP - RTL Mode - **set down** - 2  
Disarm - **1 Keep Up**  - The throttle is locked  
RATE - Hi - Set Up before enabling the motors     
4. Wait for the drone to enter the positioning state - RTK Fix / Float
5. Push the throttle stick to the low position to the right - **2 To Bottom Right**. 
6. Arm - **3 Keep Down** 
7. The propellers start to turn
8. Slowly raise the throttle to make the drone take off - **4 Raise Throttle**
9. We could change other Flight Mode for flight

**Landing**

* RTL Mode  
Set up the RTL Mode stick.   
The drone will return home automatically. (we could check the MODE in GCS)   
Disarm - **1 Keep Up**  
* Manually control Landing  
Change Flight Mode - 1: Altitude hold    
Push the throttle stick to the low position    
Disarm - **1 Keep Up**  
Push the throttle stick to Bottom Left  

We can choose one of the ways to land, generally for RTL.

![Remote Control](/static/transmitter-controls.jpg "Remote Control") 

**More details:**

* [DXe Transmitter Manual – Multilingual](https://www.spektrumrc.com/ProdInfo/Files/SPM1000-manual-MULTI.pdf)  

**Usage Warning:**  

* Do not arm the drone near people too close   
* Do not arm the drone over people’ head  

**Operation Video**

* [YouTube](https://youtu.be/BS5PN4v3c20)
* [bilibili](https://www.bilibili.com/video/BV185411P7wj?share_source=copy_web)

<iframe width="560" height="315" src="https://www.youtube.com/embed/BS5PN4v3c20" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

</br>


## Battery

* Its capacity is 3000 mAh and the rated voltage is 8.7V. 

**Battery Charging and Discharging**

* At normal charging mode, in constant current stage, the battery is charged in 0.2C until voltage reaches 8.7V, when constant voltage stage starts. Whole charging ends after 3.5 hours or when charging current is less than 60mA(0.02C). 
* At fast charging mode, the charging current is 1C until voltage reaches at 8.7V. The whole process is up to 3 hours or ends when charging current is less than 60mA(0.02C)
	
			
**Usage Warning**

* Do not disassemble, crush and incinerate, drop or leave high pressure on the battery. 
* Do not short circuit the battery 
* Do not expose the battery to temperatures above 45 degrees or below 0 degrees

**Storage Instruction**

* Keep the environment dry and clean 
* Ensure the battery at a storage voltage (7.08-7.62V) if not in use for a long time. If voltage is above or below that level, please charge or discharge battery
* Battery must be fully charged and discharged routinely every three month. After battery is fully discharged, recharge the battery to 50% capacity 


## Battery Charger

* 2S Li-ion HV Battery Charger, 8.7V/1.5A*10Channel
* Input: AC100~240V 50/60Hz 3A(Max) 
* Output: DC8.7V/1.5A*10Channel

**Instruction**

* Connecting battery with charger, making sure the positive of battery connecting with the positive of charger, the negative of battery connecting with the negative of charger.
* Plug charger in DC power outlet, LED turns to RED, the charging is starting.
* The charging finish once LED turns to GREEN. After charging, make sure unplug charger from DC power outlet.
* Disconnecting battery with charger. 
    * Note: battery may become hot after charging.


**Usage Warning**

* Don't short circuit charger  
* Use the charger to charge correct battery  
* Don't cover charger and battery during charging  
* Don't charge battery unattended   

</br>


## Get Log 

Please download the [QGC](http://qgroundcontrol.com) software.  
Open QGC, use a micro USB cable to connect the computer to the USB port on the right side of the drone. Click **LOG DOWNLOAD**. It may need to click **Refresh** button. Select the log and click **DOWNLOAD** button. 
![Download Data Log](/static/qgc.jpg "Download Data Log")
Downloading and Analyzing Data Logs in [Mission Planner](https://ardupilot.org/copter/docs/common-downloading-and-analyzing-data-logs-in-mission-planner.html) 

</br>



## Repair

**Tool preparation** 

* A solder
* A tweezers  
* A screwdriver  
* A Micro USB cable  
* A Tin roll  
* A drone battery  
* A 3M Double Sided Foam
* A laptop/computer with [QGC](http://qgroundcontrol.com) installed  


**Repair the Body Frame**   

1. Unlock the propellers with H1.5 screwdriver  

2. Remove the propeller guard from 4 arms of the drone body

3. Move the drone outside the propeller guard

4. Remove 8 screws from 4 arms of the drone body with PH1 screwdriver.

5. Remove the top cap of the drone. Pay attention there is an cable connect with GPS and the motherboard.

6. Unsolder the motor cables connect with the ECS

7. Remove 3 screws of the battery plug 

8. Remove 2 screws of the battery case

9. Remove 4 screws of the LED cover

10. Remove 4 screws of motherboard

11. Unlock the 2 connectors of motherboard

12. Remove the motherboard, LED board, receiver

13. Remove the motors

14. Change the new frame

15. Install the motors 

16. Attach the receiver with the Foam

17. Install the LED board and motherboard, connect the LED board & receiver to the motherboard

18. Solder the motor cables connect with the ECS. Pay attention to the order od the cables.

19. Install battery case and battery plug.

20. Do the motor test

21. Install the the top cap of the drone. Pay attention there is an cable connect with GPS and the motherboard

22. Install 8 screws from 4 arms of the drone body with PH1 screwdriver

23. Install the LED cover

24. Install the propeller guard 
 
25. Install the 4 propellers. Pay attention the direction of the propellers  

26. Manually fly the drone for the test  


**How to Manually Fly a Drone?**  

* Setup the Vimdrones Drone Light Show System - [YouTube](https://youtu.be/iSv-nGm3Wn8)  
* Manually Fly the Drone - [YouTube](https://youtu.be/BS5PN4v3c20)


**Operation Video**

* [YouTube](https://youtu.be/jG-_YRAtWek)
* [bilibili](https://www.bilibili.com/video/BV18y4y117aA?share_source=copy_web)

<iframe width="560" height="315" src="https://www.youtube.com/embed/jG-_YRAtWek" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

