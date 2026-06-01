# Week 3 – Web Application Vulnerability Assessment and Penetration Testing (VAPT)

## Overview

This folder contains the activities, screenshots, exploit evidence, and report generated during Week 3 of the VAPT training program. The assessment was conducted in a controlled laboratory environment using OWASP Broken Web Applications (BWA) and Damn Vulnerable Web Application (DVWA).

## Objectives

* Perform reconnaissance and enumeration of the target environment.
* Identify and validate common web application vulnerabilities.
* Conduct manual and automated exploitation.
* Analyze network traffic and captured requests.
* Utilize industry-standard security tools for assessment and verification.
* Document findings, risks, and remediation recommendations.

## Target Environment

* Attacker Machine: Kali Linux
* Target Machine: OWASP BWA (DVWA)
* Network Configuration: VirtualBox Host-Only Adapter
* Target IP Address: 192.168.56.104

## Tools Used

* Burp Suite
* SQLMap
* Metasploit Framework
* Wireshark
* SearchSploit (Exploit-DB)
* Firefox Browser

## Key Findings

| Vulnerability          | Severity | Status                 |
| ---------------------- | -------- | ---------------------- |
| SQL Injection          | Critical | Successfully Exploited |
| Reflected XSS          | High     | Successfully Exploited |
| Insecure CAPTCHA       | Medium   | Successfully Bypassed  |
| Information Disclosure | Medium   | Identified             |
| Directory Enumeration  | Medium   | Identified             |

## Results Summary

* Successfully intercepted and modified HTTP requests using Burp Suite.
* Demonstrated SQL Injection through manual payload manipulation.
* Used SQLMap to automate SQL Injection detection and database enumeration.
* Identified multiple SQL Injection techniques including Boolean-Based Blind, Error-Based, Time-Based Blind, and UNION Query Injection.
* Demonstrated Reflected Cross-Site Scripting (XSS) through browser-side script execution.
* Bypassed Insecure CAPTCHA validation by manipulating workflow parameters.
* Performed reconnaissance and service enumeration using Metasploit Framework.
* Identified Apache, PHP, MySQL, and related web technologies running on the target server.
* Captured and analyzed network traffic using Wireshark.
* Retrieved and customized a Python-based Proof-of-Concept exploit from Exploit-DB using SearchSploit.

## Activities Performed

1. Environment Setup and Configuration
2. Reconnaissance and Enumeration
3. Burp Suite Request Interception
4. SQL Injection Exploitation
5. Automated SQL Injection using SQLMap
6. Reflected XSS Testing
7. Insecure CAPTCHA Bypass
8. Metasploit Reconnaissance
9. Wireshark Packet Analysis
10. Exploit-DB PoC Review and Customization

## Repository Structure

* **Report/** – Final VAPT Report.
* **Screenshots/** – Testing and exploitation evidence.
* **Evidence/** – Logs and packet captures.
* **Exploits/** – Customized PoC files.

## Disclaimer

All testing activities were performed in an isolated and authorized laboratory environment strictly for educational and cybersecurity training purposes.
