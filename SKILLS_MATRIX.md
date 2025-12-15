\# Cybersecurity Skills Matrix — Red Team Path



This document tracks the knowledge and skills required for entry-level red team,

offensive security, and adversary simulation roles.



The focus is on understanding how systems are broken, abused, and evaded —

not just how they are defended.



Legend:

\[ ] Not started

\[~] In progress

\[x] Demonstrated (lab, exploit, writeup, or code)



---



\## 1. Offensive Security Fundamentals

\[~] CIA triad from an attacker perspective

\[ ] Threat modeling (how attackers think, not compliance models)

\[ ] Attack surface identification

\[ ] Authentication vs authorization abuse cases

\[ ] Privilege escalation concepts (vertical vs horizontal)

\[ ] Common attacker tradecraft (living off the land, credential abuse)

\[ ] OPSEC basics (noise reduction, artifact awareness)

\[ ] Ethics, legality, and scope boundaries







## 2. Networking for Attackers

### Core Mental Models
[~] Understand networks from an abuse perspective (visibility, reach, trust)
[ ] Identify attack surfaces created by network design
[ ] Infer network behavior from packet responses (not diagrams)

### IP, Routing, and Segmentation
[ ] Identify subnets, gateways, and routing boundaries
[ ] Recognize segmentation assumptions vs actual enforcement
[ ] Understand NAT behavior and its implications for attribution and pivoting
[ ] Identify internal vs external trust boundaries

### ARP and Local Network Abuse
[ ] Understand ARP behavior and trust model
[ ] Identify when ARP spoofing is feasible vs mitigated
[ ] Recognize artifacts and detection opportunities of ARP abuse

### DNS and Name Resolution
[ ] Enumerate hostnames and services via DNS
[ ] Understand split-horizon DNS and internal naming conventions
[ ] Abuse name resolution order (especially in Windows environments)
[ ] Identify information leakage via DNS misconfiguration

### TCP, UDP, and Port Behavior
[ ] Understand TCP handshake states and what they reveal
[ ] Interpret RST vs DROP responses during scanning
[ ] Perform service fingerprinting beyond open/closed
[ ] Understand UDP discovery challenges and opportunities

### HTTP / HTTPS as an Attack Channel
[ ] Understand HTTP as a tunneling and C2 mechanism
[ ] Analyze headers, cookies, and authentication flows
[ ] Identify proxy behavior and trust assumptions
[ ] Understand TLS termination points and inspection implications

### Windows-Centric Network Protocols
[ ] Understand SMB’s role in enumeration and lateral movement
[ ] Understand LDAP as a directory and intelligence source
[ ] Understand Kerberos at a conceptual level (tickets, trust, abuse paths)
[ ] Identify network-based indicators of Active Directory environments

### Traffic Analysis and OPSEC
[ ] Capture and analyze basic network traffic
[ ] Identify what traffic is logged vs invisible to defenders
[ ] Understand how attackers blend traffic to reduce detection
[ ] Recognize noisy vs stealthy network behaviors

### Tooling (Conceptual Mastery)
[ ] Use nmap with intent (timing, flags, stealth tradeoffs)
[ ] Use packet capture tools to answer specific questions
[ ] Use OS-native networking tools for discovery and pivoting
[ ] Explain *why* a tool was used, not just how



