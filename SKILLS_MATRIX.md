# Cybersecurity Skills Matrix - Red Team Path

[![Focus](https://img.shields.io/badge/Focus-Red%20Team%20Foundations-d32f2f?style=for-the-badge)](#1-offensive-security-fundamentals)
[![Track](https://img.shields.io/badge/Track-Skills%20Matrix-5c6ac4?style=for-the-badge)](#legend)

This document tracks the knowledge required for entry-level red team, offensive security, and adversary emulation roles. Emphasis is on understanding how systems are broken, abused, and evaded—not merely defended.

## Legend

- `[ ]` Not started
- `[~]` In progress
- `[x]` Demonstrated (lab, exploit, write-up, or code)

---

## 1. Offensive Security Fundamentals
- `[~]` CIA triad from an attacker perspective
- `[ ]` Threat modeling focused on attacker objectives
- `[ ]` Attack surface identification
- `[ ]` Authentication vs. authorization abuse scenarios
- `[ ]` Privilege escalation concepts (vertical and horizontal)
- `[ ]` Common attacker tradecraft (living off the land, credential abuse)
- `[ ]` OPSEC basics (noise reduction, artifact awareness)
- `[ ]` Ethics, legality, and scope boundaries

## 2. Networking for Attackers

### Core Mental Models
- `[~]` View networks through visibility, reach, and trust
- `[ ]` Identify attack surfaces created by network design
- `[ ]` Infer network behavior from packet responses (not diagrams)

### IP, Routing, and Segmentation
- `[ ]` Identify subnets, gateways, and routing boundaries
- `[ ]` Distinguish segmentation assumptions vs. enforcement
- `[ ]` Understand NAT behavior for attribution/pivoting
- `[ ]` Identify internal vs. external trust boundaries

### ARP and Local Network Abuse
- `[ ]` Understand ARP behavior and trust model
- `[ ]` Determine when ARP spoofing is feasible vs. mitigated
- `[ ]` Recognize artifacts/detections tied to ARP abuse

### DNS and Name Resolution
- `[ ]` Enumerate hosts/services via DNS
- `[ ]` Understand split-horizon DNS and internal naming
- `[ ]` Abuse name-resolution order (especially Windows)
- `[ ]` Spot information leakage from misconfigurations

### TCP, UDP, and Port Behavior
- `[ ]` Interpret TCP handshake states and what they reveal
- `[ ]` Read RST vs. DROP responses during scans
- `[ ]` Perform service fingerprinting beyond open/closed
- `[ ]` Understand UDP discovery challenges/opportunities

### HTTP/HTTPS as an Attack Channel
- `[ ]` Use HTTP(S) for tunneling and C2
- `[ ]` Analyze headers, cookies, authentication flows
- `[ ]` Identify proxy behavior and trust assumptions
- `[ ]` Understand TLS termination and inspection impacts

### Windows-Centric Network Protocols
- `[ ]` Explain SMB’s role in enumeration and lateral movement
- `[ ]` See LDAP as a directory/intel source
- `[ ]` Understand Kerberos concepts (tickets, trust, abuse paths)
- `[ ]` Identify AD indicators within network traffic

### Traffic Analysis and OPSEC
- `[ ]` Capture/analyze basic network traffic
- `[ ]` Distinguish logged vs. invisible traffic to defenders
- `[ ]` Understand how attackers blend traffic to reduce detection
- `[ ]` Recognize noisy vs. stealthy behaviors

### Tooling (Conceptual Mastery)
- `[ ]` Use Nmap intentionally (timing, flags, stealth)
- `[ ]` Use packet capture tools to answer specific questions
- `[ ]` Rely on OS-native tools for discovery/pivoting
- `[ ]` Explain why each tool or technique was chosen
