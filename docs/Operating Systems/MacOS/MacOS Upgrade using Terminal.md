# MacOS Upgrades

## DESCRIPTION:
This SOP describes all necessary steps to **upgrade** a MacOS Operating system to another version using a full installer download. This process will be completed via Terminal.
## DEFINITION:  
Mac users can download full complete MacOS installers directly from the command line. This is an incredibly useful feature particularly if you want to use it within scripts, you manage multiple Macs, or you simply want to have full access to a complete installer application of MacOS for any other purpose.

With this particular trick, you can download complete “Install MacOS” application packages directly from the Terminal application, and it works to get full installers of macOS Monterey, macOS Big Sur, Catalina, Mojave, and High Sierra too.

## RESPONSIBILTY:  
This will only be conducted by IT Members.

## DESCRIBED TASK:  
1. Login to the terminal of the MacOS Machine through any means avaliable to you.
3. Inside the terminal type ```softwareupdate --fetch-full-installer --full-installer-version 12.2.1```
5. It will then go through the process of downloading and installing this version of MacOS.
6. Once the process exits successfully (no errors) you have successfully upgraded MacOS.

## Notes
- This procedure should **NOT** require a reboot of the system itself.
- Please note the version in step #2. This will allow you to install a specific version of MacOS. Please contact your lead technician to discuss which version of MacOS you all are currently supporting.

## Futher Troubleshooting
None Avaliable for this process. 
