# Group Policy Client Service Failed the Logon

Actual Error: Group Policy Client service failed the logon access is denied.

## Troubleshooting Steps

1. Ping the Domain Controller
2. Reboot the Server the issue is occuring on (if possible) 
3. Open Powershell and run ```test-computersecurechannel``` if it comes back as true than move on. 
4. Try logging on with another user
5. If the logon with another user works investigate if they are using Redirected Folders or roaming profiles. These can cause this issue. 


## General Meaning

This error typically pops up when a machine is unable to run a group policy object that is being applied. I have typically seen this error when you have long running scripts, roaming profiles, or redirected folders. 

## Typical Solution

Login with another user and if the troubleshooting steps above fail rename the users profile folder (typically located in C:\Users) to %username%.bak and allow the user to establish another profile. 