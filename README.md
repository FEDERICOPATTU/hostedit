# hostedit
A powershell script to update Windows hosts file with current WSL ip address(es)

this Windows powershell file is designed to update Windows hosts file with current wsl ip address allowing integration with wsl provided services. It can also launch specific commands to be run on the wsl host. 

Marco Guardigli
mgua@tomware.it
mar 20, 2022

## Installation
 - Place this hostedit.ps1 file in 
   c:\windows\system32\drivers\etc

 - configure it accordingly to your names 
   editing $wsl_name and $names variables
   
 - add command chaining features, placing commands to be 
   launched on wsl host in 
   c:\windows\system32\drivers\etc\cmdchain.txt  

 - execute it when needed from a powershell admin prompt (it will not work if not admin)

 ------------
 
 ## Creating a easy to use desktop shortcut:
 
 - Create a desktop shortcut for powershell.exe and name it "hostedit"
 - Edit its properties and add c:\windows\system32\drivers\etc\hostedit.ps1 
   at the end of the target line leaving a space after "powershell.exe"
 - When needed, right click on the shortcut and run as administrator
 
