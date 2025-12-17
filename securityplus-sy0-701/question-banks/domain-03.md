# Question Bank – Domain 3 (Security Architecture)

## How to Use
- Answer without looking at the answer key.
- Record responses (e.g., `1B 2D 3C`) for quick review.
- Study every missed question and log the run in `progress/practice-scores.md`.

---

## Questions

### Q1 – Segmentation Goal
What is the PRIMARY goal of network segmentation?

A) Increase bandwidth  
B) Reduce lateral movement after compromise  
C) Remove the need for patching  
D) Replace encryption

---

### Q2 – DMZ Purpose
A company must host a public web server that is reachable from the internet but isolated from internal systems. Where should it reside?

A) Internal LAN  
B) Demilitarized zone (DMZ)  
C) Management VLAN  
D) Database subnet only

---

### Q3 – Secure Remote Access
Which option BEST provides secure remote access to internal resources while limiting exposure?

A) Port forwarding RDP directly to endpoints  
B) VPN with MFA  
C) Disable edge firewall rules  
D) HTTP-based admin tools on the internet

---

### Q4 – Secure Protocol Choice
Which protocol is BEST for remote administration of Linux servers?

A) Telnet  
B) SSH  
C) FTP  
D) HTTP

---

### Q5 – Cloud Responsibility
In a public cloud model, which statement is MOST accurate?

A) Customers handle data-center physical security  
B) Providers own all application security  
C) Responsibilities are shared between provider and customer  
D) Providers are not responsible for hypervisor security

---

### Q6 – WAF Use Case
Which control MOST effectively protects a public web app from SQL injection?

A) NAC  
B) Web Application Firewall (WAF)  
C) Disk encryption  
D) Privacy screen filters

---

### Q7 – DLP Focus
What is the PRIMARY goal of Data Loss Prevention (DLP)?

A) Stop malware infections  
B) Prevent unauthorized data exfiltration  
C) Improve availability  
D) Replace access control lists

---

### Q8 – Bastion Host
Administrators must connect to internal servers through a hardened jump box with logging. This component is a:

A) Honeypot  
B) Bastion host / jump server  
C) Proxy cache server  
D) SIEM collector

---

### Q9 – Secure Wi-Fi
Which configuration MOST improves business Wi-Fi security?

A) WEP with a long key  
B) WPA2/WPA3-Enterprise with 802.1X  
C) Open Wi-Fi plus captive portal  
D) Disable SSID broadcast

---

### Q10 – High Availability
Which design choice MOST directly improves availability for critical systems?

A) Single firewall with default rules  
B) Redundant components with failover  
C) Shared admin accounts  
D) Disable logging to save disk space

---

## Answer Key and Explanations

### Q1
**Answer:** B – Segmentation limits an attacker’s lateral movement after a compromise.

### Q2
**Answer:** B – A DMZ isolates public-facing services from the internal network.

### Q3
**Answer:** B – A VPN with MFA protects remote sessions and reduces exposed services.

### Q4
**Answer:** B – SSH encrypts administrative sessions; Telnet/HTTP/FTP do not.

### Q5
**Answer:** C – Cloud security responsibilities are shared based on the service model.

### Q6
**Answer:** B – A WAF inspects HTTP(S) traffic and blocks common web exploits.

### Q7
**Answer:** B – DLP focuses on preventing sensitive data from leaving authorized channels.

### Q8
**Answer:** B – A bastion host (jump box) is a hardened single entry point for admins.

### Q9
**Answer:** B – WPA2/WPA3-Enterprise plus 802.1X delivers strong authentication and encryption.

### Q10
**Answer:** B – Redundancy with failover is the core of high-availability design.
