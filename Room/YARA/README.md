# <img src="https://user-images.githubusercontent.com/51442719/174496736-c14a8624-fedd-4e8d-887f-4dad42bb6a40.png" width="100"> [YARA](https://tryhackme.com/room/yara)
  > ![image](https://user-images.githubusercontent.com/51442719/174496659-3b7fe02a-6ed9-430e-b601-7f46edeaf1f2.png)
  > ####  Learn the applications and language that is Yara for everything threat intelligence, forensics, and threat hunting!
  > - [x] Task 1  [Introduction]()
  > - [x] Task 2  [What is Yara?]()
  > - [ ] Task 3  [Installing Yara (Ubuntu/Debian & Windows)]()
  > - [ ] Task 4  [Deploy]()
  > - [ ] Task 5  [Introduction to Yara Rules]()
  > - [ ] Task 6  [Expanding on Yara Rules]()
  > - [ ] Task 7  [Yara Modules]()
  > - [ ] Task 8  [Other tools and Yara]()
  > - [ ] Task 9  [Using LOKI and its Yara rule set]()
  > - [ ] Task 10  [Creating Yara rules with yarGen]()
  > - [ ] Task 11  [Valhalla]()
  > - [ ] Task 12  [Conclusion]()

---

## Task 1  [Introduction]()
  > ### This room will expect you to understand basic Linux familiarity, such as installing software and commands for general navigation of the system. Moreso, this room isn't designed to test your knowledge or for point-scoring. It is here to encourage you to follow along and to experiment with what you have learned here. <br>
  > ### Feel free to use the VM attached to this room in Task 4: Deploy, or alternatively, install Yara on your system using the steps provided in this room. <br>
  > ### As always, I hope you take a few things away from this room, namely, the wonder that Yara (Yet Another Ridiculous Acronym) is and it's importance in infosec today. Yara was developed by Victor M. Alvarez (@plusvic) and @VirusTotal. Check the GitHub repo [here](https://github.com/virustotal/yara).

---

## Task 2  [What is Yara?]()
- 2.1. [All about Yara](#21-all-about-yara)
- 2.2. [Why does Malware use Strings?](#22-why-does-malware-use-strings)
- 2.3. [Caveat: Malware Analysis](#23-caveat-malware-analysis)
  > ## 2.1. All about Yara 
  > ### "The pattern matching swiss knife for malware researchers (and everyone else)" ([Virustotal., 2020](https://virustotal.github.io/yara/))
  > ### With such a fitting quote, Yara can identify information based on both binary and textual patterns, such as hexadecimal and strings contained within a file.
  > ### Rules are used to label these patterns. For example, Yara rules are frequently written to determine if a file is malicious or not, based upon the features - or patterns - it presents.
  > ### Strings are a fundamental component of programming languages. Applications use strings to store data such as text.
  > ### For example, the code snippet below prints "Hello World" in Python. The text "Hello World" would be stored as a string.
  > ![image](https://user-images.githubusercontent.com/51442719/174509253-00758cab-42f7-4133-b28c-3e201713c212.png)
  > #### We could write a Yara rule to search for "hello world" in every program on our operating system if we would like. 
  > ## 2.2. Why does Malware use Strings?
  > ### Malware, just like our "Hello World" application, uses strings to store textual data. Here are a few examples of the data that various malware types store within strings:
  > | Type       	| Data                               	| Description                                            	|
  > |------------	|------------------------------------	|--------------------------------------------------------	|
  > | Ransomware 	| 12t9YDPgwueZ9NyMgw519p7AA8isjr6SMw 	| 	Bitcoin Wallet for ransom payments                     	|
  > | Botnet     	| 	12.34.56.7                         	| 	The IP address of the Command and Control (C&C) server 	|
  > ## 2.3. Caveat: Malware Analysis
  > Explaining the functionality of malware is vastly out of scope for this room due to the sheer size of the topic. I have covered strings in much more detail in "Task 12 - Strings" of my [MAL: Introductory room](https://tryhackme.com/room/malmalintroductory). In fact, I am creating a whole Learning Path for it. If you'd like to get a taster whilst learning the fundamentals, I'd recommend my room.
  > 







