# Project 3: Off Limits

## Overview
You're a red-teamer assessing Wishful Thinking Inc. They run an old FTP service that hands back whatever file path a client asks for and never checks it — a directory-traversal vulnerability. First you'll exploit it to reach files you were never meant to see; then you'll flip to the blue team and use Snort + packet analysis to detect the attack and prove exactly what it reached.

## Tools Used
- Ubuntu (Linux)
- Wireshark / tcpdump
- Snort

## What I learned
- Exploited a path traversal vulnerability using ../ to access restricted files outside the FTP directory.
- Retrieved sensitive information, including the server's operating system details, /etc/shadow, and confidential earnings data.
- Analyzed a .pcapng file using tcpdump to identify successful HTTP requests (200 OK) and unauthorized file access.
- Created custom Snort rules to detect directory traversal attempts and reviewed generated alerts.
- Tested URL-encoded traversal (%2e%2e%2f) and developed an additional detection rule.
- Learned how proper path validation and restricted file permissions can prevent or limit path traversal attacks.

## Screenshots
<img width="404" height="557" alt="image" src="https://github.com/user-attachments/assets/7efc10ca-1019-4dea-bf5c-441b90777223" />

<img width="407" height="219" alt="image" src="https://github.com/user-attachments/assets/4b3207bd-4131-43e0-9724-8ed26afe6b34" />

<img width="404" height="267" alt="image" src="https://github.com/user-attachments/assets/0112e758-5999-4cec-bb02-7a75606ed34b" />

<img width="407" height="155" alt="image" src="https://github.com/user-attachments/assets/a009075f-5e48-43aa-89b8-de368c1d8ec1" />

## Screenshot of Stretch Challenge
<img width="407" height="398" alt="image" src="https://github.com/user-attachments/assets/82d13113-f145-4dde-b8a1-b4b6bcd2d695" />
