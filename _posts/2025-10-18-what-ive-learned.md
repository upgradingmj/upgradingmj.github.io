---
title: What is Git?
date: 2025-10-18
categories: [career, education]
tags: [learningwithmj]

---

# Understanding the Git Protocol


One of the most biggest challenges in my career was my lack of understanding of the Git protocol. People say the best way to learn is by doing, and I placed that into practice by staging this website, yes I didn't get it right the first.. or second time but I eventually got it! I understand why developers have so much flexibility and control in terms of their workflow. 

One of the most common misconceptions for folks is conflating between Git and Github by believing they're one and the same. While most people who use Git do also famously use Github these services are different as Git is able to work with version control software vensors such as Github, Gitlab, Gitea, etc. I was also guilty of this as well since I had no idea how the underground protocol worked.

In order to understand how Git works more we need to have a brief chat about VCS systems also known as "Version Control Systems."

Version Control systems are tools used by software developers when working on projects to track and manage changes to code. The perks of this is that if something breaks or doesn't work properly, the team has a single source of truth and can isolate the issue and restore stable blocks of code without needing the throw the whole project out. 

There are 3 different VCS types I'll briefly discuss today.

- Local 
- CVCS = Centralized Version Control System
- DVCS = Distributed Version Control Systems (like Git!)

Local VCS Systems:
 
 - Is pretty simple and is just someone working and maintaining projects locally on their computer at home. 
 - The pro's of this of course is that it's easily doable by anyone (since this is what we all do on a daily basis) but there are no backups, ways to properly track changes for a team to be able to reference and manage, and is meant for people riding solo. 

Centralized Version Control Systems (CVCS):
- This is essentially a centralized server that an entire team can work on. 
- Allows for centralized administration for RBAC controls and provides great benefits for IT Administrators. 
- Biggest draw back being a single point of failure if server goes down or data is lost. Which means that I'm likely getting a phone call at that point. 

Distributed Version Control Systems (DVCS):

- Rather than just relying on snapshots of latest files
- Repositories are fully mirrored (including full history)
- If any server dies, any of the client repositories can be copied back up to the server to be restored.
- Each clone is a fully backup of all the data allowing for complete redundancy

What makes Git Different than other Version Control Systems?

- Git handles data differently.
- Other VCS stores info as a list of file based changes.
- Other VCS think of the info they store as a set of files and the changes made to each file over time (known as delta-based version control).
- Git thinks of data more like a series of snapshots of a mini filesystem. Each Git commit or save state, Git essentially takes a photo of all your files look like at that moment and time and refers to that as a snapshot.
- If no files haven't been changed, Git doesn't store the file again (Similar to how TimeMachine Backups work on MacOS where it doesn't duplicate backups of unchanged files) Git instead just links the previous identical file it already has stored.
- This creates a "data stream" of snapshots.
- Allows git to act like a mini file system.
- Most operations in git is local and doesn't require info from another computer on the  network.
- This reduces the burden of network latency overhead.
- No server call outs since everything it reads is local on your disk.
- This allows for great autonomy since if an endpoint can't get network access (either to a reliable connection or a VPN) such as if someone hopes on an airplane. They can do everything by committing all things to a local disk.
- Very little reliance is needed on an internet connection.

One of the coolest things when learning about Git was due to the protocols nature of not relying much on a network connection. The lack of needing to be connected to a server 24/7 (unless you need to commit changes to a service like Github through a final upload) allows developers do what they do best.

As someone who's worked in IT for the past half decade and would get calls as soon as a network connection drops (even for a second) when accessing critical line of business applications. It's always made me wonder why I barely got any calls from developers regarding IT issues. In fact I remember one guy I worked with who was always traveling and as someone who loved technology due to the flexibility it offered in our modern society, I oftened wondered how it was possible. 

Anyways, that was my rant on what I've been learning the past few weeks. Thank you for taking the time to read this article, I plan to keep posting and improve my writing skills, if you have any feedback please feel free to let me know! 

Give me a follow on Linkedln! 