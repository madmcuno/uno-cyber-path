# pfSense Enterprise Network Segmentation Lab

## Overview
This lab demonstrates the design, deployment, hardening, and validation of an enterprise-style network perimeter using pfSense as a stateful firewall. The environment implements proper network segmentation, least-privilege access, secure service publishing, and a dedicated management plane.

The lab was built and tested entirely in VirtualBox using multiple Linux virtual machines to simulate realistic traffic flows and attack surfaces.

> [!NOTE]
> All validation steps were performed in a local lab. Adapt IPs and hardening steps to match your environment.

---

## Objectives
- Build a firewall-centric network architecture
- Implement LAN, DMZ, and MGMT segmentation
- Securely publish a DMZ web service to WAN
- Restrict and harden inbound and outbound traffic
- Enforce administrative access through a dedicated MGMT network
- Validate security controls through positive and negative testing

---

## Network Architecture

### Networks
| Network | Purpose | Subnet / Notes |
| --- | --- | --- |
| WAN | Upstream / Internet | VirtualBox NAT |
| LAN | User network | 10.10.10.0/24 |
| DMZ | Public-facing services | 10.10.20.0/24 |
| MGMT | Firewall administration | 10.10.30.0/24 |

### Virtual Machines
| Hostname | Role |
| --- | --- |
| FW-EDGE | pfSense firewall |
| LAN-CLIENT-01 | Internal client |
| DMZ-SERVER-01 | Public web server |
| MGMT-ADMIN-01 | Administrative host |

---

## IP Addressing
| Interface / Host | Address |
| --- | --- |
| pfSense LAN | 10.10.10.1 |
| pfSense DMZ | 10.10.20.1 |
| pfSense MGMT | 10.10.30.1 |
| LAN client | DHCP (10.10.10.x) |
| DMZ server | 10.10.20.10 (static) |
| MGMT admin | 10.10.30.10 (static) |

---

## Firewall Design

### LAN Policy
- Full outbound access
- Explicit block to firewall admin interface
- No management access allowed

### DMZ Policy
Outbound allowed:
- DNS (53 to pfSense)
- HTTPS (443)

Inbound allowed:
- HTTPS (443) via WAN NAT

Blocked:
- ICMP
- LAN access
- All other protocols

### MGMT Policy
- Access to pfSense admin interface only
- No internet access
- No LAN or DMZ access

---

## Inbound Hardening (WAN)

### NAT and Port Forwarding
- WAN TCP 443 forwarded to DMZ-SERVER-01:443
- HTTP (80) disabled

### Security Controls
- HTTPS-only service exposure
- Source IP restriction using aliases
- Rate limiting using pfSense limiters via floating rules
- Firewall logging enabled
- Bogon networks blocked on WAN

---

## HTTPS Configuration
- Nginx deployed on DMZ server
- Self-signed TLS certificate
- HTTP redirected to HTTPS
- Port 80 disabled at firewall

---

## Management Plane Security
- pfSense admin interface reachable only from MGMT network
- LAN and DMZ explicitly blocked from admin access
- Anti-lockout rule disabled after MGMT validation
- Explicit LAN to firewall block rule enforced

> [!IMPORTANT]
> Keep administrative access isolated. A reachable management plane from LAN or DMZ defeats segmentation.

---

## Validation and Testing

Positive tests:
- WAN HTTPS to DMZ service loads successfully
- MGMT admin can access pfSense web UI
- LAN outbound internet access works

Negative tests:
- LAN blocked from pfSense admin interface
- DMZ blocked from LAN
- DMZ blocked from ICMP and non-web traffic
- MGMT blocked from internet
- HTTP access fails while HTTPS succeeds

Rate limiting:
- Traffic observed in limiter queues via pfTop
- Limiter enforcement verified using repeated requests

> [!TIP]
> Run each test from the intended zone to confirm both routing and rule intent, not just service reachability.

---

## Troubleshooting and Lessons Learned

Key issues encountered:
- Host-only network mis-binding in VirtualBox
- DHCP authority conflicts
- pfSense DHCP binding failures due to corrupted state
- Anti-lockout rule overriding segmentation intent
- NAT auto-rules not supporting limiters directly

Resolutions:
- Reduced environment to one host-only adapter per zone
- Clean pfSense reinstall after config corruption
- Explicit firewall block rules instead of implicit allow
- Floating rules used for traffic shaping
- State resets required after rule changes

---

## Security Takeaways
- Firewall rules are first-match
- "Allow LAN to any" includes the firewall itself
- Management access must be explicitly restricted
- Rate limiting belongs in filtering logic, not NAT
- DMZs should never implicitly trust LAN or WAN

---

## Final Result
This lab results in a production-grade perimeter design demonstrating:
- Proper network segmentation
- Hardened service publishing
- Dedicated management plane
- Realistic firewall rule design
- Professional troubleshooting methodology

---

## Future Enhancements
- Centralized syslog and SIEM ingestion
- IDS/IPS integration (Suricata)
- Certificate authority integration
- Backup and restore automation
- Attack simulation and detection

---

Status: Complete

Skill Areas: Networking, Firewalls, Linux, Security Architecture, Troubleshooting
