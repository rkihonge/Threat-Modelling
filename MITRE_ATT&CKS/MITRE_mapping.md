# MITRE ATT&CK Mapping for Banking App Threats

This document maps the STRIDE threats to relevant MITRE ATT&CK techniques.

| STRIDE Category        | Threat Example                 | MITRE ATT&CK Technique | ID     |
|------------------------|--------------------------------|------------------------|--------|
| Spoofing Identity      | Phishing login pages           | Phishing               | T1566  |
| Tampering              | SQL Injection / MITM           | Exploit Public-Facing App | T1190 |
| Repudiation            | Denying transactions           | Valid Accounts misuse  | T1078  |
| Information Disclosure | API data leak                  | Data from Information Repositories | T1213 |
| Denial of Service      | Flooding login requests        | Network DoS            | T1499  |
| Elevation of Privilege | SQL Injection to admin         | Privilege Escalation   | T1068  |

## Notes
- STRIDE and MITRE frameworks complement each other.  
- STRIDE identifies **what** types of threats exist.  
- MITRE ATT&CK explains **how** attackers might execute those threats.  
