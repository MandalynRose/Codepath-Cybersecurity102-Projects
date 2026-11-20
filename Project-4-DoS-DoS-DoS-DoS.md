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
