# Project 4: DoS DoS DoS DoS DoS DoS DoS DoS DoS DoS DoS DoS DoS DoS DoS DoS DoS DoS DoS DoS DoS DoS DoS DoS DoS

## Overview
Cyber attacks that have increased in popularity over the years are DDoS (Distributed Denial of Service) attacks, even affecting top tech companies like Google and Amazon. A simpler version of the attack is DoS (Denial of Service), a scheme where the attacker operates from a single internet connection rather than many.

For this project, we'll be running a type of DoS attack named Slowloris against the local server on our VM and design rules in nginx to mitigate the attack. Unlike volumetric attacks that flood a server with raw traffic, Slowloris holds connections open by sending partial HTTP requests deliberately slowly — exhausting connection limits without generating the volume that traditional DoS defenses look for. For bonus points, we'll also compare some .pcap files to see which one shows server traffic set to mitigate DoS attacks, and which one shows a vulnerable server.

## Tools Used
- Ubuntu (Linux)
- Nginx
- Slowloris
- Netdata
- Firefox

## What I learned
- Learned how DoS attacks affect servers.
- Used Slowloris to simulate a DoS attack.
- Monitored TCP connections using Netdata.
- Added security rules to Nginx to help prevent DoS attacks.
- Compared server activity before and after adding protection.

## Screenshots
A screenshot of your  nginx config file(s) with your DoS mitigation rules implemented:
<img width="530" height="297" alt="image" src="https://github.com/user-attachments/assets/ae193b04-3d84-4b81-8007-8003b9118a86" />
<img width="528" height="318" alt="image" src="https://github.com/user-attachments/assets/8540fb10-53c3-4b2a-858b-ceaa831a31f3" />

A screenshot of your Netdata TCP connections graph during the unprotected Slowloris attack:
<img width="528" height="458" alt="image" src="https://github.com/user-attachments/assets/bed56977-358a-4de0-9af5-b26bd6c42efa" />

A screenshot of your Netdata TCP connections graph during the protected Slowloris attack:
<img width="529" height="425" alt="image" src="https://github.com/user-attachments/assets/430627d1-becb-467f-9ac2-3d1444653c67" />

An explanation of the differences between the unprotected and protected Slowloris attacks, in your own words:
- During the unprotected Slowloris attack, Nginx had no added DoS mitigation rules to limit the attack. During the protected attack, I added security rules to limit connections and request timeouts (the gap is wider). But, the TCP graph still showed high connection spikes (in the pic)  so the protection did not clearly reduce the attack's impact.
