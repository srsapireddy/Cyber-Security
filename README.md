# Cyber-Security
## Installing Kali-Linux
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/4810e4b6-a12a-41d3-8212-268f5504bdc5)

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

Command: ``` chmod 637 filename ```

To know the existing permission: ``` ls -l filename ```

### To create a new file:
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/12da759b-02d1-4185-bdab-c4a0005f04d5)

By default, the permission is 644.
Where a nono command is a text editor

## Burpsuite: To capture a request 
### Burpsuite proxy configuration
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/b305b725-69bf-46d7-9948-ce711c2a2bce)

### Start
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/d9972243-2a50-4f17-8c08-1315f435b68b)

All the requests will be intercepted in the burp suite tool.

![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/2b91c003-1049-4852-beeb-f2af41a06c26)

Intercepted request
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/c820e253-4010-49a1-92e4-2c2d2994bd8a)

### You can also install Proxy Switcher for Burpsuite
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/1185714f-8c93-488f-9ae5-859c86ef73a3)

### Difference between Burpsuite and Wireshark
The wireshark sends packets from one place to another, where we study packets. Using burpsuite, we analyze the requests made by your browser and the server. We don't see requests in the server.

### Linux Commands Cheetsheet
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/c22500a1-dcaa-483a-acc1-09ccb7f69479)







