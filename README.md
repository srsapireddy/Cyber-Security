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
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/31c2600d-a2c4-4cc9-b607-ebc4f812322a)

## Burpsuite
### Proxy Module
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/6380f954-c378-44c8-9323-a2fe13791869)
HTTP History in Proxy Module
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/e146d18c-e279-4140-bd49-0e7706c694d5)
Request and Response checking that we are getting from the server in HTTP History
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/bbc44bf6-023f-42a0-a50a-4f6466fa0ab1)
### Other Modules like Interceptor
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/8451a752-9aae-4d87-b180-714d888dae76)
Repeater: To see the live request and response. Used for testing purposes only.
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/c3d5a96c-ef94-4728-a306-ce8336087fbc)

Intruder: Used to give attack to the target
Intruder is just used for dictionary attacks. Or the attacks related to permutations and combinations. 
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/8395a87b-a2d0-4c47-b811-d0005c794953)
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/18f4ccc3-3ed4-4c88-b2b0-9aa2bf31c066)
Types of Attacks:
1. Sniper attacks happen when you set the limit. For example, for four digits, it is 1000 - 9999 (Number of combinations available). Here, we can fix a target and attack in case OTP is a four-digit password.
2. Clusterbombing doesn't have anything as a range in there. Here, we can use numbers and alphabets. 

Comparer compares the difference between data information.
Decoder 
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/4cfa6386-9c4b-4759-bb6d-9b867799b3df)
Example
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/c3ab51b0-0803-4ae1-88ba-7427665a438d)















