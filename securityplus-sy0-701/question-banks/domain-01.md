# Question Bank — Domain 1 (General Security Concepts)

## How to Use
- Answer questions without looking at the answer key.
- Write answers as: `1C 2A 3B ...`
- Review explanations for every missed question.
- Log results in `progress/practice-scores.md`.

---

## Questions

### Q1 — Availability and Attacks

Which part of the CIA triad is primarily impacted by a denial-of-service (DoS) attack?

A) Confidentiality  
B) Integrity  
C) Availability  
D) Authentication  

---

### Q2 — Authentication Factors

A company requires employees to use a smart card AND a PIN to access systems. This is an example of:

A) Multifactor authentication  
B) Single sign-on  
C) Role-based access control  
D) Least privilege  

---

### Q3 — Preventive Controls

Which security control is considered preventive rather than detective?

A) IDS  
B) Firewall  
C) SIEM  
D) Log review  

---

### Q4 — Zero Trust Model

Zero Trust architecture assumes:

A) Internal users are trusted by default  
B) External networks are hostile but internal networks are safe  
C) All access must be continuously verified  
D) Encryption is optional on private networks  

---

### Q5 — Risk Calculation

Which term best describes the combination of likelihood and impact?

A) Threat  
B) Vulnerability  
C) Risk  
D) Exposure  

---

### Q6 — Authorization

Which option BEST describes authorization?

A) Proving who you are  
B) Determining what you can access  
C) Recording actions taken  
D) Encrypting communication  

---

### Q7 — Non-Repudiation

Which control BEST supports non-repudiation?

A) Hashing  
B) Symmetric encryption  
C) Digital signatures  
D) Obfuscation  

---

### Q8 — Least Privilege

A user can access a finance share even though they are not in the Finance group. Which concept is MOST likely being violated?

A) Separation of duties  
B) Least privilege  
C) Tokenization  
D) Password complexity  

---

### Q9 — Compensating Controls

A company installs a badge reader because the door lock cannot be repaired immediately. The badge reader is an example of a:

A) Corrective control  
B) Detective control  
C) Compensating control  
D) Deterrent control  

---

### Q10 — Detective Controls

Which is the BEST example of a detective control?

A) Firewall blocking inbound traffic  
B) Security guard checking IDs  
C) Centralized log monitoring with alerting  
D) Patch management program  

---

### Q11 — Preventive Measures

A security team blocks USB storage devices across endpoints to reduce data theft. This is an example of:

A) Deterrence  
B) Prevention  
C) Recovery  
D) Investigation  

---

### Q12 — Separation of Duties

A company requires two employees to approve wire transfers over $10,000. This is BEST described as:

A) Defense in depth  
B) Separation of duties  
C) Single point of failure  
D) Federation  

---

### Q13 — Defense in Depth

Which statement BEST aligns with defense in depth?

A) Put all controls at the perimeter  
B) Use one strong control to reduce cost  
C) Layer controls so failure of one doesn’t equal compromise  
D) Focus only on administrators  

---

### Q14 — Risk vs Exposure

A vulnerability is rated critical, but the affected system is isolated and unreachable. Which factor MOST reduces real-world risk?

A) Threat actor intent  
B) Attack surface / exposure  
C) Vulnerability severity  
D) Password policy  

---

### Q15 — Zero Trust in Practice

Which scenario BEST reflects a Zero Trust architecture?

A) VPN users are trusted for 8 hours after login  
B) Internal traffic bypasses inspection  
C) Access is continuously evaluated and least privilege enforced  
D) A strong firewall protects internal systems  

---

## Answer Key & Explanations

### Q1
**Correct Answer:** C — Availability  
DoS attacks aim to make services unavailable to legitimate users.

### Q2
**Correct Answer:** A — Multifactor authentication  
Smart card (something you have) + PIN (something you know).

### Q3
**Correct Answer:** B — Firewall  
Firewalls prevent unwanted traffic; IDS and SIEM detect activity.

### Q4
**Correct Answer:** C — All access must be continuously verified  
Zero Trust follows “never trust, always verify.”

### Q5
**Correct Answer:** C — Risk  
Risk is commonly defined as likelihood × impact.

### Q6
**Correct Answer:** B — Determining what you can access  
Authorization defines permissions after authentication.

### Q7
**Correct Answer:** C — Digital signatures  
Digital signatures provide integrity and non-repudiation.

### Q8
**Correct Answer:** B — Least privilege  
Users should only have access required for their role.

### Q9
**Correct Answer:** C — Compensating control  
Used when the ideal control cannot be implemented immediately.

### Q10
**Correct Answer:** C — Centralized log monitoring with alerting  
Detective controls identify and alert on events.

### Q11
**Correct Answer:** B — Prevention  
Blocking USB devices reduces the chance of data exfiltration.

### Q12
**Correct Answer:** B — Separation of duties  
High-risk actions require multiple people.

### Q13
**Correct Answer:** C — Layer controls so failure of one doesn’t equal compromise  
That’s the essence of defense in depth.

### Q14
**Correct Answer:** B — Attack surface / exposure  
If the system isn’t reachable, practical risk is reduced.

### Q15
**Correct Answer:** C — Access is continuously evaluated and least privilege enforced  
Zero Trust removes implicit trust, even internally.
