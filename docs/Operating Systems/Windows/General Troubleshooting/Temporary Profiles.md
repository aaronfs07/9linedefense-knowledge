# Temporary Profiles

## DESCRIPTION: 
This SOP describes all necessary steps to remove a temporary profile from a PC.  
## DEFINITION:  
This error will occur when there was an error downloading the users profile from the server.  
## RESPONSIBILTY:  
This will only be conducted by IT personnel.  

## DESCRIBED TASK:  
1. Login to Local PC  
2. Login to PC with account that has Admin privileges. Click Start and in the “Search programs and files” box at the bottom type in regedit and press enter or click on the icon that appears under Programs. This will take you into the Registry Editor.  
3. From the file tree on the left navigate to the following folder: HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\ProfileList
4. Once here locate any folders with the “.bak” extension on the end of the name and delete this folder. This should clear any temporary profile error.
5. Log out of PC and have user login.

## Notes
- This procedure should **NOT** require a reboot of the system itself. Considering that this issue is very common on Windows environments that download a profile from somewhere it is most likely NOT a machine itself issue. 

## Futher Troubleshooting
- Once the .bak file is cleared ensure that the system can reach the roaming profile/redirected desktop storage location. 
- If the environment is a remote desktop farm ensure that this procedure is run on **ALL** member servers. 