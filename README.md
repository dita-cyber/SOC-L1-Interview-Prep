# SOC-L1-Interview-Prep

Exactly a year ago, I was deep in preparation for my first SOC technical interview for a L1 analyst position. During that time, I gathered notes and study materials that helped me build an organized review of cybersecurity concepts. I’ve kept those notes ever since, and now I’ve finally decided to organize them digitally, not just for my own future reference, but also to help others who might be seeking some structure in their own interview prep.

While it’s impossible to predict every question an interviewer might ask, I believe the topics covered in these notes represent a strong starting point for anyone aiming to land an L1 SOC role. 

----

**CIA Triad**
Confidentiality: Protect information from unauthorized access.
Integrity: Ensure information has not been altered.
Availability: Ensure information is accessible when needed.

----

**IOC (Indicators of Compromise)**

Well-defined evidence of a breach; digital footprints such as:

Unusual outbound traffic
Anomalies in privileged user account activity
Login red flags
Increases in database read volume
Unusual HTML response sizes

-----

**Vulnerability vs. Risk vs. Threat**

Vulnerability: A weakness or gap in an organization’s defenses that could be exploited.
Risk: The likelihood that a threat will exploit a vulnerability.
Threat: A potential danger or action that could cause harm or damage.

-----

**Event vs. Incident**

Event: Any observable, verifiable, and documentable occurrence.
Incident: An event that negatively affects a company or impacts its security posture.

Note: Not every event is an incident, but every incident is an event.

-----

**Incident Response Process**

A structured approach to handling cybersecurity breaches, aimed at minimizing damage and reducing recovery time.

Preparation: Develop a response plan, train the team, and set up tools.
Identification: Monitor and analyze logs, audit trails, alerts, and firewall reports.
Containment: Isolate affected systems to limit spread and impact.
Eradication: Completely remove the threat from the environment.
Recovery: Restore systems and data; test to ensure normal operations.
Lessons Learned: Review the incident, document findings, and improve defenses.
