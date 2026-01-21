# Entry-Level Cybersecurity Mock Interview (v2)

Purpose: prepare for entry-level cybersecurity interviews by demonstrating clear thinking under pressure, real-world awareness, and basic operational capability.

---

## 1. Cybersecurity Fundamentals

### Q1. What is the CIA triad?

<code style="background-color:#f6efdf;color:#6a5b47;padding:0.1em 0.35em;border-radius:0.35em;">Strong Sample Answer</code>

Confidentiality prevents unauthorized access, integrity prevents unauthorized modification, and availability ensures systems remain accessible when needed.

> <code style="background-color:#f0e2c0;color:#6b553a;padding:0.1em 0.35em;border-radius:0.35em;">Neutral takeaway</code>: the priority can shift by environment and business impact.

<code style="background-color:#f0e2c0;color:#6b553a;padding:0.1em 0.35em;border-radius:0.35em;">Pressure Questions + Answers</code>

- **Which is most impacted by ransomware?**
  Availability first, then integrity.
- **Can improving availability reduce confidentiality?**
  Yes, if redundancy or access is expanded without proper controls.
- **Hospital system -- what is the priority?**
  Availability, but never at the cost of patient data confidentiality.

<code style="background-color:#e7d2c3;color:#5a3e2b;padding:0.1em 0.35em;border-radius:0.35em;">Real-World Breach Scenario</code>

Ransomware encrypts hospital systems, halting patient care.

<code style="background-color:#f6efdf;color:#6a5b47;padding:0.1em 0.35em;border-radius:0.35em;">Linux / Windows Follow-Ups</code>

| Linux | Windows |
| --- | --- |
| `uptime` | `tasklist` |
| `df -h` | `Get-Service` |
| `systemctl status` | `wevtutil qe System` |

<code style="background-color:#e7d2c3;color:#5a3e2b;padding:0.1em 0.35em;border-radius:0.35em;">Common Mistakes</code>

- Treating CIA as equal in all environments
- Ignoring business impact

---

### Q2. Authentication vs Authorization

<code style="background-color:#f6efdf;color:#6a5b47;padding:0.1em 0.35em;border-radius:0.35em;">Strong Sample Answer</code>

Authentication verifies identity. Authorization determines access after identity is verified.

> <code style="background-color:#f0e2c0;color:#6b553a;padding:0.1em 0.35em;border-radius:0.35em;">Neutral takeaway</code>: identity precedes access; least privilege limits impact.

<code style="background-color:#f0e2c0;color:#6b553a;padding:0.1em 0.35em;border-radius:0.35em;">Pressure Questions + Answers</code>

- **Can authorization exist without authentication?**
  No -- authorization assumes identity.
- **Where does MFA fit?**
  Authentication.
- **How does least privilege help?**
  Limits blast radius after compromise.

<code style="background-color:#e7d2c3;color:#5a3e2b;padding:0.1em 0.35em;border-radius:0.35em;">Real-World Breach Scenario</code>

Compromised credentials grant excessive access due to poor RBAC.

<code style="background-color:#f6efdf;color:#6a5b47;padding:0.1em 0.35em;border-radius:0.35em;">Linux / Windows Follow-Ups</code>

| Linux | Windows |
| --- | --- |
| `id` | `whoami /groups` |
| `groups` | `Get-LocalGroup` |
| `sudo -l` | `whoami /priv` |

<code style="background-color:#e7d2c3;color:#5a3e2b;padding:0.1em 0.35em;border-radius:0.35em;">Common Mistakes</code>

- Using terms interchangeably
- Ignoring access reviews

---

### Q3. What is phishing?

<code style="background-color:#f6efdf;color:#6a5b47;padding:0.1em 0.35em;border-radius:0.35em;">Strong Sample Answer</code>

Phishing is social engineering designed to trick users into revealing information or executing malicious actions.

> <code style="background-color:#f0e2c0;color:#6b553a;padding:0.1em 0.35em;border-radius:0.35em;">Neutral takeaway</code>: response is about containment and escalation, not blame.

<code style="background-color:#f0e2c0;color:#6b553a;padding:0.1em 0.35em;border-radius:0.35em;">Pressure Questions + Answers</code>

- **User clicked link -- now what?**
  Isolate system, report, preserve evidence.
- **How do you reduce phishing risk?**
  Training, email filtering, MFA.
- **Why is spear phishing harder?**
  Personalization increases trust.

<code style="background-color:#e7d2c3;color:#5a3e2b;padding:0.1em 0.35em;border-radius:0.35em;">Real-World Breach Scenario</code>

Business Email Compromise leads to fraudulent wire transfer.

<code style="background-color:#f6efdf;color:#6a5b47;padding:0.1em 0.35em;border-radius:0.35em;">Linux / Windows Follow-Ups</code>

| Linux | Windows |
| --- | --- |
| `grep mail.log` | `Get-WinEvent -LogName Security` |
| `journalctl` | `Get-MessageTrace` |

<code style="background-color:#e7d2c3;color:#5a3e2b;padding:0.1em 0.35em;border-radius:0.35em;">Common Mistakes</code>

- Blaming users
- Failing to escalate quickly

---

## 2. Operating Systems and Networking Basics

### Q4. What happens when you type a URL into a browser?

<code style="background-color:#f6efdf;color:#6a5b47;padding:0.1em 0.35em;border-radius:0.35em;">Strong Sample Answer</code>

DNS resolution, TCP connection, TLS handshake, HTTP request/response.

> <code style="background-color:#f0e2c0;color:#6b553a;padding:0.1em 0.35em;border-radius:0.35em;">Neutral takeaway</code>: DNS and transport are as critical as the web request.

<code style="background-color:#f0e2c0;color:#6b553a;padding:0.1em 0.35em;border-radius:0.35em;">Pressure Questions + Answers</code>

- **Where can attackers intercept?**
  DNS, network, or TLS downgrade.
- **What fails if DNS is down?**
  Name resolution.
- **Why HTTPS?**
  Encryption and integrity.

<code style="background-color:#e7d2c3;color:#5a3e2b;padding:0.1em 0.35em;border-radius:0.35em;">Real-World Breach Scenario</code>

DNS hijacking redirects users to a malicious site.

<code style="background-color:#f6efdf;color:#6a5b47;padding:0.1em 0.35em;border-radius:0.35em;">Linux / Windows Follow-Ups</code>

| Linux | Windows |
| --- | --- |
| `dig` | `nslookup` |
| `ss -tuln` | `netstat -ano` |

<code style="background-color:#e7d2c3;color:#5a3e2b;padding:0.1em 0.35em;border-radius:0.35em;">Common Mistakes</code>

- Skipping DNS
- Treating HTTPS as "just encryption"

---

### Q5. TCP vs UDP

<code style="background-color:#f6efdf;color:#6a5b47;padding:0.1em 0.35em;border-radius:0.35em;">Strong Sample Answer</code>

TCP is reliable and connection-oriented. UDP is fast and connectionless.

> <code style="background-color:#f0e2c0;color:#6b553a;padding:0.1em 0.35em;border-radius:0.35em;">Neutral takeaway</code>: security depends on the use case, not the protocol alone.

<code style="background-color:#f0e2c0;color:#6b553a;padding:0.1em 0.35em;border-radius:0.35em;">Pressure Questions + Answers</code>

- **Why UDP in amplification attacks?**
  No handshake, spoofable source IPs.
- **Can TCP be abused?**
  Yes -- SYN floods.
- **Is UDP insecure by default?**
  No -- depends on the use case.

<code style="background-color:#e7d2c3;color:#5a3e2b;padding:0.1em 0.35em;border-radius:0.35em;">Real-World Breach Scenario</code>

DNS amplification DDoS disrupts public services.

<code style="background-color:#f6efdf;color:#6a5b47;padding:0.1em 0.35em;border-radius:0.35em;">Linux / Windows Follow-Ups</code>

| Linux | Windows |
| --- | --- |
| `tcpdump` | `netstat -an` |
| `ss -u` | `Get-NetUDPEndpoint` |

<code style="background-color:#e7d2c3;color:#5a3e2b;padding:0.1em 0.35em;border-radius:0.35em;">Common Mistakes</code>

- Calling UDP "unsafe"
- Ignoring protocol context

---

### Q6. What is a firewall?

<code style="background-color:#f6efdf;color:#6a5b47;padding:0.1em 0.35em;border-radius:0.35em;">Strong Sample Answer</code>

A firewall filters traffic based on rules like IP, port, and protocol.

> <code style="background-color:#f0e2c0;color:#6b553a;padding:0.1em 0.35em;border-radius:0.35em;">Neutral takeaway</code>: firewalls reduce risk, they do not eliminate it.

<code style="background-color:#f0e2c0;color:#6b553a;padding:0.1em 0.35em;border-radius:0.35em;">Pressure Questions + Answers</code>

- **What bypasses firewalls?**
  Allowed ports and insider threats.
- **Flat network risk?**
  Easy lateral movement.
- **Host vs network firewall?**
  Local vs perimeter control.

<code style="background-color:#e7d2c3;color:#5a3e2b;padding:0.1em 0.35em;border-radius:0.35em;">Real-World Breach Scenario</code>

Attacker pivots laterally after initial compromise.

<code style="background-color:#f6efdf;color:#6a5b47;padding:0.1em 0.35em;border-radius:0.35em;">Linux / Windows Follow-Ups</code>

| Linux | Windows |
| --- | --- |
| `iptables -L` | `Get-NetFirewallRule` |
| `ufw status` | `Get-NetFirewallProfile` |

<code style="background-color:#e7d2c3;color:#5a3e2b;padding:0.1em 0.35em;border-radius:0.35em;">Common Mistakes</code>

- Treating firewalls as full security
- No segmentation

---

## 3. Security Tools and Concepts

### Q7. Antivirus vs EDR vs SIEM

<code style="background-color:#f6efdf;color:#6a5b47;padding:0.1em 0.35em;border-radius:0.35em;">Strong Sample Answer</code>

Antivirus detects known malware, EDR monitors endpoint behavior, SIEM aggregates and correlates logs.

> <code style="background-color:#f0e2c0;color:#6b553a;padding:0.1em 0.35em;border-radius:0.35em;">Neutral takeaway</code>: tools support decisions; response and ownership matter most.

<code style="background-color:#f0e2c0;color:#6b553a;padding:0.1em 0.35em;border-radius:0.35em;">Pressure Questions + Answers</code>

- **Why won't SIEM stop malware?**
  It detects; it does not block.
- **EDR alert, no response -- then?**
  Alerts are useless without action.
- **Post-incident -- most useful?**
  SIEM.

<code style="background-color:#e7d2c3;color:#5a3e2b;padding:0.1em 0.35em;border-radius:0.35em;">Real-World Breach Scenario</code>

EDR detects lateral movement; SIEM correlates domain-wide activity.

<code style="background-color:#f6efdf;color:#6a5b47;padding:0.1em 0.35em;border-radius:0.35em;">Linux / Windows Follow-Ups</code>

| Linux | Windows |
| --- | --- |
| `ps aux` | `Get-Process` |
| `last` | `Get-WinEvent` |
| `/var/log` | `Get-WinEvent -LogName Security` |

<code style="background-color:#e7d2c3;color:#5a3e2b;padding:0.1em 0.35em;border-radius:0.35em;">Common Mistakes</code>

- Treating tools as interchangeable
- No alert ownership

---

### Q8. What are logs and why do they matter?

<code style="background-color:#f6efdf;color:#6a5b47;padding:0.1em 0.35em;border-radius:0.35em;">Strong Sample Answer</code>

Logs provide visibility, detection, accountability, and forensic evidence.

> <code style="background-color:#f0e2c0;color:#6b553a;padding:0.1em 0.35em;border-radius:0.35em;">Neutral takeaway</code>: quality and consistency matter more than sheer volume.

<code style="background-color:#f0e2c0;color:#6b553a;padding:0.1em 0.35em;border-radius:0.35em;">Pressure Questions + Answers</code>

- **What makes logs unreliable?**
  No NTP, gaps, or tampering.
- **Why time sync matters?**
  Correlation accuracy.
- **Reduce alert fatigue?**
  Tuning and baselining.

<code style="background-color:#e7d2c3;color:#5a3e2b;padding:0.1em 0.35em;border-radius:0.35em;">Real-World Breach Scenario</code>

Missing logs delay breach detection.

<code style="background-color:#f6efdf;color:#6a5b47;padding:0.1em 0.35em;border-radius:0.35em;">Linux / Windows Follow-Ups</code>

| Linux | Windows |
| --- | --- |
| `journalctl` | `w32tm /query /status` |
| `chronyc tracking` | `Get-WinEvent` |

<code style="background-color:#e7d2c3;color:#5a3e2b;padding:0.1em 0.35em;border-radius:0.35em;">Common Mistakes</code>

- Logging everything, analyzing nothing

---

## 4. Incident Response

### Q9. Suspected malware -- first step?

<code style="background-color:#f6efdf;color:#6a5b47;padding:0.1em 0.35em;border-radius:0.35em;">Strong Sample Answer</code>

Isolate the system, preserve evidence, escalate per procedure.

> <code style="background-color:#f0e2c0;color:#6b553a;padding:0.1em 0.35em;border-radius:0.35em;">Neutral takeaway</code>: containment first, then investigation.

<code style="background-color:#f0e2c0;color:#6b553a;padding:0.1em 0.35em;border-radius:0.35em;">Pressure Questions + Answers</code>

- **Who do you notify?**
  SOC or IR lead.
- **When reimage?**
  After investigation.
- **Executive device?**
  Same process, higher urgency.

<code style="background-color:#e7d2c3;color:#5a3e2b;padding:0.1em 0.35em;border-radius:0.35em;">Real-World Breach Scenario</code>

Malware spreads due to delayed isolation.

<code style="background-color:#f6efdf;color:#6a5b47;padding:0.1em 0.35em;border-radius:0.35em;">Linux / Windows Follow-Ups</code>

| Linux | Windows |
| --- | --- |
| `ip link set down` | Disable NIC |
| `ps aux` | `tasklist` |

<code style="background-color:#e7d2c3;color:#5a3e2b;padding:0.1em 0.35em;border-radius:0.35em;">Common Mistakes</code>

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



