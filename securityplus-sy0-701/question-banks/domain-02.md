# Question Bank – Domain 2 (Threats, Vulnerabilities, and Mitigations)

## How to Use
- Answer without peeking at the explanations.
- Record responses as `1B 2A 3C ...` to speed up self-grading.
- Review every missed question and log the result in `progress/practice-scores.md`.

---

## Questions

### Q1 – Virus vs. Worm
Which option BEST describes a worm?

A) Requires a user to run an infected file to spread  
B) Self-replicates and spreads across networks without user action  
C) Hides inside a legitimate program but does not replicate  
D) Encrypts files and demands payment

---

### Q2 – Trojan Characteristics
A user installs a “free PDF converter” that looks legitimate but silently installs a backdoor. This is MOST likely:

A) Trojan  
B) Worm  
C) Logic bomb  
D) Rootkit

---

### Q3 – Phishing Recognition
An employee receives an email from “IT Support” stating their account will be disabled unless they log in immediately. This is BEST described as:

A) Tailgating  
B) Phishing  
C) Pretexting  
D) Watering-hole attack

---

### Q4 – Best Mitigation
A company is hit by credential stuffing attacks. Which control MOST directly reduces successful logins with stolen passwords?

A) Network segmentation  
B) Multi-factor authentication (MFA)  
C) Full-disk encryption  
D) Data loss prevention (DLP)

---

### Q5 – Vulnerability vs. Threat
Which statement is MOST accurate?

A) A vulnerability is an attacker targeting a system  
B) A threat is a weakness in software  
C) A vulnerability is a weakness that can be exploited  
D) A threat is the same as risk

---

### Q6 – Ransomware Resilience
Which action MOST improves recovery from ransomware without paying the attacker?

A) Disable all user accounts  
B) Maintain tested offline/immutable backups  
C) Enforce password rotation every week  
D) Block all inbound network traffic

---

### Q7 – Identifying a MitM
Users report being redirected to a fake login page on public Wi-Fi even when typing the correct URL. This is MOST consistent with:

A) Man-in-the-middle (MitM) attack  
B) SQL injection  
C) Cross-site scripting (XSS)  
D) ARP spoofing is impossible on Wi-Fi

---

### Q8 – Patch Priority
A critical vulnerability exists on a public-facing server, and exploit code is available online. What is the BEST next step?

A) Wait for the next maintenance window  
B) Patch immediately or apply compensating controls to reduce exposure  
C) Conduct user awareness training  
D) Disable endpoint antivirus

---

### Q9 – Password Spraying
Logs show many failed logins across numerous accounts, each with only a few attempts using common passwords. This is MOST likely:

A) Brute force  
B) Password spraying  
C) Dictionary attack against one account  
D) Credential stuffing

---

### Q10 – Social Engineering Clue
An attacker calls the help desk, claims to be a new executive, and demands a password reset immediately. This is BEST described as:

A) Pretexting  
B) Spear phishing  
C) Shoulder surfing  
D) Whaling requires email only

---

## Answer Key and Explanations

### Q1
**Answer:** B – Worms self-replicate without user action; viruses usually need a user to run something.

### Q2
**Answer:** A – Trojans appear legitimate but perform malicious actions such as installing backdoors.

### Q3
**Answer:** B – Classic phishing uses urgency and fake login pages to steal credentials.

### Q4
**Answer:** B – MFA stops most credential stuffing because stolen passwords alone are insufficient.

### Q5
**Answer:** C – A vulnerability is a weakness. Threats exploit weaknesses; risk combines likelihood and impact.

### Q6
**Answer:** B – Tested offline/immutable backups enable recovery without paying ransom.

### Q7
**Answer:** A – Symptoms point to interception/redirection, which is a MitM attack.

### Q8
**Answer:** B – Public-facing + known exploit = patch now or deploy compensating controls immediately.

### Q9
**Answer:** B – Password spraying uses a few common passwords across many accounts to avoid lockouts.

### Q10
**Answer:** A – Urgency plus a fabricated identity is classic pretexting.
