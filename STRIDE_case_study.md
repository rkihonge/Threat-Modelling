# STRIDE Threat Modelling: Online Banking App

This case study applies the STRIDE framework to a **banking web application** with features such as:
- User login
- Account balance viewing
- Fund transfers
- Customer support messaging

---

## STRIDE Analysis

### 1. Spoofing Identity
**Threat:** Attackers create fake login pages (phishing) to steal credentials.  
**Impact:** Unauthorized access to user accounts.  
**Mitigation:**  
- Multi-factor authentication (MFA)  
- Strong password policies  
- Domain monitoring for phishing sites  

---

### 2. Tampering with Data
**Threat:** An attacker modifies transaction values in transit using Man-in-the-Middle (MITM).  
**Impact:** Altered transfers and financial loss.  
**Mitigation:**  
- Enforce HTTPS with TLS 1.3  
- Digital signatures on transactions  
- Intrusion detection for anomalous behavior  

---

### 3. Repudiation
**Threat:** Users deny making a transfer due to lack of logs.  
**Impact:** Disputes and inability to trace fraudulent actions.  
**Mitigation:**  
- Strong audit logging with timestamps  
- Non-repudiation through digital signatures  
- Immutable log storage  

---

### 4. Information Disclosure
**Threat:** Sensitive data (account balance, personal info) leaked via insecure APIs.  
**Impact:** Privacy violations, identity theft.  
**Mitigation:**  
- Encrypt data in transit and at rest  
- Apply role-based access controls (RBAC)  
- Perform API security testing  

---

### 5. Denial of Service (DoS)
**Threat:** Attackers flood the login page with massive requests.  
**Impact:** Service outage, customers locked out.  
**Mitigation:**  
- Rate limiting and throttling  
- Web Application Firewall (WAF)  
- DDoS protection services  

---

### 6. Elevation of Privilege
**Threat:** Exploiting SQL Injection to gain admin privileges.  
**Impact:** Full system compromise.  
**Mitigation:**  
- Parameterized queries and ORM  
- Regular security testing (SAST/DAST)  
- Least privilege access controls  
