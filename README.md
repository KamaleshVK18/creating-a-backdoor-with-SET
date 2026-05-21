# creating-a-backdoor-with-SET
creating a backdoor with SET - Ethical Hacking Techniques course

# AIM:
To Create a backdoor with Social Engineering Toolkit (SET)

## DESIGN STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode


### Step 2:

Investigate on the various categories of tools as follows:

### Step 3:

Open terminal and try execute some kali linux commands

### Architecture Diagram

```
+----------------+        +------------------------+        +----------------------+
| Attacker's PC  | -----> | SET (Credential        | -----> | Fake Login Page      |
| (Kali Linux)   |        | Harvester via Apache)  |        | (Hosted by SET)      |
+----------------+        +------------------------+        +----------------------+
       |                                                             |
       |                                                             v
       |   1. Configure SET with phishing site (e.g., Gmail clone)   |
       |                                                             |
       |                                                             v
       |                                                 +----------------------+
       |                                                 | Victim's Browser     |
       | <------------------------------------------------| Clicks Phishing Link|
       |                                                 +----------------------+
       |                                                             |
       |                                                             v
       |     2. Victim Enters Credentials → Sent to SET/Attacker    |
       |                                                             |
       |                                                             v
       |                                                 +----------------------+
       |                                                 | Credentials Captured |
       |                                                 | in Apache log/SET DB |
       |                                                 +----------------------+

```

## EXECUTION STEPS AND ITS OUTPUT:
Social Engineering attacks are the various cons used by the hackers to trick people into providing sensitive data to the attackers.

**Steps to Use SET for Phishing (Credential Harvester Attack Method)**

**1. Open terminal:**
```bash
sudo setoolkit
```
**2. Navigate:**
```bash
1) Social-Engineering Attacks  
2) Website Attack Vectors  
3) Credential Harvester Attack Method  
```
**3. Enter your IP address as the attacker server.**
**4. Choose:**
```bash
2) Site Cloner
```
**5. Enter the URL of the legitimate site ```(e.g., https://accounts.google.com)```**

**6. Send the generated link to the victim.**

**7. Once the victim logs in → their credentials are stored in:**
```bash
/var/www/html/
```

## OUTPUT:

<img width="1918" height="663" alt="Screenshot 2026-05-21 083839" src="https://github.com/user-attachments/assets/b3173cbc-6877-4dd1-924d-f41597dc1822" />

<img width="1436" height="651" alt="Screenshot 2026-05-21 083849" src="https://github.com/user-attachments/assets/de49f3de-2a73-40ab-8b99-2917ba948fa4" />

<img width="1453" height="673" alt="Screenshot 2026-05-21 083903" src="https://github.com/user-attachments/assets/37d72a30-6a12-4e1f-b38a-85aec5c8bb00" />

<img width="1460" height="741" alt="image" src="https://github.com/user-attachments/assets/7079820a-444f-4b13-9580-a9b3ae561c39" />

<img width="1284" height="734" alt="image" src="https://github.com/user-attachments/assets/27431ddd-670f-439d-a484-bd825d8bb165" />




## RESULT:
The Social Engineering Toolkit (SET) is used to create backdoor is  examined successfully
