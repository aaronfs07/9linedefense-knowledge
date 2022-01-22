# Linux Unifi Server Troubleshooting Guide

## Ubuntu/Debian Troubleshooting

- On Ubuntu Unifi Controllers you may encounter the APT error `Repository 'https://dl.ubnt.com/unifi/debian stable InRelease' changed its 'Codename' value from 'unifi-6.1' to 'unifi-6.2'` If you do you simply need to run the following command to acknowledge the changes in APT Release Information
	- `sudo apt-get update --allow-releaseinfo-change`
	- This issue will pop up from time to time as the release info changes. This can cause automated scripts to sometimes fail on the controller devices.