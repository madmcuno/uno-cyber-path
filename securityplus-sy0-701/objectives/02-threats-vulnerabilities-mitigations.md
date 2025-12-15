\# Domain 2 — Threats, Vulnerabilities, and Mitigations



\## How to Use

\- Write short explanations you can say out loud.

\- Focus on: what happens, why it works, how to reduce it.

\- Pair with `question-banks/domain-02.md`.



---



\## Concepts You Must Understand



\### Malware vs “Attack Technique”

What it is:  

Malware is malicious software (the tool). An attack technique is how it gets used (the method).



Why it matters:  

Questions often mix the two. “Phishing” is not malware; it’s a delivery method.



How it shows up on the exam:  

You’ll get a scenario and must identify the most likely malware type or the best mitigation.



Common mistakes:

\- Calling phishing “malware”

\- Confusing “virus/worm/trojan” (how it spreads vs how it hides)



---



\### Social Engineering

What it is:  

Tricking humans into giving access, secrets, or actions.



Why it matters:  

Humans are the soft, squishy attack surface.



How it shows up on the exam:  

You’ll see urgency, authority, fear, or “helpfulness” being exploited.



Common mistakes:

\- Missing the emotional manipulation cues

\- Picking a technical control when the question wants a people/process control



---



\### Vulnerabilities and Exposure

What it is:  

A vulnerability is a weakness. Exposure is whether an attacker can realistically reach and use it.



Why it matters:  

“Critical vulnerability” doesn’t always equal “critical risk” if exposure is low.



How it shows up on the exam:  

The scenario includes clues like “internet-facing,” “isolated network,” “no patching,” or “default creds.”



Common mistakes:

\- Treating severity score as the only factor

\- Ignoring reachability/attack surface



---



\## Things That Break, Get Abused, or Go Wrong



\### Phishing (and look-alikes)

\- What happens: attacker uses messages to trick a user into clicking, paying, or sharing info.

\- Why it works: it targets trust + urgency.

\- How it’s usually mitigated: user training, email filtering, MFA, and verification procedures.



---



\### Ransomware

\- What happens: files get encrypted, access is blocked, payment demanded.

\- Why it works: unpatched systems, bad backups, over-permissioned accounts, macro abuse.

\- How it’s usually mitigated: offline/immutable backups, patching, least privilege, app allow-listing, segmentation.



---



\### Password Attacks

\- What happens: guessing, spraying, stuffing, cracking.

\- Why it works: reused passwords, weak passwords, exposed credential dumps.

\- How it’s usually mitigated: MFA, rate-limiting, strong password policy, monitoring unusual logins.



---



\## Exam Reality Notes

\- CompTIA loves “BEST” answer: choose the one that reduces risk most directly in the scenario.

\- If the scenario screams “human trick,” don’t over-index on firewalls.

\- If the scenario screams “unpatched internet-facing system,” patching/segmentation usually beats awareness training.



---



\## Key Takeaways

\- Identify the attack type first, then pick the mitigation that matches the scenario.

\- Severity is not the same thing as real-world risk.

\- Social engineering is usually about emotion + process failure, not tech.



