# Project 1: Catch Me If You Can!

## Overview
One of the most popular scams throughout industries is the Business Email Compromise (BEC). BECs are responsible for many notable real world scams, incurring $26 billion dollars of losses from 2016 to 2019 alone.

We'll be handling our own BEC situation, where a malicious actor (played by Leonardo DiCaprio) has sent phishing emails to many of our employees, trying to trick them into sending hundreds of thousands of dollars. To stop this, we'll be looking at some potentially malicious emails and inspecting .pcap files to determine which emails are legitimate and which ones are fraudulent.

## Tools Used
- Azure Lab Services
- Ubuntu (Linux)
- Wireshark

## What I Learned
- Analyzed four packet capture files (.pcap), labeled A, B, C, and D, to identify suspicious email activity.
- Used Wireshark's packet filtering capabilities to examine network traffic and investigate potential phishing attempts.
- Identified suspicious activity in PCAP C, which contained multiple emails associated with the same user.
- Used Wireshark's Follow → TCP Stream feature to inspect email communications and identify a threatening message in which the sender claimed to possess the recipient's passcode and demanded payment.
- Extracted important email details, including timestamps, sender and recipient information, subject lines, and message contents.
- Identified email delivery information associated with the 15360.com domain and the MailEnable ESMTP service.
## Screenshots
<img width="526" height="220" alt="P1_Screenshot1" src="https://github.com/user-attachments/assets/17110266-0270-4c34-a202-9b6316aecd56" />

<img width="530" height="238" alt="P1_Screenshot2" src="https://github.com/user-attachments/assets/fe42f503-9601-4c4d-be96-d3e133ffa0fa" />

<img width="532" height="210" alt="P1_Screenshot3" src="https://github.com/user-attachments/assets/7331e504-fc5d-4f9a-bf3f-318997cc8ae1" />


