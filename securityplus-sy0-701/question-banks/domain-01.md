\# Question Bank — Domain 1 (General Security Concepts)



\## How to use

\- Answer questions first WITHOUT looking at the key.

\- Then check the Answer Key and read the explanations.

\- Track misses in: ../progress/practice-scores.md



---



\## Questions (v1)



\### Q1

Which part of the CIA triad is primarily impacted by a denial-of-service (DoS) attack?

A) Confidentiality  

B) Integrity  

C) Availability  

D) Authentication  



\### Q2

A company requires employees to use a smart card AND a PIN to access systems. This is an example of:

A) Multifactor authentication  

B) Single sign-on  

C) Role-based access control  

D) Least privilege  



\### Q3

Which security control is considered preventive rather than detective?

A) IDS  

B) Firewall  

C) SIEM  

D) Log review  



\### Q4

Zero Trust architecture assumes:

A) Internal users are trusted by default  

B) External networks are hostile but internal is safe  

C) All access must be continuously verified  

D) Encryption is optional if the network is private  



\### Q5

Which term best describes the combination of likelihood and impact?

A) Threat  

B) Vulnerability  

C) Risk  

D) Exposure  




### Q6
Which option BEST describes authorization?
A) Proving who you are  
B) Determining what you can access  
C) Recording actions taken  
D) Encrypting communication  

### Q7
Which control BEST supports non-repudiation?
A) Hashing  
B) Symmetric encryption  
C) Digital signatures  
D) Obfuscation  

### Q8
A user reports they can access a finance share even though they are not in the Finance group. Which concept is MOST likely being violated?
A) Separation of duties  
B) Least privilege  
C) Tokenization  
D) Password complexity  

### Q9
A company adds a badge reader to a door because the lock is frequently broken and cannot be replaced immediately. The badge reader is a:
A) Corrective control  
B) Detective control  
C) Compensating control  
D) Deterrent control  

### Q10
Which is the BEST example of a detective control?
A) Firewall rule blocking inbound traffic  
B) Security guard checking IDs at the entrance  
C) Centralized log monitoring with alerting  
D) Patch management program  

### Q11
A security team blocks USB storage devices across endpoints to reduce data theft. This is an example of:
A) Deterrence  
B) Prevention  
C) Recovery  
D) Investigation  

### Q12
A company requires two employees to approve wire transfers above $10,000. This is BEST described as:
A) Defense in depth  
B) Separation of duties  
C) Single point of failure  
D) Federation  

### Q13
Which statement BEST aligns with “defense in depth”?
A) Put all security tools at the perimeter  
B) Use one strong control to reduce cost  
C) Layer controls so failure of one doesn’t equal compromise  
D) Focus only on users with admin access  

### Q14
A security analyst is asked to rank a new vulnerability as “high” because the exploit exists publicly, even though the affected system is isolated and not reachable. Which factor MOST reduces real-world risk?
A) Threat actor intent  
B) Attack surface / exposure  
C) Vulnerability severity  
D) Password policy  

### Q15
Which scenario BEST reflects “Zero Trust”?
A) VPN users are trusted after login for 8 hours  
B) Internal traffic is allowed without inspection  
C) Access is continuously evaluated and least privilege is enforced  
D) Systems are secure if the firewall is configured correctly



---



\## Answer Key + Explanations (v1)



\### A1: C) Availability

DoS attacks are designed to make a service unreachable, reducing availability.



\### A2: A) Multifactor authentication

Smart card (something you have) + PIN (something you know) = two factors.



\### A3: B) Firewall

A firewall blocks unwanted traffic (preventive). IDS and SIEM are typically detective; log review is detective.



\### A4: C) All access must be continuously verified

Zero Trust = “never trust, always verify” (even for internal traffic).



\### A5: C) Risk

Risk is commonly framed as likelihood × impact.



### A6: B) Determining what you can access
Authentication = who you are. Authorization = what you’re allowed to do. Accounting = logging/auditing.

### A7: C) Digital signatures
Digital signatures provide integrity and non-repudiation (proof a specific private key signed something).

### A8: B) Least privilege
If a user can access data they shouldn’t, they have more privilege than required.

### A9: C) Compensating control
A compensating control is used when the “ideal” control isn’t possible right now.

### A10: C) Centralized log monitoring with alerting
Detective controls identify events (logging/monitoring). Firewalls and guards are typically preventive; patching is preventive/corrective.

### A11: B) Prevention
Blocking USB storage reduces the likelihood of data exfiltration.

### A12: B) Separation of duties
Requiring two people prevents one person from completing a high-risk action alone.

### A13: C) Layer controls so failure of one doesn’t equal compromise
That’s the whole point: multiple layers reduce single-control failure risk.

### A14: B) Attack surface / exposure
If the vulnerable system isn’t reachable, exposure is reduced, lowering practical risk even if severity is high.

### A15: C) Access is continuously evaluated and least privilege is enforced
Zero Trust assumes no implicit trust—verification and least privilege are ongoing.




