\# Question Bank — Domain 3 (Security Architecture)



\## How to Use

\- Answer questions without looking at the answer key.

\- Write answers as: `1C 2A 3B ...`

\- Review explanations for every missed question.

\- Log results in `progress/practice-scores.md`.



---# Question Bank — Domain 3 (Security Architecture)



\## How to Use

\- Answer questions without looking at the answer key.

\- Write answers as: `1C 2A 3B ...`

\- Review explanations for every missed question.

\- Log results in `progress/practice-scores.md`.



---



\## Questions



\### Q1 — Segmentation Goal



Which outcome is the PRIMARY goal of network segmentation?



A) Increase bandwidth  

B) Reduce lateral movement after compromise  

C) Remove the need for patching  

D) Replace encryption



---



\### Q2 — DMZ Purpose



A company hosts a public web server that must be reachable from the internet but isolated from internal systems. Where should it be placed?



A) In the internal LAN  

B) In a DMZ  

C) On a management VLAN  

D) Behind the database subnet only



---



\### Q3 — Secure Remote Access



Which option BEST provides secure remote access to internal resources while reducing exposure of those resources to the internet?



A) Port forwarding RDP to a workstation  

B) VPN with MFA  

C) Disable firewall rules on the edge  

D) Use HTTP for remote admin tools



---



\### Q4 — Secure Protocol Choice



Which protocol is BEST for secure remote administration of Linux systems?



A) Telnet  

B) SSH  

C) FTP  

D) HTTP



---



\### Q5 — Cloud Responsibility



In a typical public cloud model, which statement is MOST accurate?



A) The customer is responsible for the physical security of the data center  

B) The cloud provider is responsible for all application security  

C) Responsibilities are shared between provider and customer  

D) The provider is not responsible for hypervisor security



---



\### Q6 — WAF Use Case



Which control is MOST appropriate to help protect a public web application from common web attacks like SQL injection?



A) NAC (Network Access Control)  

B) WAF (Web Application Firewall)  

C) Disk encryption  

D) Screen privacy filters



---



\### Q7 — DLP Focus



What is the PRIMARY goal of Data Loss Prevention (DLP)?



A) Prevent malware infections  

B) Prevent unauthorized data exfiltration  

C) Improve availability during outages  

D) Replace access control lists



---



\### Q8 — Bastion Host



A company requires administrators to access internal servers only through a hardened jump box with strong logging. This is BEST described as a:



A) Honeypot  

B) Bastion host / jump server  

C) Proxy cache server  

D) SIEM collector



---



\### Q9 — Secure Wi-Fi



Which configuration MOST improves Wi-Fi security for a business network?



A) WEP with a long key  

B) WPA2/WPA3-Enterprise with 802.1X  

C) Open Wi-Fi with a captive portal only  

D) Disable SSID broadcast



---



\### Q10 — High Availability



Which design choice MOST directly improves availability for a critical system?



A) Single firewall with default rules  

B) Redundant components with failover  

C) Shared admin accounts  

D) Disabling logs to save disk space



---



\## Answer Key \& Explanations



\### Q1

\*\*Correct Answer:\*\* B — Reduce lateral movement after compromise  

Segmentation limits how far an attacker can move if one segment is breached.



\### Q2

\*\*Correct Answer:\*\* B — In a DMZ  

DMZ isolates public-facing systems from the internal network.



\### Q3

\*\*Correct Answer:\*\* B — VPN with MFA  

A VPN reduces direct exposure and MFA helps protect against stolen passwords.



\### Q4

\*\*Correct Answer:\*\* B — SSH  

SSH provides encrypted remote shell access; Telnet is plaintext.



\### Q5

\*\*Correct Answer:\*\* C — Responsibilities are shared  

Providers secure underlying infrastructure; customers secure configs, identities, data, and apps (varies by model).



\### Q6

\*\*Correct Answer:\*\* B — WAF  

A WAF is designed to filter/inspect web traffic and block common web attacks.



\### Q7

\*\*Correct Answer:\*\* B — Prevent unauthorized data exfiltration  

DLP focuses on controlling sensitive data movement (email, web upload, USB, etc.).



\### Q8

\*\*Correct Answer:\*\* B — Bastion host / jump server  

A hardened, monitored entry point for administrative access.



\### Q9

\*\*Correct Answer:\*\* B — WPA2/WPA3-Enterprise with 802.1X  

Enterprise Wi-Fi uses strong authentication and centralized control, unlike WEP/open networks.



\### Q10

\*\*Correct Answer:\*\* B — Redundant components with failover  

Availability improves most with redundancy and automatic failover.





\## Questions



\### Q1 — Segmentation Goal



Which outcome is the PRIMARY goal of network segmentation?



A) Increase bandwidth  

B) Reduce lateral movement after compromise  

C) Remove the need for patching  

D) Replace encryption



---



\### Q2 — DMZ Purpose



A company hosts a public web server that must be reachable from the internet but isolated from internal systems. Where should it be placed?



A) In the internal LAN  

B) In a DMZ  

C) On a management VLAN  

D) Behind the database subnet only



---



\### Q3 — Secure Remote Access



Which option BEST provides secure remote access to internal resources while reducing exposure of those resources to the internet?



A) Port forwarding RDP to a workstation  

B) VPN with MFA  

C) Disable firewall rules on the edge  

D) Use HTTP for remote admin tools



---



\### Q4 — Secure Protocol Choice



Which protocol is BEST for secure remote administration of Linux systems?



A) Telnet  

B) SSH  

C) FTP  

D) HTTP



---



\### Q5 — Cloud Responsibility



In a typical public cloud model, which statement is MOST accurate?



A) The customer is responsible for the physical security of the data center  

B) The cloud provider is responsible for all application security  

C) Responsibilities are shared between provider and customer  

D) The provider is not responsible for hypervisor security



---



\### Q6 — WAF Use Case



Which control is MOST appropriate to help protect a public web application from common web attacks like SQL injection?



A) NAC (Network Access Control)  

B) WAF (Web Application Firewall)  

C) Disk encryption  

D) Screen privacy filters



---



\### Q7 — DLP Focus



What is the PRIMARY goal of Data Loss Prevention (DLP)?



A) Prevent malware infections  

B) Prevent unauthorized data exfiltration  

C) Improve availability during outages  

D) Replace access control lists



---



\### Q8 — Bastion Host



A company requires administrators to access internal servers only through a hardened jump box with strong logging. This is BEST described as a:



A) Honeypot  

B) Bastion host / jump server  

C) Proxy cache server  

D) SIEM collector



---



\### Q9 — Secure Wi-Fi



Which configuration MOST improves Wi-Fi security for a business network?



A) WEP with a long key  

B) WPA2/WPA3-Enterprise with 802.1X  

C) Open Wi-Fi with a captive portal only  

D) Disable SSID broadcast



---



\### Q10 — High Availability



Which design choice MOST directly improves availability for a critical system?



A) Single firewall with default rules  

B) Redundant components with failover  

C) Shared admin accounts  

D) Disabling logs to save disk space



---



\## Answer Key \& Explanations



\### Q1

\*\*Correct Answer:\*\* B — Reduce lateral movement after compromise  

Segmentation limits how far an attacker can move if one segment is breached.



\### Q2

\*\*Correct Answer:\*\* B — In a DMZ  

DMZ isolates public-facing systems from the internal network.



\### Q3

\*\*Correct Answer:\*\* B — VPN with MFA  

A VPN reduces direct exposure and MFA helps protect against stolen passwords.



\### Q4

\*\*Correct Answer:\*\* B — SSH  

SSH provides encrypted remote shell access; Telnet is plaintext.



\### Q5

\*\*Correct Answer:\*\* C — Responsibilities are shared  

Providers secure underlying infrastructure; customers secure configs, identities, data, and apps (varies by model).



\### Q6

\*\*Correct Answer:\*\* B — WAF  

A WAF is designed to filter/inspect web traffic and block common web attacks.



\### Q7

\*\*Correct Answer:\*\* B — Prevent unauthorized data exfiltration  

DLP focuses on controlling sensitive data movement (email, web upload, USB, etc.).



\### Q8

\*\*Correct Answer:\*\* B — Bastion host / jump server  

A hardened, monitored entry point for administrative access.



\### Q9

\*\*Correct Answer:\*\* B — WPA2/WPA3-Enterprise with 802.1X  

Enterprise Wi-Fi uses strong authentication and centralized control, unlike WEP/open networks.



\### Q10

\*\*Correct Answer:\*\* B — Redundant components with failover  

Availability improves most with redundancy and automatic failover.



