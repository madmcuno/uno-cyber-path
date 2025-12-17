# Domain 1 - General Security Concepts

> Build fluency with the core terminology every other Security+ domain relies on.

## How to Use This File
- Treat this as a high-signal summary and replace the prompts with your own shorthand.
- Focus on intent: why a control exists, how it fails, and when the exam expects you to apply it.
- Pair with the Domain 1 question bank to validate recall under pressure.

---

## Core Security Principles

### CIA Triad
**Confidentiality**  
Protects data from unauthorized disclosure.  
Typical controls: encryption, access control, data classification.

**Integrity**  
Guards against unauthorized modification or corruption.  
Typical controls: hashing, digital signatures, checksums.

**Availability**  
Ensures data and systems are accessible when needed.  
Typical controls: redundancy, backups, fault tolerance, anti-DDoS.

> Exam angle: DoS/DDoS questions almost always target availability.

### AAA Framework
**Authentication** - Proves identity (passwords, smart cards, biometrics).  
**Authorization** - Grants permissions (RBAC, ACLs, ABAC).  
**Accounting** - Tracks activity (logs, audit trails, session captures).

> Exam angle: Watch for scenarios where candidates confuse "who are you?" (authentication) with "what can you touch?" (authorization).

---

## Security Concepts and Models

### Least Privilege
Give people, processes, and systems only the access required for their tasks.  
Benefits: smaller blast radius, limited lateral movement, lower insider risk.

### Defense in Depth
Layer technical, administrative, and physical controls so that one failure does not equal compromise.  
Think "firewall + MFA + monitoring" rather than a single silver bullet.

### Zero Trust
Assumes no implicit trust even inside the perimeter.  
Principles: continuous verification, least privilege, segmentation, strong identity controls.  
Mantra: "Never trust, always verify."

---

## Security Controls

### Control Categories
- **Administrative** - Policies, procedures, training, background checks.
- **Technical** - Firewalls, IDS/IPS, encryption, authentication systems.
- **Physical** - Locks, guards, cameras, badge readers.

### Control Functions
- **Preventive** - Stop incidents before they occur (firewalls, MFA, access control).
- **Detective** - Identify incidents in progress or post-incident (IDS, SIEM, logs).
- **Corrective** - Remediate after detection (patching, reimaging, backups).
- **Compensating** - Alternate controls when the preferred option is unavailable (guards while the badge reader is offline).

> Exam angle: If the prompt says "temporary workaround," think compensating control.

---

## Risk Concepts
**Threat** - Anything capable of exploiting a vulnerability.  
**Vulnerability** - A weakness that could be exploited.  
**Risk** - Likelihood and impact of a threat exploiting a vulnerability.  
**Impact** - The consequence if exploitation succeeds.  
**Likelihood** - The chance the exploit occurs.

Quick reminders:
- A critical vulnerability is not automatically a critical risk if exposure is low.
- Risk responses include acceptance, avoidance, mitigation, and transference.
- Combine qualitative (high/medium/low) and quantitative ($$) analysis to prioritize fixes.
