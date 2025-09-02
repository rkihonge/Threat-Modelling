# STRIDE Threat Modelling – Online Banking App

## 1. Spoofing
- **Threat**: Attacker impersonates a user (phishing, credential stuffing).  
- **Mitigation**: Multi-factor authentication (MFA), rate limiting, anomaly detection.  

## 2. Tampering
- **Threat**: Malicious actor alters transaction data in transit.  
- **Mitigation**: Strong TLS, integrity checks, secure APIs.  

## 3. Repudiation
- **Threat**: User denies making a transaction.  
- **Mitigation**: Non-repudiation controls (transaction logs, digital signatures).  

## 4. Information Disclosure
- **Threat**: Sensitive user data (PINs, account info) leaked.  
- **Mitigation**: Encryption at rest/in transit, strict data access policies.  

## 5. Denial of Service
- **Threat**: Banking app becomes unavailable due to DDoS.  
- **Mitigation**: WAF, rate limiting, scalable infrastructure.  

## 6. Elevation of Privilege
- **Threat**: Attacker gains admin access through vulnerability.  
- **Mitigation**: RBAC, principle of least privilege, patch management.  
