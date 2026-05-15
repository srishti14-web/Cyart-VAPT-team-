 Week 2 - Vulnerability Assessment and Penetration Testing (VAPT)

## Objective
This project demonstrates the complete Vulnerability Assessment and Penetration Testing (VAPT) workflow including reconnaissance, vulnerability scanning, exploitation, post-exploitation, and reporting. The assessment was conducted using multiple cybersecurity tools in controlled lab environments and intentionally vulnerable targets.

---

## Tools Used

| Tool | Purpose |
|------|----------|
| Nmap | Network scanning and service detection |
| Nikto | Web vulnerability scanning |
| Metasploit | Exploitation framework |
| Shodan | OSINT and exposed service discovery |
| Wappalyzer | Technology stack identification |
| Sublist3r | Subdomain enumeration |
| sha256sum | Evidence hashing |

---

## Targets Used

| Target | Purpose |
|--------|----------|
| testfire.net | Reconnaissance and web vulnerability scanning |
| Metasploitable2 | Exploitation and post-exploitation testing |

---

## VAPT Workflow

Reconnaissance  
↓  
Scanning  
↓  
Vulnerability Analysis  
↓  
Exploitation  
↓  
Post-Exploitation  
↓  
Reporting  

---

## Project Structure

```text
Week 2/
├── README.md
├── Theoretical Knowledge/
├── Vulnerability Scanning Lab/
├── Reconnaissance Practice/
├── Exploitation Lab/
├── Post-Exploitation Practice/
├── Capstone Project/
```

Key Findings
- Potential DOM-Based XSS identified on target application
- Missing CSRF protections observed
- Weak SSL/TLS configurations detected
- Samba and DistCC remote command execution vulnerabilities tested
- Multiple exposed services identified during reconnaissance and scanning

Vulnerabilities Identified

| Vulnerability                    | Severity | CVSS Score |
| -------------------------------- | -------- | ---------- |
| DOM-Based XSS                    | Medium   | 6.1        |
| Missing CSRF Protection          | Medium   | 6.5        |
| Slowloris Denial of Service      | High     | 7.5        |
| Weak Diffie-Hellman Key Exchange | Medium   | 5.9        |
| Samba Username Map Script RCE    | High     | 8.0        |
| UnrealIRCd Backdoor RCE          | Critical | 9.8        |
| DistCC Command Execution         | High     | 8.1        |

Exploitation summary 

| Exploit ID | Description                   | Target IP      | Status    |
| ---------- | ----------------------------- | -------------- | --------- |
| 004        | Samba Username Map Script RCE | 192.168.56.102 | Attempted |
| 005        | UnrealIRCd Backdoor RCE       | 192.168.56.102 | Attempted |
| 006        | DistCC Command Execution      | 192.168.56.102 | Success   |


├── Screenshots/
├── Reports/
└── Scan Results/
