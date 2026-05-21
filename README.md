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

<img width="1600" height="927" alt="image" src="https://github.com/user-attachments/assets/a4aaa93d-bc52-433c-a78b-0b80c194c3dd" />

<img width="1600" height="932" alt="image" src="https://github.com/user-attachments/assets/7519be37-f233-4bb4-ab75-8308209838ea" />

<img width="1600" height="946" alt="image" src="https://github.com/user-attachments/assets/c7915351-8d25-4022-8d60-cdabb7149521" />

<img width="1600" height="905" alt="image" src="https://github.com/user-attachments/assets/732babca-9e94-4ed6-a1a7-cc1510243631" />

<img width="1844" height="1086" alt="image" src="https://github.com/user-attachments/assets/52145558-4a8c-43a8-ae49-677ff90c74b9" />


<img width="1222" height="422" alt="image" src="https://github.com/user-attachments/assets/c7891861-96c3-4e11-a476-1988ff53717b" />



## RESULT:
The Social Engineering Toolkit (SET) is used to create backdoor is  examined successfully
