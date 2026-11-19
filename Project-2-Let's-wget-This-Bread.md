# Project 2: Let's wget This Bread

## Overview
In real incident response, one of the first questions an analyst asks is: "what changed on this system, and when?" The Linux Audit daemon answers that question by watching specific files and directories for modifications and recording exactly which process triggered each change.

In this project, you'll write Audit rules to monitor a set of protected files, then run three attack scripts that silently modify those files. Your job is to use the audit logs to figure out which attack changed which file — the same attribution work analysts do after a real breach.

## Tools Used
- Azure Virtual Machine
- Ubuntu (Linux)
- Auditd (auditctl, ausearch)

## What I Learned
- Learned how to use Auditd to monitor changes made to files in Linux.
- Created audit rules using auditctl to track 10 protected files.
- Used ausearch to check the logs and find which files were changed.
- Found that attack-a modified clouddia.txt, attack-b modified oakley.txt, and attack-c modified precipitation.csv.
- Learned how audit logs can help identify which files were affected during a cyberattack.

## Screenshot
<img width="857" height="547" alt="image" src="https://github.com/user-attachments/assets/4bd32365-74e3-44e1-987c-92d480759965" />
