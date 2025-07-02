# SOC-L1-Interview-Prep

Exactly a year ago, I was deep in preparation for my first SOC technical interview for a L1 analyst position. During that time, I gathered notes and study materials that helped me build an organized review of cybersecurity concepts. I’ve kept those notes ever since, and now I’ve finally decided to organize them digitally, not just for my own future reference, but also to help others who might be seeking some structure in their own interview prep.

While it’s impossible to predict every question an interviewer might ask, I believe the topics covered in these notes represent a strong starting point for anyone aiming to land an L1 SOC role. 

----

**CIA Triad**<br/>
Confidentiality: Protect information from unauthorized access.<br/>
Integrity: Ensure information has not been altered.<br/>
Availability: Ensure information is accessible when needed.<br/>

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

Vulnerability: A weakness or gap in an organization’s defenses that could be exploited.<br/>
Risk: The likelihood that a threat will exploit a vulnerability.<br/>
Threat: A potential danger or action that could cause harm or damage.<br/>

-----

**Event vs. Incident**<br/>

Event: Any observable, verifiable, and documentable occurrence.<br/>
Incident: An event that negatively affects a company or impacts its security posture.<br/>

Note: Not every event is an incident, but every incident is an event.<br/>

-----

**Incident Response Process**<br/>

A structured approach to handling cybersecurity breaches, aimed at minimizing damage and reducing recovery time.<br/>

Preparation: Develop a response plan, train the team, and set up tools.<br/>
Identification: Monitor and analyze logs, audit trails, alerts, and firewall reports.<br/>
Containment: Isolate affected systems to limit spread and impact.<br/>
Eradication: Completely remove the threat from the environment.<br/>
Recovery: Restore systems and data; test to ensure normal operations.<br/>
Lessons Learned: Review the incident, document findings, and improve defenses.<br/>

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
