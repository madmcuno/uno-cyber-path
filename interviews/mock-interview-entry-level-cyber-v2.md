# Entry-Level Cybersecurity Mock Interview (v2)

Purpose: prepare for entry-level cybersecurity interviews by demonstrating clear thinking under pressure, real-world awareness, and basic operational capability.

---

## 1. Cybersecurity Fundamentals

### Q1. What is the CIA triad?

![Strong Sample Answer](https://img.shields.io/badge/Strong%20Sample%20Answer-f9f2e1?style=flat)

Confidentiality prevents unauthorized access, integrity prevents unauthorized modification, and availability ensures systems remain accessible when needed.

> ![Neutral takeaway](https://img.shields.io/badge/Neutral%20takeaway-d7cfc0?style=flat): the priority can shift by environment and business impact.

![Pressure Questions + Answers](https://img.shields.io/badge/Pressure%20Questions%20%2B%20Answers-e26a58?style=flat)

- **Which is most impacted by ransomware?**
  Availability first, then integrity.
- **Can improving availability reduce confidentiality?**
  Yes, if redundancy or access is expanded without proper controls.
- **Hospital system -- what is the priority?**
  Availability, but never at the cost of patient data confidentiality.

![Real-World Breach Scenario](https://img.shields.io/badge/Real--World%20Breach%20Scenario-c7a485?style=flat)

Ransomware encrypts hospital systems, halting patient care.

![Linux / Windows Follow-Ups](https://img.shields.io/badge/Linux%20%2F%20Windows%20Follow--Ups-f9f2e1?style=flat)

| Linux | Windows |
| --- | --- |
| `uptime` | `tasklist` |
| `df -h` | `Get-Service` |
| `systemctl status` | `wevtutil qe System` |

![Common Mistakes](https://img.shields.io/badge/Common%20Mistakes-c7a485?style=flat)

- Treating CIA as equal in all environments
- Ignoring business impact

---

### Q2. Authentication vs Authorization

![Strong Sample Answer](https://img.shields.io/badge/Strong%20Sample%20Answer-f9f2e1?style=flat)

Authentication verifies identity. Authorization determines access after identity is verified.

> ![Neutral takeaway](https://img.shields.io/badge/Neutral%20takeaway-d7cfc0?style=flat): identity precedes access; least privilege limits impact.

![Pressure Questions + Answers](https://img.shields.io/badge/Pressure%20Questions%20%2B%20Answers-e26a58?style=flat)

- **Can authorization exist without authentication?**
  No -- authorization assumes identity.
- **Where does MFA fit?**
  Authentication.
- **How does least privilege help?**
  Limits blast radius after compromise.

![Real-World Breach Scenario](https://img.shields.io/badge/Real--World%20Breach%20Scenario-c7a485?style=flat)

Compromised credentials grant excessive access due to poor RBAC.

![Linux / Windows Follow-Ups](https://img.shields.io/badge/Linux%20%2F%20Windows%20Follow--Ups-f9f2e1?style=flat)

| Linux | Windows |
| --- | --- |
| `id` | `whoami /groups` |
| `groups` | `Get-LocalGroup` |
| `sudo -l` | `whoami /priv` |

![Common Mistakes](https://img.shields.io/badge/Common%20Mistakes-c7a485?style=flat)

- Using terms interchangeably
- Ignoring access reviews

---

### Q3. What is phishing?

![Strong Sample Answer](https://img.shields.io/badge/Strong%20Sample%20Answer-f9f2e1?style=flat)

Phishing is social engineering designed to trick users into revealing information or executing malicious actions.

> ![Neutral takeaway](https://img.shields.io/badge/Neutral%20takeaway-d7cfc0?style=flat): response is about containment and escalation, not blame.

![Pressure Questions + Answers](https://img.shields.io/badge/Pressure%20Questions%20%2B%20Answers-e26a58?style=flat)

- **User clicked link -- now what?**
  Isolate system, report, preserve evidence.
- **How do you reduce phishing risk?**
  Training, email filtering, MFA.
- **Why is spear phishing harder?**
  Personalization increases trust.

![Real-World Breach Scenario](https://img.shields.io/badge/Real--World%20Breach%20Scenario-c7a485?style=flat)

Business Email Compromise leads to fraudulent wire transfer.

![Linux / Windows Follow-Ups](https://img.shields.io/badge/Linux%20%2F%20Windows%20Follow--Ups-f9f2e1?style=flat)

| Linux | Windows |
| --- | --- |
| `grep mail.log` | `Get-WinEvent -LogName Security` |
| `journalctl` | `Get-MessageTrace` |

![Common Mistakes](https://img.shields.io/badge/Common%20Mistakes-c7a485?style=flat)

- Blaming users
- Failing to escalate quickly

---

## 2. Operating Systems and Networking Basics

### Q4. What happens when you type a URL into a browser?

![Strong Sample Answer](https://img.shields.io/badge/Strong%20Sample%20Answer-f9f2e1?style=flat)

DNS resolution, TCP connection, TLS handshake, HTTP request/response.

> ![Neutral takeaway](https://img.shields.io/badge/Neutral%20takeaway-d7cfc0?style=flat): DNS and transport are as critical as the web request.

![Pressure Questions + Answers](https://img.shields.io/badge/Pressure%20Questions%20%2B%20Answers-e26a58?style=flat)

- **Where can attackers intercept?**
  DNS, network, or TLS downgrade.
- **What fails if DNS is down?**
  Name resolution.
- **Why HTTPS?**
  Encryption and integrity.

![Real-World Breach Scenario](https://img.shields.io/badge/Real--World%20Breach%20Scenario-c7a485?style=flat)

DNS hijacking redirects users to a malicious site.

![Linux / Windows Follow-Ups](https://img.shields.io/badge/Linux%20%2F%20Windows%20Follow--Ups-f9f2e1?style=flat)

| Linux | Windows |
| --- | --- |
| `dig` | `nslookup` |
| `ss -tuln` | `netstat -ano` |

![Common Mistakes](https://img.shields.io/badge/Common%20Mistakes-c7a485?style=flat)

- Skipping DNS
- Treating HTTPS as "just encryption"

---

### Q5. TCP vs UDP

![Strong Sample Answer](https://img.shields.io/badge/Strong%20Sample%20Answer-f9f2e1?style=flat)

TCP is reliable and connection-oriented. UDP is fast and connectionless.

> ![Neutral takeaway](https://img.shields.io/badge/Neutral%20takeaway-d7cfc0?style=flat): security depends on the use case, not the protocol alone.

![Pressure Questions + Answers](https://img.shields.io/badge/Pressure%20Questions%20%2B%20Answers-e26a58?style=flat)

- **Why UDP in amplification attacks?**
  No handshake, spoofable source IPs.
- **Can TCP be abused?**
  Yes -- SYN floods.
- **Is UDP insecure by default?**
  No -- depends on the use case.

![Real-World Breach Scenario](https://img.shields.io/badge/Real--World%20Breach%20Scenario-c7a485?style=flat)

DNS amplification DDoS disrupts public services.

![Linux / Windows Follow-Ups](https://img.shields.io/badge/Linux%20%2F%20Windows%20Follow--Ups-f9f2e1?style=flat)

| Linux | Windows |
| --- | --- |
| `tcpdump` | `netstat -an` |
| `ss -u` | `Get-NetUDPEndpoint` |

![Common Mistakes](https://img.shields.io/badge/Common%20Mistakes-c7a485?style=flat)

- Calling UDP "unsafe"
- Ignoring protocol context

---

### Q6. What is a firewall?

![Strong Sample Answer](https://img.shields.io/badge/Strong%20Sample%20Answer-f9f2e1?style=flat)

A firewall filters traffic based on rules like IP, port, and protocol.

> ![Neutral takeaway](https://img.shields.io/badge/Neutral%20takeaway-d7cfc0?style=flat): firewalls reduce risk, they do not eliminate it.

![Pressure Questions + Answers](https://img.shields.io/badge/Pressure%20Questions%20%2B%20Answers-e26a58?style=flat)

- **What bypasses firewalls?**
  Allowed ports and insider threats.
- **Flat network risk?**
  Easy lateral movement.
- **Host vs network firewall?**
  Local vs perimeter control.

![Real-World Breach Scenario](https://img.shields.io/badge/Real--World%20Breach%20Scenario-c7a485?style=flat)

Attacker pivots laterally after initial compromise.

![Linux / Windows Follow-Ups](https://img.shields.io/badge/Linux%20%2F%20Windows%20Follow--Ups-f9f2e1?style=flat)

| Linux | Windows |
| --- | --- |
| `iptables -L` | `Get-NetFirewallRule` |
| `ufw status` | `Get-NetFirewallProfile` |

![Common Mistakes](https://img.shields.io/badge/Common%20Mistakes-c7a485?style=flat)

- Treating firewalls as full security
- No segmentation

---

## 3. Security Tools and Concepts

### Q7. Antivirus vs EDR vs SIEM

![Strong Sample Answer](https://img.shields.io/badge/Strong%20Sample%20Answer-f9f2e1?style=flat)

Antivirus detects known malware, EDR monitors endpoint behavior, SIEM aggregates and correlates logs.

> ![Neutral takeaway](https://img.shields.io/badge/Neutral%20takeaway-d7cfc0?style=flat): tools support decisions; response and ownership matter most.

![Pressure Questions + Answers](https://img.shields.io/badge/Pressure%20Questions%20%2B%20Answers-e26a58?style=flat)

- **Why won't SIEM stop malware?**
  It detects; it does not block.
- **EDR alert, no response -- then?**
  Alerts are useless without action.
- **Post-incident -- most useful?**
  SIEM.

![Real-World Breach Scenario](https://img.shields.io/badge/Real--World%20Breach%20Scenario-c7a485?style=flat)

EDR detects lateral movement; SIEM correlates domain-wide activity.

![Linux / Windows Follow-Ups](https://img.shields.io/badge/Linux%20%2F%20Windows%20Follow--Ups-f9f2e1?style=flat)

| Linux | Windows |
| --- | --- |
| `ps aux` | `Get-Process` |
| `last` | `Get-WinEvent` |
| `/var/log` | `Get-WinEvent -LogName Security` |

![Common Mistakes](https://img.shields.io/badge/Common%20Mistakes-c7a485?style=flat)

- Treating tools as interchangeable
- No alert ownership

---

### Q8. What are logs and why do they matter?

![Strong Sample Answer](https://img.shields.io/badge/Strong%20Sample%20Answer-f9f2e1?style=flat)

Logs provide visibility, detection, accountability, and forensic evidence.

> ![Neutral takeaway](https://img.shields.io/badge/Neutral%20takeaway-d7cfc0?style=flat): quality and consistency matter more than sheer volume.

![Pressure Questions + Answers](https://img.shields.io/badge/Pressure%20Questions%20%2B%20Answers-e26a58?style=flat)

- **What makes logs unreliable?**
  No NTP, gaps, or tampering.
- **Why time sync matters?**
  Correlation accuracy.
- **Reduce alert fatigue?**
  Tuning and baselining.

![Real-World Breach Scenario](https://img.shields.io/badge/Real--World%20Breach%20Scenario-c7a485?style=flat)

Missing logs delay breach detection.

![Linux / Windows Follow-Ups](https://img.shields.io/badge/Linux%20%2F%20Windows%20Follow--Ups-f9f2e1?style=flat)

| Linux | Windows |
| --- | --- |
| `journalctl` | `w32tm /query /status` |
| `chronyc tracking` | `Get-WinEvent` |

![Common Mistakes](https://img.shields.io/badge/Common%20Mistakes-c7a485?style=flat)

- Logging everything, analyzing nothing

---

## 4. Incident Response

### Q9. Suspected malware -- first step?

![Strong Sample Answer](https://img.shields.io/badge/Strong%20Sample%20Answer-f9f2e1?style=flat)

Isolate the system, preserve evidence, escalate per procedure.

> ![Neutral takeaway](https://img.shields.io/badge/Neutral%20takeaway-d7cfc0?style=flat): containment first, then investigation.

![Pressure Questions + Answers](https://img.shields.io/badge/Pressure%20Questions%20%2B%20Answers-e26a58?style=flat)

- **Who do you notify?**
  SOC or IR lead.
- **When reimage?**
  After investigation.
- **Executive device?**
  Same process, higher urgency.

![Real-World Breach Scenario](https://img.shields.io/badge/Real--World%20Breach%20Scenario-c7a485?style=flat)

Malware spreads due to delayed isolation.

![Linux / Windows Follow-Ups](https://img.shields.io/badge/Linux%20%2F%20Windows%20Follow--Ups-f9f2e1?style=flat)

| Linux | Windows |
| --- | --- |
| `ip link set down` | Disable NIC |
| `ps aux` | `tasklist` |

![Common Mistakes](https://img.shields.io/badge/Common%20Mistakes-c7a485?style=flat)

- Rebooting
- Acting without authorization

---

## Safe Answers When You Don't Know

- "I'd verify by checking logs or documentation."
- "I'd escalate to the appropriate team."
- "I don't have that memorized, but I know where to find it."

---

## Rapid-Fire Drill

- What is least privilege?
- What port is HTTPS?
- Difference between hashing and encryption?
- What does DNS do?
- Why centralize logs?

---

## First 90 Days Mindset

- Learn the environment
- Understand escalation paths
- Master logs before tools
- Ask questions early

---

## Confidence Signals Interviewers Look For

- Calm under pressure
- Clear escalation
- Process over ego
- Business-aware decisions









