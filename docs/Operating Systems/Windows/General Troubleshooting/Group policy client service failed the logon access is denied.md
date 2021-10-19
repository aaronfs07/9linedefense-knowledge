Normally a reboot of the RDS farm. If that is not working then I would run the following in powershell 
test-computersecurechannel
If it comes back true it is good to go. Move on to the below 
See if you can ping 10.10.10.95
If you can move on
See if you You login and get a temporary profile. Same way he is logging in. 
The group policy failure means there is some network disconnect between Danny's profile the rds


Reboot MMPV-RD*, MMPV-RG*, and MMPV-RA*,
The star being a wildcard. For example MMPV-RD01-OPPV
Make sure users aren't logged in before rebooting 
Another test troubleshooting item is to login and go to C:\Users and find Danny's username and right-click and rename it to username.old
Username being Danny's username. Just add .old. And then have him log back in