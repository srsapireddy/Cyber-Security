# Cyber-Security
## Installing Kali-Linux
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/124008b5-3c62-4033-81b2-7361dd12db75)

### Updating Kali Linux
```
apt-get update && apt-get upgrade -y
```
### To know the username of the Kali Linux
```
uname -a
```
## File Architecture of Linux
### Root of Kali Linux
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/f35580b8-5751-483a-abb0-ba7558cb0e94)

### Login as a root user
```
sudo -i
```

### File Permissions
Groups in Linux
1. Admin/ Owner Group
2. User Group
3. Public Group

Modes:
R : Read    : 4
W : Write   : 2  
X : Execute : 1

Example: 6 - To give read and write permission to the admin
Example: 3 - To give write and execute permission to the user
Example: 7 - To give all the permission to the public

Command: chmod 637 filename 

To know the existing permission: ls -l filename

### To create a new file:
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/12da759b-02d1-4185-bdab-c4a0005f04d5)

By default, the permission is 644.
Where a nono command is a text editor

## Burpsuite




