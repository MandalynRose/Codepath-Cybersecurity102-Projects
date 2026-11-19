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
