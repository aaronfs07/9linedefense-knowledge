# Cisco: Clearing Port Security

## DESCRIPTION: 
This SOP describes all necessary steps to clear Port Security when configured on a Cisco Switch. This guide will work for any Cisco Catalyst or small business switch configured with a CLI interface. 

## DEFINITION:  
Port security is a method most commonly utilized by IT Administrators in order to block only but the recognized MAC Addresses to connect to a Port. This can either be done through learned MACs or pre-programmed MAC Addresses. 

## RESPONSIBILTY:  
This will only be conducted by IT personnel.  

## DESCRIBED TASK:  
1. Login to Local Switch via SSH. 
2. Enter Administrative mode by typing `enable` . You may need to enter a password here. Actually, you **SHOULD** have to enter a password here. 
3. Type in `show interface status err-disabled`, it will then show the ports that are considered error disabled. If it shows psecure-violation then that port is confirmed to be down due to Port Security. 
4. In order to clear out the error you should first type in `clear port-security all interface gi0/23` ensure to replace `gi0/23` with the specified interface that you need to replace. 
5. Once that is completed enter `configure terminal interface gi0/23` this will enter the configuration terminal for that interface. 

## Notes
- This procedure should **NOT** require a reboot of the system itself. Considering that this issue is very common on Windows environments that download a profile from somewhere it is most likely NOT a machine itself issue. 

## Futher Troubleshooting
- Once the .bak file is cleared ensure that the system can reach the roaming profile/redirected desktop storage location. 
- If the environment is a remote desktop farm ensure that this procedure is run on **ALL** member servers. 