---
layout: post
title:  "Blog"
date:   2020-06-9 21:03:36 +0530
categories: HTB OSCP CySEC Blog
---
6/16/2020 - Worked on a Windows hackthebox machine today. A pretty informative box, involved the same c# decompilation in order to extract the method to decrypt an encrypted password. In this case the user password was inside of a sqlite db file, and the method that encrypted it used two static keys along with aes after taking the cleartext to Base64. This would have been secure had the encryption be dynamic rather than being able to find both static keys within the decompiled program. After using that given password I was able to get a shell with winrm. After some enumeration I was able to query AD to get information on a deleted admin account mentioned, after decoding that I was able to get root. Pretty interesting machine, learned a good amount about navigating and extracting nuggets of information from an anonymous RPC session. 

6/9/2020 - Hopefully I will keep this updated to the best of my abilities. This will be my first entry, I plan on going into my findings online and what I am currently interested in and where I am spending my time.

Over the past month I have had a lot of time to study due to COVID-19. I have been focusing almost all of my efforts on solving HackTheBox challenges. The amount of information and different technologies I get to play with and mess with to figure stuff out is crazy. The other day one of the boxes required me to decompile a .NET application and read its source code in order to extract the encryption and decryption process used for the hashes I had found on the machine. After rewriting and tweaking the .NET code I was able to decrypt it. Took me some time and definitely was my first time decompiling an application I had used ILSpy to accomplish this. It was super fun and informative. That is why I am spending so much time on these HTB challenges to prepare myself for the coursework once I start the OSCP course. My current plans are to obtain at least 50% ownership of active machines on HackTheBox and then proceed with the OSCP course in preparation for the test. I am currently at 20% ownership on hackthebox.
