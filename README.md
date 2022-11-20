# SyncToNAs-Windows 
Install SyncToy <br/> 
Create a Folder Pair: <br/>
![image](https://user-images.githubusercontent.com/44326428/202930408-f005a2ba-0d66-4d41-a2dc-f00526eb4044.png) <br/>
Select the Source (LEFT) and Destination (RIGHT) <br/>
if a Samba share, then \\share\foldername <br/>
![image](https://user-images.githubusercontent.com/44326428/202930550-922121ad-875e-4fb5-b7c0-2057a55bec4e.png) <br/>
Choose the option for "What to do Accordingly", for my case, I'm repliacating my source to the right, therefore I choose: Echo <br/>
![image](https://user-images.githubusercontent.com/44326428/202930751-e5cd2976-fde8-4246-8d3f-8ac0d21ba4e1.png)<br/>
Give it a name, this will be needed for the automation process<br/><br/>

Once All the Tasks ("Pairing") has been finished<br/>
  * Sync Up to make sure everything works <br/>
  * Create a Batch script with this content:
  ```
  @echo off
  "C:\Program Files\SyncToy 2.1\SyncToyCmd.exe" -r FolderPairName
  exit
  ```
  * Test the script by itself
  * Create a Task Scchedule pointing at the Bat script, to run as often as your want!
  
  Voila!

# SyncToNAs-OneDrive
WIP
