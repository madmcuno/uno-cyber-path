# Entry-Level Cybersecurity Mock Interview (v2)

Purpose: prepare for entry-level cybersecurity interviews by demonstrating clear thinking under pressure, real-world awareness, and basic operational capability.

---

## 1. Cybersecurity Fundamentals

### Q1. What is the CIA triad?

![Strong Sample Answer](https://img.shields.io/badge/Strong%20Sample%20Answer-f6efdf?style=flat-square)

Confidentiality prevents unauthorized access, integrity prevents unauthorized modification, and availability ensures systems remain accessible when needed.

> ![Neutral takeaway](https://img.shields.io/badge/Neutral%20takeaway-f0e2c0?style=flat-square): the priority can shift by environment and business impact.

![Pressure Questions + Answers](https://img.shields.io/badge/Pressure%20Questions%20%2B%20Answers-f0e2c0?style=flat-square)

- **Which is most impacted by ransomware?**
  Availability first, then integrity.
- **Can improving availability reduce confidentiality?**
  Yes, if redundancy or access is expanded without proper controls.
- **Hospital system -- what is the priority?**
  Availability, but never at the cost of patient data confidentiality.

![Real-World Breach Scenario](https://img.shields.io/badge/Real--World%20Breach%20Scenario-e7d2c3?style=flat-square)

Ransomware encrypts hospital systems, halting patient care.

![Linux / Windows Follow-Ups](https://img.shields.io/badge/Linux%20%2F%20Windows%20Follow--Ups-f6efdf?style=flat-square)

| Linux | Windows |
| --- | --- |
| `uptime` | `tasklist` |
| `df -h` | `Get-Service` |
| `systemctl status` | `wevtutil qe System` |

![Common Mistakes](https://img.shields.io/badge/Common%20Mistakes-e7d2c3?style=flat-square)

- Treating CIA as equal in all environments
- Ignoring business impact

---

### Q2. Authentication vs Authorization

![Strong Sample Answer](https://img.shields.io/badge/Strong%20Sample%20Answer-f6efdf?style=flat-square)

Authentication verifies identity. Authorization determines access after identity is verified.

> ![Neutral takeaway](https://img.shields.io/badge/Neutral%20takeaway-f0e2c0?style=flat-square): identity precedes access; least privilege limits impact.

![Pressure Questions + Answers](https://img.shields.io/badge/Pressure%20Questions%20%2B%20Answers-f0e2c0?style=flat-square)

- **Can authorization exist without authentication?**
  No -- authorization assumes identity.
- **Where does MFA fit?**
  Authentication.
- **How does least privilege help?**
  Limits blast radius after compromise.

![Real-World Breach Scenario](https://img.shields.io/badge/Real--World%20Breach%20Scenario-e7d2c3?style=flat-square)

Compromised credentials grant excessive access due to poor RBAC.

![Linux / Windows Follow-Ups](https://img.shields.io/badge/Linux%20%2F%20Windows%20Follow--Ups-f6efdf?style=flat-square)

| Linux | Windows |
| --- | --- |
| `id` | `whoami /groups` |
| `groups` | `Get-LocalGroup` |
| `sudo -l` | `whoami /priv` |

![Common Mistakes](https://img.shields.io/badge/Common%20Mistakes-e7d2c3?style=flat-square)

- Using terms interchangeably
- Ignoring access reviews

---

### Q3. What is phishing?

![Strong Sample Answer](https://img.shields.io/badge/Strong%20Sample%20Answer-f6efdf?style=flat-square)

Phishing is social engineering designed to trick users into revealing information or executing malicious actions.

> ![Neutral takeaway](https://img.shields.io/badge/Neutral%20takeaway-f0e2c0?style=flat-square): response is about containment and escalation, not blame.

![Pressure Questions + Answers](https://img.shields.io/badge/Pressure%20Questions%20%2B%20Answers-f0e2c0?style=flat-square)

- **User clicked link -- now what?**
  Isolate system, report, preserve evidence.
- **How do you reduce phishing risk?**
  Training, email filtering, MFA.
- **Why is spear phishing harder?**
  Personalization increases trust.

![Real-World Breach Scenario](https://img.shields.io/badge/Real--World%20Breach%20Scenario-e7d2c3?style=flat-square)

Business Email Compromise leads to fraudulent wire transfer.

![Linux / Windows Follow-Ups](https://img.shields.io/badge/Linux%20%2F%20Windows%20Follow--Ups-f6efdf?style=flat-square)

| Linux | Windows |
| --- | --- |
| `grep mail.log` | `Get-WinEvent -LogName Security` |
| `journalctl` | `Get-MessageTrace` |

![Common Mistakes](https://img.shields.io/badge/Common%20Mistakes-e7d2c3?style=flat-square)

- Blaming users
- Failing to escalate quickly

---

## 2. Operating Systems and Networking Basics

### Q4. What happens when you type a URL into a browser?

![Strong Sample Answer](https://img.shields.io/badge/Strong%20Sample%20Answer-f6efdf?style=flat-square)

DNS resolution, TCP connection, TLS handshake, HTTP request/response.

> ![Neutral takeaway](https://img.shields.io/badge/Neutral%20takeaway-f0e2c0?style=flat-square): DNS and transport are as critical as the web request.

![Pressure Questions + Answers](https://img.shields.io/badge/Pressure%20Questions%20%2B%20Answers-f0e2c0?style=flat-square)

- **Where can attackers intercept?**
  DNS, network, or TLS downgrade.
- **What fails if DNS is down?**
  Name resolution.
- **Why HTTPS?**
  Encryption and integrity.

![Real-World Breach Scenario](https://img.shields.io/badge/Real--World%20Breach%20Scenario-e7d2c3?style=flat-square)

DNS hijacking redirects users to a malicious site.

![Linux / Windows Follow-Ups](https://img.shields.io/badge/Linux%20%2F%20Windows%20Follow--Ups-f6efdf?style=flat-square)

| Linux | Windows |
| --- | --- |
| `dig` | `nslookup` |
| `ss -tuln` | `netstat -ano` |

![Common Mistakes](https://img.shields.io/badge/Common%20Mistakes-e7d2c3?style=flat-square)

- Skipping DNS
- Treating HTTPS as "just encryption"

---

### Q5. TCP vs UDP

![Strong Sample Answer](https://img.shields.io/badge/Strong%20Sample%20Answer-f6efdf?style=flat-square)

TCP is reliable and connection-oriented. UDP is fast and connectionless.

> ![Neutral takeaway](https://img.shields.io/badge/Neutral%20takeaway-f0e2c0?style=flat-square): security depends on the use case, not the protocol alone.

![Pressure Questions + Answers](https://img.shields.io/badge/Pressure%20Questions%20%2B%20Answers-f0e2c0?style=flat-square)

- **Why UDP in amplification attacks?**
  No handshake, spoofable source IPs.
- **Can TCP be abused?**
  Yes -- SYN floods.
- **Is UDP insecure by default?**
  No -- depends on the use case.

![Real-World Breach Scenario](https://img.shields.io/badge/Real--World%20Breach%20Scenario-e7d2c3?style=flat-square)

DNS amplification DDoS disrupts public services.

![Linux / Windows Follow-Ups](https://img.shields.io/badge/Linux%20%2F%20Windows%20Follow--Ups-f6efdf?style=flat-square)

| Linux | Windows |
| --- | --- |
| `tcpdump` | `netstat -an` |
| `ss -u` | `Get-NetUDPEndpoint` |

![Common Mistakes](https://img.shields.io/badge/Common%20Mistakes-e7d2c3?style=flat-square)

- Calling UDP "unsafe"
- Ignoring protocol context

---

### Q6. What is a firewall?

![Strong Sample Answer](https://img.shields.io/badge/Strong%20Sample%20Answer-f6efdf?style=flat-square)

A firewall filters traffic based on rules like IP, port, and protocol.

> ![Neutral takeaway](https://img.shields.io/badge/Neutral%20takeaway-f0e2c0?style=flat-square): firewalls reduce risk, they do not eliminate it.

![Pressure Questions + Answers](https://img.shields.io/badge/Pressure%20Questions%20%2B%20Answers-f0e2c0?style=flat-square)

- **What bypasses firewalls?**
  Allowed ports and insider threats.
- **Flat network risk?**
  Easy lateral movement.
- **Host vs network firewall?**
  Local vs perimeter control.

![Real-World Breach Scenario](https://img.shields.io/badge/Real--World%20Breach%20Scenario-e7d2c3?style=flat-square)

Attacker pivots laterally after initial compromise.

![Linux / Windows Follow-Ups](https://img.shields.io/badge/Linux%20%2F%20Windows%20Follow--Ups-f6efdf?style=flat-square)

| Linux | Windows |
| --- | --- |
| `iptables -L` | `Get-NetFirewallRule` |
| `ufw status` | `Get-NetFirewallProfile` |

![Common Mistakes](https://img.shields.io/badge/Common%20Mistakes-e7d2c3?style=flat-square)

- Treating firewalls as full security
- No segmentation

---

## 3. Security Tools and Concepts

### Q7. Antivirus vs EDR vs SIEM

![Strong Sample Answer](https://img.shields.io/badge/Strong%20Sample%20Answer-f6efdf?style=flat-square)

Antivirus detects known malware, EDR monitors endpoint behavior, SIEM aggregates and correlates logs.

> ![Neutral takeaway](https://img.shields.io/badge/Neutral%20takeaway-f0e2c0?style=flat-square): tools support decisions; response and ownership matter most.

![Pressure Questions + Answers](https://img.shields.io/badge/Pressure%20Questions%20%2B%20Answers-f0e2c0?style=flat-square)

- **Why won't SIEM stop malware?**
  It detects; it does not block.
- **EDR alert, no response -- then?**
  Alerts are useless without action.
- **Post-incident -- most useful?**
  SIEM.

![Real-World Breach Scenario](https://img.shields.io/badge/Real--World%20Breach%20Scenario-e7d2c3?style=flat-square)

EDR detects lateral movement; SIEM correlates domain-wide activity.

![Linux / Windows Follow-Ups](https://img.shields.io/badge/Linux%20%2F%20Windows%20Follow--Ups-f6efdf?style=flat-square)

| Linux | Windows |
| --- | --- |
| `ps aux` | `Get-Process` |
| `last` | `Get-WinEvent` |
| `/var/log` | `Get-WinEvent -LogName Security` |

![Common Mistakes](https://img.shields.io/badge/Common%20Mistakes-e7d2c3?style=flat-square)

- Treating tools as interchangeable
- No alert ownership

---

### Q8. What are logs and why do they matter?

![Strong Sample Answer](https://img.shields.io/badge/Strong%20Sample%20Answer-f6efdf?style=flat-square)

Logs provide visibility, detection, accountability, and forensic evidence.

> ![Neutral takeaway](https://img.shields.io/badge/Neutral%20takeaway-f0e2c0?style=flat-square): quality and consistency matter more than sheer volume.

![Pressure Questions + Answers](https://img.shields.io/badge/Pressure%20Questions%20%2B%20Answers-f0e2c0?style=flat-square)

- **What makes logs unreliable?**
  No NTP, gaps, or tampering.
- **Why time sync matters?**
  Correlation accuracy.
- **Reduce alert fatigue?**
  Tuning and baselining.

![Real-World Breach Scenario](https://img.shields.io/badge/Real--World%20Breach%20Scenario-e7d2c3?style=flat-square)

Missing logs delay breach detection.

![Linux / Windows Follow-Ups](https://img.shields.io/badge/Linux%20%2F%20Windows%20Follow--Ups-f6efdf?style=flat-square)

| Linux | Windows |
| --- | --- |
| `journalctl` | `w32tm /query /status` |
| `chronyc tracking` | `Get-WinEvent` |

![Common Mistakes](https://img.shields.io/badge/Common%20Mistakes-e7d2c3?style=flat-square)

- Logging everything, analyzing nothing

---

## 4. Incident Response

### Q9. Suspected malware -- first step?

![Strong Sample Answer](https://img.shields.io/badge/Strong%20Sample%20Answer-f6efdf?style=flat-square)

Isolate the system, preserve evidence, escalate per procedure.

> ![Neutral takeaway](https://img.shields.io/badge/Neutral%20takeaway-f0e2c0?style=flat-square): containment first, then investigation.

![Pressure Questions + Answers](https://img.shields.io/badge/Pressure%20Questions%20%2B%20Answers-f0e2c0?style=flat-square)

- **Who do you notify?**
  SOC or IR lead.
- **When reimage?**
  After investigation.
- **Executive device?**
  Same process, higher urgency.

![Real-World Breach Scenario](https://img.shields.io/badge/Real--World%20Breach%20Scenario-e7d2c3?style=flat-square)

Malware spreads due to delayed isolation.

![Linux / Windows Follow-Ups](https://img.shields.io/badge/Linux%20%2F%20Windows%20Follow--Ups-f6efdf?style=flat-square)

| Linux | Windows |
| --- | --- |
| `ip link set down` | Disable NIC |
| `ps aux` | `tasklist` |

![Common Mistakes](https://img.shields.io/badge/Common%20Mistakes-e7d2c3?style=flat-square)

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




