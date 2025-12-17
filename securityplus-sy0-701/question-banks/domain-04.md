# Question Bank – Domain 4 (Security Operations)

## How to Use
- Answer each question cold, then grade yourself with the key below.
- Note your score in `progress/practice-scores.md` so you can track improvements.
- Always review the explanations for anything you miss.

---

## Questions

### Q1 – First IR Priority
A host shows active compromise and is talking to an unknown external IP. What is the BEST immediate action?

A) Delete all logs  
B) Isolate the host from the network  
C) Announce the incident company-wide  
D) Power off the entire data center

---

### Q2 – Log Correlation
Which tool is MOST associated with collecting and correlating logs across systems to detect incidents?

A) SIEM  
B) DNS  
C) DHCP  
D) Network-attached storage (NAS)

---

### Q3 – Evidence Handling
Which practice BEST preserves evidence integrity during an investigation?

A) Modify files to add notes  
B) Maintain a documented chain of custody  
C) Copy evidence without recording times  
D) Store evidence on a public share

---

### Q4 – Least Destructive Approach
When investigating a potentially infected machine, what is the BEST approach to avoid destroying evidence?

A) Run cleanup tools immediately  
B) Take a forensic image first  
C) Reimage the system immediately  
D) Delete suspicious files

---

### Q5 – Detection vs. Prevention
An IDS alert fires, but no traffic is blocked. What function is the IDS performing?

A) Prevention  
B) Detection  
C) Correction  
D) Recovery

---

### Q6 – Authentication Logs
Which log source is MOST useful for investigating repeated failed logins across multiple accounts?

A) Web server access logs  
B) Authentication/directory service logs  
C) Printer logs  
D) Temperature sensor logs

---

### Q7 – Containment Goal
What is the PRIMARY goal of containment during incident response?

A) Train employees  
B) Prevent further damage or spread  
C) Publish a postmortem  
D) Replace all hardware

---

### Q8 – False Positive
A detection rule triggers on normal administrator activity. This alert is a:

A) True negative  
B) False positive  
C) False negative  
D) True positive

---

### Q9 – Vulnerability Scan Output
A vuln scan reports missing patches and weak configs. What should happen NEXT?

A) Ignore it because scanners are noisy  
B) Prioritize remediation based on risk and exposure  
C) Shut down the entire network  
D) Only update documentation

---

### Q10 – Backups in Ops
Which backup approach MOST helps defend against ransomware?

A) Backups stored on the same writable share as production  
B) Offline/immutable backups with regular restore testing  
C) Backups that overwrite previous versions  
D) Skip backups and rely on antivirus

---

## Answer Key and Explanations

### Q1
**Answer:** B – Isolate the system to contain the threat while preserving evidence.

### Q2
**Answer:** A – SIEM platforms aggregate and correlate logs to surface incidents.

### Q3
**Answer:** B – A documented chain of custody preserves admissibility and integrity.

### Q4
**Answer:** B – Imaging captures the system state before cleanup alters evidence.

### Q5
**Answer:** B – IDS solutions detect/alert; prevention is handled by IPS or other controls.

### Q6
**Answer:** B – Authentication/directory logs show account names, timestamps, and failure reasons.

### Q7
**Answer:** B – Containment stops the bleeding so the incident cannot worsen.

### Q8
**Answer:** B – A false positive fires even though the activity is legitimate.

### Q9
**Answer:** B – Findings must be triaged and remediated according to risk/exposure.

### Q10
**Answer:** B – Offline/immutable backups plus testing ensure ransomware cannot encrypt your recovery path.
