# Mr. Robot CTF – Linux Privilege Escalation

## Objective
Gain root access to a vulnerable Linux machine by identifying and exploiting misconfigurations and authentication weaknesses.

## Environment
- Platform: TryHackMe
- Attacker OS: Kali Linux
- Target OS: Ubuntu-based Linux
- Network: VPN-isolated lab

## Methodology
- Enumerated open services (SSH, HTTP, HTTPS)
- Discovered sensitive files via robots.txt
- Identified a WordPress login portal
- Recovered valid credentials and gained initial user access
- Enumerated SUID binaries on the system
- Identified a misconfigured SUID root binary (nmap)
- Exploited interactive command execution to spawn a root shell
- Retrieved all three hidden keys

## Key Security Concepts Demonstrated
- Service enumeration
- Linux file permissions
- SUID-based privilege escalation
- Authentication weaknesses
- Root-level system access

## Defensive Takeaways
- Avoid assigning SUID permissions to interactive programs
- Regularly audit SUID binaries
- Restrict command execution paths in privileged programs
