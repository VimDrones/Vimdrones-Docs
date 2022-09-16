## GCS not connect to RTK base
When GCS could not connect to the RTK base. It shows “Waiting for server connection…”    

* Please check connection between RTK base and router.  
* Please check if the computer is connected to the Wi-Fi of Vimdrones.  
* If you use Windows, please allow Vimdrones GCS through firewall when installing Vimdrones GCS for the first time. If you choose not allowed, GCS cannot properly connect to the server.    

Please follow these steps: 
 
**METHOD I:**

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

**Quick tip:**   
If Vimdrones GCS isn’t on the list, click the Allow another app button to locate the Vimdrones GCS.   
![GCS Firewall](/static/gcs-firewall-3.png "GCS Firewall") 

**METHOD II:**

Turn off the Private network and Public network.

We suggest you using use the Method I.

