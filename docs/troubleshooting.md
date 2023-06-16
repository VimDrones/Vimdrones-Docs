

## GCS not connect to RTK base
 
When GCS could not connect to the RTK base. It shows “Waiting for server connection…”    

* Please check connection between RTK base and router.  
* Please check if the computer is connected to the WiFi of Vimdrones.  
* If you use Windows, please allow Vimdrones GCS through firewall when installing Vimdrones GCS for the first time. If you choose not allowed, GCS cannot properly connect to the server.   
Please follow these steps: 
 
**METHOD I**

1. Open Windows Security.  
2. Click on Firewall & network protection.  
3. Click the Allow an app through firewall option.  
   ![GCS Firewall](/static/gcs-firewall-1.png "GCS Firewall")
4. Click the Change settings button.  
5. Check vimdrones gcs.exe to allow through the firewall.  
6. Check on Private and Public access the network. 
   ![GCS Firewall](/static/gcs-firewall-2.png "GCS Firewall")
7. Click the OK button.  
8. Reopen Vimdrones GCS.    
   If you open and close GCS for multiple times, please open the Task Manager(Control + Shift + ESC) and close all GCS in the Task Manager. 


**Quick tip:** If Vimdrones GCS isn’t on the list, click the Allow another app button to locate the Vimdrones GCS.   
![GCS Firewall](/static/gcs-firewall-3.png "GCS Firewall") 

**METHOD II**

Turn off the Private network and Public network.

We suggest you using use the Method I.

------

## Drone not online

When power on the drone, we could hear a beep (normal) sound but no light. The drone is not online in the GCS.


- Please pull out the battery and replug the SD card. SD card might be loose when in the transport.  
- If it is still not working. Please change an SD card that works well in another drone. If the drone is online,  the SD card might be broken. Please make a new SD card and plug it into this drone.
- Please check if the WIFI SSID and Password of the SD card match the router. 
- Please check if the number of devices that can be connected to the router is exceeded. 


-----
## Project upload fail

Some drones upload the design project fail and keep white flashing.

- Please click Upload(Skip success) to upload the project again.
![Ground Station Interface](/static/gcs-project-update.jpeg "Ground Station Interface")
- Or please select the drone that upload fails and click the upload button in the Drone Dashboard. When upload success, the color of token number will become green. 
- Please check the Wifi Rssi of the drone that upload fail.  If the Received Signal is week,  please jump to the troubleshooting of [Wifi Signal](https://docs.vimdrones.com/troubleshooting/#wifi-signal-is-weak-wifi-channel-sometimes-turns-off).  
- Please check if the drone has the IP address. If no IP address, please contact us for technical support.  


**Note:** We could check the upload state in the OverView Panel.   
Token Fail means the drone'project upload fail or Empty.  
![Ground Station Interface](/static/gcs-overviewer-token.jpeg "Ground Station Interface")


------
## Drone not takeoff

Some drones didn’t takeoff in the drone light show. 

- The battery is low. If the battery voltage is lower than 7.2V, the drone won’t takeoff. 
  Please change a battery with full charge.
- The token of drone is not match or empty. 
  Please upload the the design project to the drone. 
- It appears **PreArm: Check mag field** in the Log System. 
  Please move the drone to another place to check if still have the same message. If not, there may be magnetic interference under the ground of that drone. Please try to place it on our foam box to keep the drone off the ground.
- It appears **GPS glitch** of the drone when we takeoff the drones.   
  Reboot the drones after RTK base survey in success to avoid GPS position offset, to totally avoid GPS glitch reject takeoff can remove GPS item in ArmCheck.  
- It appears **PreArm: Logging failed** in the Log System.   
  Change the internal SD card, or uncheck Logging Available in ArmCheck to avoid this.  
- It appears **PreArm: Internal error(0x800)** in the Log System.
  Please contact us for technical support.   

**How to change ArmCheck?**

Please connect the right port of the drone to the PC with a micro USB cable. Open QGC, Safety -> uncheck the items   

![QGround Station Interface](/static/qgc-armcheck.jpeg "QGround Station Interface")


-----
## Wifi Signal is weak/ Wifi channel sometimes turns OFF

When the drone’s Received Signal is weak or Wifi channel sometimes turns OFF, you can refer to the following steps.   

* Adjust the distance of the router to the dronesIt is recommended that adjust the placement of the router is close to the drones. Shorten the distance between the router and drones, to avoid the distance of the signal transmission affecting the strength of the signal.  

* Adjust the direction of the router's antennasPlease try adjusting the angle of the external antenna (e.g. 45 degrees, 90 degrees, etc.) to the optimal signal distance.   
For example, as RT-AC86U, please refer to the user manual for other models. To ensure the best Wifi signal, set the antennas as below suggested image  
![Router](/static/router-antenna.jpeg "Router") 

* Avoid interference or barriers affecting the wifi signal around the routerAvoid putting the router next to the power bank.It is recommended to place the router in the center of the drones where possible in an open area, not on the ground.  

* Check and update the Firmware Version of the router.  



----

## Drone circling after taking off

If the drone flies in circles, please perform Magnetic calibration after landed. 

**Why do we need to do Magnetic calibration?**

When drones are affected by environmental magnetic fields, drones will fly a horizontal circular path in the air, which is not good for the drone show and may cause collision. An electric cable underneath the ground may affect the takeoff of drones. You can place a package box as a platform to raise the drone’s height. If the problem is solved, you don't need to proceed with magnetic calibration of the drone.

Another situation is before we shipped your drones, we already did the magnetic calibration. But after drones have been shipped far away from our location, you may better proceed with magnetic calibration before your test flight.


**How to do Magnetic calibration?**

**METHOD I**

After the drone light show devices are set up. Open the Vimdrones GCS. Select the drone you need to do the magnetic calibration.   
In the Dashboard of the drone, click the **Mal Cal** button. The drone will change red light. Now you need to rotate the drone along 3 axes.  

1. Rotate the drone horizontally on the ground   
2. Flip left and right to rotate the drone  
3. Flip up and down to rotate the drone   
4. When the drone start flashing, randomly rotate the drone  

**Result**  

* If the drone shows **green** light, it means the result is **good**.   
  The drone will reboot itself and red flashing. Then finish the magnetic calibration.  
* If the drone shows **yellow** light, it means the result is **normal**.   
  Please do the magnetic calibration again.  
* If the drone shows **red** light, it means the result is **bad**.   
  Please do the magnetic calibration again.  

**Pay attention**: Away from the electricity environment while doing the magnetic calibration

**Operation Video**

* [YouTube](https://youtu.be/ZlQ8sfpCqeQ)
* [bilibili](https://www.bilibili.com/video/BV1TL4y1a7N3/?share_source=copy_web&vd_source=943fe440f06e9a2914e98a6a98356954)

<iframe width="560" height="315" src="https://www.youtube.com/embed/ZlQ8sfpCqeQ" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

---

**METHOD II**   

Compass calibration through QGroundControl software   

1. Plug in with right USB port.  
2. Go to Sensors page for Compass calibration process. 
![QGroundControl](/static/qgc-mag-1.jpeg "QGroundControl")
3. Rotate the drone along 3 axes, and finish random rotating at last till progress bar finished. Calibration result should be green, which means a GOOD result. Reboot the drone to finish calibration.  
![QGroundControl](/static/qgc-mag-2.jpeg "QGroundControl")


## Others
If there are any other questions, please contact us for technical support.   
[Get in Touch](https://vimdrones.com/en/contact)