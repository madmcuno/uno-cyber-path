# Domain 2 - Threats, Vulnerabilities, and Mitigations

> Connect the attack surface, the adversary's tooling, and the controls that shut it down.

## How to Use This File
- Summarize each topic in your own words so you can teach it back in under 30 seconds.
- Focus on what happens, why it works, and which mitigation maps directly to the scenario.
- Pair this sheet with `question-banks/domain-02.md` to pressure-test recall.

---

## Concepts You Must Understand

### Malware vs. Attack Technique
**What it is** - Malware is the malicious software (payload); the attack technique is how it is delivered or executed.  
**Why it matters** - Exam questions love mixing these terms (phishing is not malware).  
**How it shows up** - Scenarios describe symptoms; you identify the malware type *and* the best countermeasure.

Common mix-ups:
- Calling phishing or vishing "malware."
- Confusing how malware spreads (virus vs. worm) versus how it hides (trojan, rootkit).

### Social Engineering
**What it is** - Manipulating people into giving access, information, or actions.  
**Why it matters** - Humans are often the weakest control.  
**Exam signals** - Urgency, authority, curiosity, or fear cues; impersonation, pretexting, tailgating.

Common mistakes:
- Choosing a technical control when the question wants training or process controls.
- Ignoring emotional triggers embedded in the prompt.

### Vulnerabilities vs. Exposure
**What it is** - Vulnerability = weakness; exposure = can an attacker realistically reach it.  
**Why it matters** - A critical CVSS score does not equal critical risk if the system is isolated.  
**Exam signals** - Clues like "internet-facing," "default credentials," "isolated network," "no patching."

Common mistakes:
- Ranking severity purely by CVSS without considering likelihood.  
- Forgetting that compensating controls can reduce exposure even when the vulnerability remains.

---

## Things That Break, Get Abused, or Go Wrong

### Phishing (and Variants)
- **What happens** - Attackers send persuasive messages to make targets click, pay, or share credentials.
- **Why it works** - Exploits trust plus urgency or fear; spoofed domains and look-alike branding help.
- **Mitigation focus** - Security awareness, sender verification, MFA, email filtering, out-of-band confirmation.

### Ransomware
- **What happens** - Files or systems are encrypted, often with data theft, and payment is demanded.
- **Why it works** - Relies on unpatched systems, macros, excessive privileges, weak segmentation, bad backups.
- **Mitigation focus** - Offline/immutable backups, least privilege, patching, app allow-listing, segmentation, EDR.

### Password Attacks
- **What happens** - Guessing (brute force), spraying, stuffing leaked credentials, cracking offline hashes.
- **Why it works** - Password reuse, weak complexity, exposed credential dumps, lack of monitoring.
- **Mitigation focus** - MFA, password managers, account lockouts or throttling, anomaly detection, salted hashing.

---

## Exam Reality Notes
- If the stem says "BEST mitigation," pick the control that most directly reduces the described risk.
- Human-driven scenarios usually reward policy, process, or training answers over pure tech.
- Internet-facing unpatched assets shout "patch/segment first," not "run another awareness campaign."

---

## Key Takeaways
- Identify the attack type before selecting the mitigation; control families map to specific threats.
- Severity is not risk without exposure and likelihood.
- Social engineering questions are about emotion and process failure, not just technology.
