\# Entry-Level Cybersecurity Mock Interview (v2)



Purpose:  

Prepare for entry-level cybersecurity interviews by demonstrating \*\*clear thinking under pressure\*\*, real-world awareness, and basic operational capability.



---



\## 1. Cybersecurity Fundamentals



\### Q1. What is the CIA triad?



\*\*Strong Sample Answer\*\*  

Confidentiality prevents unauthorized access, integrity prevents unauthorized modification, and availability ensures systems remain accessible when needed.



\*\*Pressure Questions + Answers\*\*

\- \*\*Which is most impacted by ransomware?\*\*  

&nbsp; Availability first, then integrity.

\- \*\*Can improving availability reduce confidentiality?\*\*  

&nbsp; Yes, if redundancy or access is expanded without proper controls.

\- \*\*Hospital system—what’s priority?\*\*  

&nbsp; Availability, but never at the cost of patient data confidentiality.



\*\*Real-World Breach Scenario\*\*  

Ransomware encrypts hospital systems, halting patient care.



\*\*Linux / Windows Follow-Ups\*\*

\- Linux: `uptime`, `df -h`, `systemctl status`

\- Windows: `tasklist`, `Get-Service`, `wevtutil qe System`



\*\*Common Mistakes\*\*

\- Treating CIA as equal in all environments

\- Ignoring business impact



---



\### Q2. Authentication vs Authorization



\*\*Strong Sample Answer\*\*  

Authentication verifies identity. Authorization determines access after identity is verified.



\*\*Pressure Questions + Answers\*\*

\- \*\*Can authorization exist without authentication?\*\*  

&nbsp; No—authorization assumes identity.

\- \*\*Where does MFA fit?\*\*  

&nbsp; Authentication.

\- \*\*How does least privilege help?\*\*  

&nbsp; Limits blast radius after compromise.



\*\*Real-World Breach Scenario\*\*  

Compromised credentials grant excessive access due to poor RBAC.



\*\*Linux / Windows Follow-Ups\*\*

\- Linux: `id`, `groups`, `sudo -l`

\- Windows: `whoami /groups`, `Get-LocalGroup`



\*\*Common Mistakes\*\*

\- Using terms interchangeably

\- Ignoring access reviews



---



\### Q3. What is phishing?



\*\*Strong Sample Answer\*\*  

Phishing is social engineering designed to trick users into revealing information or executing malicious actions.



\*\*Pressure Questions + Answers\*\*

\- \*\*User clicked link—now what?\*\*  

&nbsp; Isolate system, report, preserve evidence.

\- \*\*How do you reduce phishing risk?\*\*  

&nbsp; Training, email filtering, MFA.

\- \*\*Why is spear phishing harder?\*\*  

&nbsp; Personalization increases trust.



\*\*Real-World Breach Scenario\*\*  

Business Email Compromise leads to fraudulent wire transfer.



\*\*Linux / Windows Follow-Ups\*\*

\- Linux: `grep mail.log`, `journalctl`

\- Windows: `Get-WinEvent -LogName Security`



\*\*Common Mistakes\*\*

\- Blaming users

\- Failing to escalate quickly



---



\## 2. Operating Systems \& Networking Basics



\### Q4. What happens when you type a URL into a browser?



\*\*Strong Sample Answer\*\*  

DNS resolution, TCP connection, TLS handshake, HTTP request/response.



\*\*Pressure Questions + Answers\*\*

\- \*\*Where can attackers intercept?\*\*  

&nbsp; DNS, network, or TLS downgrade.

\- \*\*What fails if DNS is down?\*\*  

&nbsp; Name resolution.

\- \*\*Why HTTPS?\*\*  

&nbsp; Encryption and integrity.



\*\*Real-World Breach Scenario\*\*  

DNS hijacking redirects users to malicious site.



\*\*Linux / Windows Follow-Ups\*\*

\- Linux: `dig`, `ss -tuln`

\- Windows: `nslookup`, `netstat -ano`



\*\*Common Mistakes\*\*

\- Skipping DNS

\- Treating HTTPS as “just encryption”



---



\### Q5. TCP vs UDP



\*\*Strong Sample Answer\*\*  

TCP is reliable and connection-oriented. UDP is fast and connectionless.



\*\*Pressure Questions + Answers\*\*

\- \*\*Why UDP in amplification attacks?\*\*  

&nbsp; No handshake, spoofable source IPs.

\- \*\*Can TCP be abused?\*\*  

&nbsp; Yes—SYN floods.

\- \*\*Is UDP insecure by default?\*\*  

&nbsp; No—depends on use case.



\*\*Real-World Breach Scenario\*\*  

DNS amplification DDoS disrupts public services.



\*\*Linux / Windows Follow-Ups\*\*

\- Linux: `tcpdump`, `ss -u`

\- Windows: `netstat -an`, `Get-NetUDPEndpoint`



\*\*Common Mistakes\*\*

\- Calling UDP “unsafe”

\- Ignoring protocol context



---



\### Q6. What is a firewall?



\*\*Strong Sample Answer\*\*  

A firewall filters traffic based on rules like IP, port, and protocol.



\*\*Pressure Questions + Answers\*\*

\- \*\*What bypasses firewalls?\*\*  

&nbsp; Allowed ports, insider threats.

\- \*\*Flat network risk?\*\*  

&nbsp; Easy lateral movement.

\- \*\*Host vs network firewall?\*\*  

&nbsp; Local vs perimeter control.



\*\*Real-World Breach Scenario\*\*  

Attacker pivots laterally after initial compromise.



\*\*Linux / Windows Follow-Ups\*\*

\- Linux: `iptables -L`, `ufw status`

\- Windows: `Get-NetFirewallRule`



\*\*Common Mistakes\*\*

\- Treating firewalls as full security

\- No segmentation



---



\## 3. Security Tools \& Concepts



\### Q7. Antivirus vs EDR vs SIEM



\*\*Strong Sample Answer\*\*  

Antivirus detects known malware, EDR monitors endpoint behavior, SIEM aggregates and correlates logs.



\*\*Pressure Questions + Answers\*\*

\- \*\*Why won’t SIEM stop malware?\*\*  

&nbsp; It detects; it doesn’t block.

\- \*\*EDR alert no response—then?\*\*  

&nbsp; Alerts are useless without action.

\- \*\*Post-incident—most useful?\*\*  

&nbsp; SIEM.



\*\*Real-World Breach Scenario\*\*  

EDR detects lateral movement; SIEM correlates domain-wide activity.



\*\*Linux / Windows Follow-Ups\*\*

\- Linux: `ps aux`, `last`, `/var/log`

\- Windows: `Get-Process`, `Get-WinEvent`



\*\*Common Mistakes\*\*

\- Treating tools as interchangeable

\- No alert ownership



---



\### Q8. What are logs and why do they matter?



\*\*Strong Sample Answer\*\*  

Logs provide visibility, detection, accountability, and forensic evidence.



\*\*Pressure Questions + Answers\*\*

\- \*\*What makes logs unreliable?\*\*  

&nbsp; No NTP, gaps, tampering.

\- \*\*Why time sync matters?\*\*  

&nbsp; Correlation accuracy.

\- \*\*Reduce alert fatigue?\*\*  

&nbsp; Tuning and baselining.



\*\*Real-World Breach Scenario\*\*  

Missing logs delay breach detection.



\*\*Linux / Windows Follow-Ups\*\*

\- Linux: `journalctl`, `chronyc tracking`

\- Windows: `w32tm /query /status`



\*\*Common Mistakes\*\*

\- Logging everything, analyzing nothing



---



\## 4. Incident Response



\### Q9. Suspected malware—first step?



\*\*Strong Sample Answer\*\*  

Isolate the system, preserve evidence, escalate per procedure.



\*\*Pressure Questions + Answers\*\*

\- \*\*Who do you notify?\*\*  

&nbsp; SOC / IR lead.

\- \*\*When reimage?\*\*  

&nbsp; After investigation.

\- \*\*Executive device?\*\*  

&nbsp; Same process, higher urgency.



\*\*Real-World Breach Scenario\*\*  

Malware spreads due to delayed isolation.



\*\*Linux / Windows Follow-Ups\*\*

\- Linux: `ip link set down`, `ps aux`

\- Windows: Disable NIC, `tasklist`



\*\*Common Mistakes\*\*

\- Rebooting

\- Acting without authorization



---



\## Safe Answers When You Don’t Know

\- “I’d verify by checking logs or documentation.”

\- “I’d escalate to the appropriate team.”

\- “I don’t have that memorized, but I know where to find it.”



---



\## Rapid-Fire Drill

\- What is least privilege?

\- What port is HTTPS?

\- Difference between hashing and encryption?

\- What does DNS do?

\- Why centralize logs?



---



\## First 90 Days Mindset

\- Learn the environment

\- Understand escalation paths

\- Master logs before tools

\- Ask questions early



---



\## Confidence Signals Interviewers Look For

\- Calm under pressure

\- Clear escalation

\- Process over ego

\- Business-aware decisions



