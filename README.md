# SOC-L1-Interview-Prep

Exactly a year ago, I was deep in preparation for my first SOC technical interview for a L1 analyst position. During that time, I gathered notes and study materials that helped me build an organized review of cybersecurity concepts. I’ve kept those notes ever since, and now I’ve finally decided to organize them digitally, not just for my own future reference, but also to help others who might be seeking some structure in their own interview prep.

While it’s impossible to predict every question an interviewer might ask, I believe the topics covered in these notes represent a strong starting point for anyone aiming to land an L1 SOC role. 

----

**CIA Triad**<br/>
**Confidentiality:** Protect information from unauthorized access.<br/>
**Integrity:** Ensure information has not been altered.<br/>
**Availability:** Ensure information is accessible when needed.<br/>

----

**IOC (Indicators of Compromise)**<br/>

Evidence of a breach; digital footprints. Examples:<br/>

- Unusual outbound traffic<br/>
- Anomalies in privileged user account activity<br/>
- Suspicious config changes<br/>
- Increases in database read volume<br/>
- Unusual HTML response sizes<br/>
- Activity from Blacklist countries<br/>

-----

**Vulnerability vs. Risk vs. Threat**

**Vulnerability:** A weakness or gap in an organization’s defenses that could be exploited.<br/>
**Risk:** The likelihood that a threat will exploit a vulnerability.<br/>
**Threat:** A potential danger or action that could cause harm or damage.<br/>

-----

**Event vs. Incident**<br/>

**Event:** Any observable, verifiable, and documentable occurrence.<br/>
**Incident:** An event that negatively affects a company or impacts its security posture.<br/>

Note: Not every event is an incident, but every incident is an event.<br/>

-----

**Incident Response Process**<br/>

A structured approach to handling cybersecurity breaches, aimed at minimizing damage and reducing recovery time.<br/>

**Preparation:** Develop a response plan, train the team, and set up tools.<br/>
**Identification:** Monitor and analyze logs, audit trails, alerts, and firewall reports.<br/>
**Containment:** Isolate affected systems to limit spread and impact.<br/>
**Eradication:** Completely remove the threat from the environment.<br/>
**Recovery:** Restore systems and data; test to ensure normal operations.<br/>
**Lessons Learned:** Review the incident, document findings, and improve defenses.<br/>

-----

**- SIEM:** Security Information and Event Management<br/>
**- SOAR:** Security Orchestration, Automation, and Response<br/>
**- IDS:** Intrusion Detection System. Monitors network traffic/system activities for signs of malicious activity or policy violations. Detects anomalies, raises alerts, and logs details<br/>
**- IPS:** Intrusion Prevention System.  Positioned behind perimeter firewalls. Adds an extra layer of defense to catch threats missed by firewalls. Signature-based detection <br/>
**- EDR:** Endpoint Detection and Response<br/>
**- NTA:** Network Traffic Analysis<br/>
**- WAF:** Web Application Firewall. Protects HTTP/HTTPS traffic (including APIs) - Often cloud-based and intelligent<br/>
**- Firewalls:** Network security devices that monitor and filter traffic based on policy rules<br/>

-----
 
**Defense-in-Depth**<br/>

A multi-layered security strategy that makes lateral movement by attackers more difficult<br/>

Examples:<br/>
- IDS and IPS<br/>
- NIDS (Network-based IDS)  --> Inbound/Outbound connections<br/>
- HIDS (Host-based IDS) --> East-west traffic monitoring from endpoints<br/>

-----

**Principle of Least Privilege**<br/>

Always grant the minimum level of access/permissions necessary to perform a task. Applies to access management, audits, and temporary privilege elevation<br/>

-----

**Zero Trust Model**<br/>

A security framework that assumes no implicit trust<br/>

Requires continuous verification in stages:<br/>
- User trust<br/>
- Device trust<br/>
- Application trust<br/>
- Infrastructure trust<br/>
- Session trust<br/>

-----

SOC Responsabilities 

Prevention -> Training, intel, development
Protection -> Threat hunting, monitoring, recovery
Detection -> Reporting, auditing, assess

Security incidents analysis

SOC Analyst Techniques

Monitoring, initial triage, basic investigations, identify patterns, make informed decisions based on data, search for information.
- Analysis logs and identify anomalies - Suspicious activities, unauthorized access, unusual login patterns, abnormal network traffic.
- Categorizing alerts based on time they arrived in the queue and severity.
- Identify what the alert is about and collect relevant information: OS services, OSINT data, Logs, Queries, IOCs.
- Correlate IOCs and past incidents.
- Communique and document findings and update the team.

----

Cyber Kill Chain Framework

Stages of cyber attacks - It is an adaptation of military developed by Lockeed Martin 2011 intended to defend agains sophisticated cyber attacks APT's
7 phases:
- Reconnaissance
- Weaponization
- Delivery
- Exploitation
- Installation
- Command and Control
- Action on Objective

----

MITREATT&CK Framework 

Assumes breach = intial tactis is initial intrusion. It is a knowledge base on adversary tactics and techniques based on real world events. 

14 tactics to described high-level steps used by adversaries
techniques is the subcategory that includes description, detection, prevention/mitigation that are recommended

Reconnaissance: Gather information
Examples: OSINT, port scanning, phishing, network/host information

Resource Development: Establish resources to support operations
Examples: Acquire accounts, infrastructure

Initial Access: Trying to get into the network
Examples: Remote media, exploit application, phishing, supply chain, content injection

Execution: Run malicious code
Examples: Scheduled tasks, commands, scripts, malicious binary

Persistence: Maintain presence into the network
Examples: Keys, accounts, registry, services, browser extentions, manipulation

Privilege Escalation: Gain higher permissions
Examples: Token, account manipulation, UAC, SetUID/SetGID (Linux User/Groups privileges)

Defense Evasion: Avoid detection
Examples: Impersonation, rookit, PID spoofing, stenography 

Credential Access: Steal account names and passwords
Examples: Brute-force, network sniffing, steal session cookies

Discovery: Trying to figure out environment information
Examples: Account discovery, network discovery, network sniffing

Lateral Moviment: Move internally through the network
Examples: Session hijacking, remote services, removable medias

Collection: Gather data of interest
Examples: Man in the middle, audio, video, email collection, repositoy, storage

Command and Control: Communicate with other compromissed system to control them
Examples: Application layer protocol, content injection, data obfuscation, non-standard ports, proxy, web services

Exfiltration: Trying to steal data and move it outside the enviroment
Examples: Physical exfiltration, storage, scheduled transfers

Impact: Manipulate, interrupt, destroy systems and data
Examples: Data destruction, manipulation, disk wipe, financial theft, system shutdown, encryption. 

----

NIST Framework

It is a reference model that guides how to secure environments and reduce risks. Holistic approach.

5 Functions (each function has a subcategory
- Identify
- Protect
- Detect
- Respond
- Recover

  4 Tiers
  Tier 1: Partial
  Tier 2: Risk Informed
  Tier 3: Repeatable 
  Tier 4: Adaptive

  Profiles:
  Roadmap by risk appetite
  Multiple profiles like current state and desired state

  ----
