**Create or Modify System Process. ID: T1543
Sub-techniques: ID: T1543.001**


This method concentrates on two distinct persistence mechanisms. 
Creating a.plist file and running it from the LaunchAgent directory constitutes the first method. 
LaunchAgent executes user-related processes and applications. The second persistence method makes use of LaunchDaemon, a system-level process.
Now that SIP has been disabled, both launch agent and launch daemon can be executed from the /System/ directory,
but doing so requires restarting the device and running a.Plist file from the /Sysyetm/ directory first. 

        
| Commands  | 
| ------------- | 
| /Library/LaunchAgents .<.Plist Name>  | 
| /Library/launchdaemon. <.Plist Name> | 
| /System/LaunchAgents. <.Plist Name> ---- requires the threat actor to disbale SIP  |
| /System/launchdaemon. <.Plist Name>| 


