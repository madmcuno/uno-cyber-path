# Domain 3 - Security Architecture

This domain is about how systems are designed so that failure is contained instead of catastrophic.

---

## Core Ideas You Must Understand

### Segmentation

What it is:  
Separating systems so compromise in one area doesn't spread everywhere.

Why it matters:  
Most real breaches get worse because everything can talk to everything.

How it shows up on the exam:  
Scenarios involving "limiting blast radius," "lateral movement," or isolating sensitive systems.

Common mistakes:
- Thinking segmentation prevents compromise (it limits damage)
- Choosing segmentation when the question asks for authentication or patching

---

### Secure Network Zones (Internal, DMZ, Management)

What it is:  
Placing systems in different trust zones based on exposure and purpose.

Why it matters:  
Public-facing systems should never have direct access to internal resources.

How it shows up on the exam:  
Public web server, database, admin access questions.

Common mistakes:
- Putting databases in DMZs
- Allowing admin access from untrusted networks

---

### Secure Protocol Selection

What it is:  
Choosing encrypted and authenticated protocols over plaintext ones.

Why it matters:  
Attackers love cleartext credentials and session data.

How it shows up on the exam:  
SSH vs Telnet, HTTPS vs HTTP, SFTP vs FTP.

Common mistakes:
- Thinking encryption fixes weak authentication
- Choosing "latest" instead of "secure"

---

### Cloud Shared Responsibility

What it is:  
Cloud providers secure infrastructure; customers secure configs, identities, and data.

Why it matters:  
Misconfiguration is the #1 cloud breach cause.

How it shows up on the exam:  
Who is responsible for patching, data security, IAM, logging.

Common mistakes:
- Assuming the provider handles everything
- Assuming the customer handles physical security

---

### High Availability vs Redundancy

What it is:  
Redundancy provides backups; availability ensures uptime.

Why it matters:  
Some systems must stay up even during failure.

How it shows up on the exam:  
Failover, load balancing, clustering.

Common mistakes:
- Confusing backups with availability
- Choosing redundancy when the question asks about uptime

---

## Key Takeaways

- Architecture limits damage; it doesn't prevent all attacks
- Public systems must be isolated
- Encryption without access control is incomplete
- Misconfiguration beats malware in the real world


