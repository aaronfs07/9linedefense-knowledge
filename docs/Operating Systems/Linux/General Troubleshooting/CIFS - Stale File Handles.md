## Stale File Handle Error on CIFS

## Presentation of the Issue

No matter how I try to interact with the files inside that share, nothing works, I always get the "Stale file handle" error. The only thing I can do is list the directories (ls). The other CIFS shares do not have that issue, and I'm able to copy files from them to my Ubuntu box without any issue. Also, I'm able to interact (copy, move, etc.) these files from that share if I'm under a Windows system.

Things I tried (to no avail) to solve the issue:

-   Unmount/mount the share
-   Reboot the system
-   Change the vers option in the mount command to 2.1 and 3.0
-   Change the cache option in the mount command to none
-   apt-update && apt-upgrade

## Solution

```
//192.168.1.2/Media/Completed_Downloads  /completed_downloads cifs rw,_netdev,noserverino,uid=debian-transmission,user=plex,pass=Psf$dFMA7DPJ?BH6 0 0

```
Use this in your /etc/fstab to mount the file instead of the other ways. From my understanding this error occurs because it is using Server generated inodes and you need to allow your client to map it's own inodes. 
