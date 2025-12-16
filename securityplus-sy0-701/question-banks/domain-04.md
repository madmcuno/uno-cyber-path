\# Question Bank — Domain 4 (Security Operations)



\## How to Use

\- Answer questions without looking at the answer key.

\- Write answers as: `1C 2A 3B ...`

\- Review explanations for every missed question.

\- Log results in `progress/practice-scores.md`.



---



\## Questions



\### Q1 — First IR Priority



A host is suspected of active compromise and is communicating with an unknown external IP. What is the BEST immediate action?



A) Delete all logs to protect privacy  

B) Isolate the host from the network  

C) Announce the incident company-wide immediately  

D) Power off the entire data center



---



\### Q2 — Log Correlation



Which tool is MOST associated with collecting and correlating logs across systems to detect incidents?



A) SIEM  

B) DNS  

C) DHCP  

D) NAS



---



\### Q3 — Evidence Handling



Which practice BEST preserves evidence integrity during an investigation?



A) Modify files to add notes  

B) Use a chain of custody  

C) Copy evidence without documenting dates/times  

D) Store evidence on a shared public folder



---



\### Q4 — Least Destructive Approach



When investigating a potentially infected machine, what is the BEST approach to avoid destroying evidence?



A) Run cleanup tools immediately  

B) Take a forensic image first  

C) Reimage the system immediately  

D) Delete suspicious files



---



\### Q5 — Detection vs Prevention



An IDS alert indicates suspicious traffic but no traffic is blocked. What is the IDS primarily doing?



A) Preventing  

B) Detecting  

C) Correcting  

D) Recovering



---



\### Q6 — Authentication Logs



Which log source is MOST useful for investigating repeated failed logins across multiple accounts?



A) Web server access logs only  

B) Authentication / directory service logs  

C) Printer logs  

D) Temperature sensor logs



---



\### Q7 — Containment Goal



What is the PRIMARY goal of containment during incident response?



A) Train employees  

B) Prevent further damage/spread  

C) Publish a postmortem  

D) Replace all hardware



---



\### Q8 — False Positive



A detection rule triggers alerts for normal admin activity. This is MOST likely a:



A) True negative  

B) False positive  

C) False negative  

D) True positive



---



\### Q9 — Vulnerability Scanning Output



A vulnerability scan reports missing patches and weak configurations. What should happen NEXT?



A) Ignore it because scanners are noisy  

B) Prioritize remediation based on risk and exposure  

C) Shut down the whole network  

D) Only update documentation



---



\### Q10 — Backups in Ops



Which backup approach MOST helps defend against ransomware?



A) Backups stored on the same writable share as production  

B) Offline/immutable backups with restore testing  

C) Backups that overwrite previous versions only  

D) No backups, rely on antivirus



---



\## Answer Key \& Explanations



\### Q1

\*\*Correct Answer:\*\* B — Isolate the host from the network  

Containment starts by stopping communication/spread while preserving evidence as much as possible.



\### Q2

\*\*Correct Answer:\*\* A — SIEM  

SIEM aggregates and correlates logs to detect patterns and alerts.



\### Q3

\*\*Correct Answer:\*\* B — Use a chain of custody  

Chain of custody documents who handled evidence and when, preserving integrity and admissibility.



\### Q4

\*\*Correct Answer:\*\* B — Take a forensic image first  

Imaging preserves a point-in-time copy before actions change the system.



\### Q5

\*\*Correct Answer:\*\* B — Detecting  

IDS detects/alerts; IPS blocks.



\### Q6

\*\*Correct Answer:\*\* B — Authentication / directory service logs  

Those logs show account, source, time, and failure reasons.



\### Q7

\*\*Correct Answer:\*\* B — Prevent further damage/spread  

Containment is about limiting impact quickly.



\### Q8

\*\*Correct Answer:\*\* B — False positive  

Alert fired but activity was legitimate.



\### Q9

\*\*Correct Answer:\*\* B — Prioritize remediation based on risk and exposure  

Scanning findings must be triaged; fix the highest risk/exposure first.



\### Q10

\*\*Correct Answer:\*\* B — Offline/immutable backups with restore testing  

If ransomware can encrypt backups, they aren’t backups—they’re hostages.

\# Question Bank — Domain 4 (Security Operations)



\## How to Use

\- Answer questions without looking at the answer key.

\- Write answers as: `1C 2A 3B ...`

\- Review explanations for every missed question.

\- Log results in `progress/practice-scores.md`.



---



\## Questions



\### Q1 — First IR Priority



A host is suspected of active compromise and is communicating with an unknown external IP. What is the BEST immediate action?



A) Delete all logs to protect privacy  

B) Isolate the host from the network  

C) Announce the incident company-wide immediately  

D) Power off the entire data center



---



\### Q2 — Log Correlation



Which tool is MOST associated with collecting and correlating logs across systems to detect incidents?



A) SIEM  

B) DNS  

C) DHCP  

D) NAS



---



\### Q3 — Evidence Handling



Which practice BEST preserves evidence integrity during an investigation?



A) Modify files to add notes  

B) Use a chain of custody  

C) Copy evidence without documenting dates/times  

D) Store evidence on a shared public folder



---



\### Q4 — Least Destructive Approach



When investigating a potentially infected machine, what is the BEST approach to avoid destroying evidence?



A) Run cleanup tools immediately  

B) Take a forensic image first  

C) Reimage the system immediately  

D) Delete suspicious files



---



\### Q5 — Detection vs Prevention



An IDS alert indicates suspicious traffic but no traffic is blocked. What is the IDS primarily doing?



A) Preventing  

B) Detecting  

C) Correcting  

D) Recovering



---



\### Q6 — Authentication Logs



Which log source is MOST useful for investigating repeated failed logins across multiple accounts?



A) Web server access logs only  

B) Authentication / directory service logs  

C) Printer logs  

D) Temperature sensor logs



---



\### Q7 — Containment Goal



What is the PRIMARY goal of containment during incident response?



A) Train employees  

B) Prevent further damage/spread  

C) Publish a postmortem  

D) Replace all hardware



---



\### Q8 — False Positive



A detection rule triggers alerts for normal admin activity. This is MOST likely a:



A) True negative  

B) False positive  

C) False negative  

D) True positive



---



\### Q9 — Vulnerability Scanning Output



A vulnerability scan reports missing patches and weak configurations. What should happen NEXT?



A) Ignore it because scanners are noisy  

B) Prioritize remediation based on risk and exposure  

C) Shut down the whole network  

D) Only update documentation



---



\### Q10 — Backups in Ops



Which backup approach MOST helps defend against ransomware?



A) Backups stored on the same writable share as production  

B) Offline/immutable backups with restore testing  

C) Backups that overwrite previous versions only  

D) No backups, rely on antivirus



---



\## Answer Key \& Explanations



\### Q1

\*\*Correct Answer:\*\* B — Isolate the host from the network  

Containment starts by stopping communication/spread while preserving evidence as much as possible.



\### Q2

\*\*Correct Answer:\*\* A — SIEM  

SIEM aggregates and correlates logs to detect patterns and alerts.



\### Q3

\*\*Correct Answer:\*\* B — Use a chain of custody  

Chain of custody documents who handled evidence and when, preserving integrity and admissibility.



\### Q4

\*\*Correct Answer:\*\* B — Take a forensic image first  

Imaging preserves a point-in-time copy before actions change the system.



\### Q5

\*\*Correct Answer:\*\* B — Detecting  

IDS detects/alerts; IPS blocks.



\### Q6

\*\*Correct Answer:\*\* B — Authentication / directory service logs  

Those logs show account, source, time, and failure reasons.



\### Q7

\*\*Correct Answer:\*\* B — Prevent further damage/spread  

Containment is about limiting impact quickly.



\### Q8

\*\*Correct Answer:\*\* B — False positive  

Alert fired but activity was legitimate.



\### Q9

\*\*Correct Answer:\*\* B — Prioritize remediation based on risk and exposure  

Scanning findings must be triaged; fix the highest risk/exposure first.



\### Q10

\*\*Correct Answer:\*\* B — Offline/immutable backups with restore testing  

If ransomware can encrypt backups, they aren’t backups—they’re hostages.



