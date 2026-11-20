# Project 5: SIEMsational CTF

## Overview
In the Unit 5 project, you will participate in a Capture-the-Flag (CTF) style Splunk activity! You'll be tested on your ability to search, analyze, and visualize data using Splunk. Unlike a guided lab where the next step is given to you, a CTF asks you to form a hypothesis and use the tools to prove it — which is exactly how SOC analysts work during a real investigation. If you want, you can also compete with your classmates to see who can get the highest score! Take the opportunity to challenge yourself, learn from your peers, and solidify your understanding of Splunk.

## Tools Used
- Splunk Enterprise
- Splunk Search Processing Language (SPL)
- Docker

## What I learned
- Learned how to use Splunk to search and analyze logs.
- Used SPL queries to filter data and find specific information.
- Investigated suspicious login attempts and malware uploads.
- Learned how SIEM tools help detect and investigate cybersecurity threats.

## Screenshots
How many TV shows on Netflix are in the Docuseries genre?:
<img width="1170" height="282" alt="image" src="https://github.com/user-attachments/assets/4757823e-8eca-4438-8718-1daab4020385" />

What two TV-Y7 rated shows were released in 2019 and were added to Netflix on November 22, 2019?:
[ index=main host=Netflix type="TV Show" rating="TV-Y7" release_year=2019 | search date_added="November 22, 2019" | table title release_year rating date_added ]
<img width="1172" height="197" alt="image" src="https://github.com/user-attachments/assets/35db6fc7-a65a-4606-b868-1c0a44eda9ce" />


What was the IP address that uploaded the malware (MD5 hash: 3AADBF7E527FC1A050E1C97FEA1CBA4D):
[ 192.168.1.10 ]
<img width="1170" height="278" alt="image" src="https://github.com/user-attachments/assets/3441dd3d-3fe7-461b-aeea-5caa7c6064ee" />

What usernames did that IP address try to login to the system as? Which one did they upload a file as?:
[ Opera/75.0.3969.218 ]
<img width="1170" height="383" alt="image" src="https://github.com/user-attachments/assets/a8fc361d-46bf-4eec-9410-af4bc32eea58" />
