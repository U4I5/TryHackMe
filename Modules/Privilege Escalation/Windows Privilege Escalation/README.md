![image](https://user-images.githubusercontent.com/51442719/181646417-4f424c63-70c3-4715-9de6-c9021bae34dd.png)
## `VIP` - [Windows Privilege Escalation](https://tryhackme.com/jr/windowsprivesc20)
#### Learn the fundamentals of Windows privilege escalation techniques.

- [x] [Task 1  Introduction](#task-1--introduction)
- [x] [Task 2  Windows Privilege Escalation](#task-2--windows-privilege-escalation)
- [ ] [Task 3  Harvesting Passwords from Usual Spots](#task-3--harvesting-passwords-from-usual-spots)
- [ ] [Task 4  Other Quick Wins](#task-4--other-quick-wins)
- [ ] [Task 5  Abusing Service Misconfigurations](#task-5--abusing-service-misconfigurations)
- [ ] [Task 6  Abusing dangerous privileges](#task-6--abusing-dangerous-privileges)
- [ ] [Task 7  Abusing vulnerable software](#task-7--abusing-vulnerable-software)
- [ ] [Task 8  Tools of the Trade](#task-8--tools-of-the-trade)
- [ ] [Task 9  Conclusion](#task-9--conclusion)


---


---

## [Task 1  Introduction]()
#### During a penetration test, you will often have access to some Windows hosts with an unprivileged user. 
- Unprivileged users will hold limited access, including their files and folders only, and have no means to perform administrative tasks on the host, preventing you from having complete control over your target.
- This room covers fundamental techniques that attackers can use to elevate privileges in a Windows environment, allowing you to use any initial unprivileged foothold on a host to escalate to an administrator account, where possible.
- If you want to brush up on your skills first, you can have a look through the [`Windows Fundamentals Module`](https://tryhackme.com/module/windows-fundamentals) or the [`Hacking Windows Module`](https://tryhackme.com/module/hacking-windows-1).
 
 
---

## [Task 2  Windows Privilege Escalation]()
#### Simply put, privilege escalation consists of using given access to a host with "user A" and leveraging it to gain access to "user B" by abusing a weakness in the target system. 
- While we will usually want "user B" to have administrative rights, there might be situations where we'll need to escalate into other unprivileged accounts before actually getting administrative privileges.
- Gaining access to different accounts can be as simple as finding credentials in text files or spreadsheets left unsecured by some careless user, but that won't always be the case. 

#### Depending on the situation, we might need to abuse some of the following weaknesses:
- Misconfigurations on Windows services or scheduled tasks
- Excessive privileges assigned to our account
- Vulnerable software
- Missing Windows security patches

#### Before jumping into the actual techniques, let's look at the different account types on a Windows system.

### Windows Users
#### Windows systems mainly have two kinds of users. 
- Depending on their access levels, we can categorise a user in one of the following groups:

| Administrators | These users have the most privileges. They can change any system configuration parameter and access any file in the system. |
|:---:|:---:|
| **Standard Users** | These users can access the computer but only perform limited tasks. Typically these users can not make permanent or essential changes to the system and are limited to their files. |

- Any user with administrative privileges will be part of the Administrators group. 
- On the other hand, standard users are part of the Users group.

- In addition to that, you will usually hear about some special built-in accounts used by the operating system in the context of privilege escalation:

| **SYSTEM / LocalSystem** | An account used by the operating system to perform internal tasks. It has full access to all files and resources available on the host with even higher privileges than administrators. |
|:---:|:---:|
| **Local Service** | Default account used to run Windows services with "minimum" privileges. It will use anonymous connections over the network. |
| **Network Service** | Default account used to run Windows services with "minimum" privileges. It will use the computer credentials to authenticate through the network. |

- These accounts are created and managed by Windows, and you won't be able to use them as other regular accounts. 
- Still, in some situations, you may gain their privileges due to exploiting specific services.

---

## [Task 3  Harvesting Passwords from Usual Spots]()

---

## [Task 4  Other Quick Wins]()

---

## [Task 5  Abusing Service Misconfigurations]()

---

## [Task 6  Abusing dangerous privileges]()

---

## [Task 7  Abusing vulnerable software]()

---

## [Task 8  Tools of the Trade]()

---

## [Task 9  Conclusion]()