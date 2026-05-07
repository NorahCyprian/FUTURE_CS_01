FUTURE_CS_01 – Vulnerability Assessment Report for a Live Website

Task Overview
This repository contains Task 1 for the Future Interns Cyber Security Internship Program.

The objective of this task is to:
•	Identify common web security vulnerabilities in a live website 
•	Classify risk levels (Low / Medium / High) 
•	Explain findings in simple business language 
•	Provide clear remediation steps 
The assessment was conducted using passive reconnaissance and non-intrusive techniques only. No exploitation, modification, or disruptive attacks were performed during the testing process.
Target Application: DVWA (Damn Vulnerable Web Application)
Target IP Address: 192.168.56.101
Environment: Metasploitable2 Framework

Tools Used
1. Nmap
Nmap was used for network discovery, port scanning, service detection, and security auditing.
Example command used:
nmap -sC -sV 192.168.56.101
Purpose:
•	Identify open ports 
•	Detect running services and their versions 
•	Understand the attack surface of the target system 

2. OWASP ZAP (Passive Scan)
OWASP ZAP is an open-source web application security scanner used to identify vulnerabilities in web applications.
In this task, it was used in passive scanning mode only, meaning no attacks or payload injection were performed. Instead, it monitored and analyzed traffic between the browser and the target application.
Key Functions Used:
•	Intercepts HTTP/HTTPS traffic between browser and server 
•	Detects security misconfigurations 
•	Identifies insecure headers (e.g., missing Content-Security-Policy) 
•	Finds information disclosure issues 
•	Highlights potential vulnerabilities without active exploitation 

3. Browser Developer Tools
Browser Developer Tools are built-in tools in modern browsers (such as Mozilla Firefox and Chrome) used to inspect and debug web applications.
Key Functions Used:
•	Inspect HTML, CSS, and JavaScript code 
•	Monitor network requests (HTTP requests and responses) 
•	View cookies, sessions, and local storage 
•	Analyze page structure and behavior 

4. Canva (Report Design)
Canva is an online design platform used for creating professional reports and visual presentations.
Key Functions Used:
•	Designing the vulnerability assessment report layout 
•	Structuring content in a professional format 
•	Adding visual elements for better presentation 
•	Improving readability of the final report 

Deliverables Included
•	Vulnerability_Assessment_Report.pdf 
•	README.md 
•	evidence/ folder containing: 
o	nmap_scan.txt 
o	headers.txt 
o	cookies.txt 
o	Screenshots of scan outputs 
These files document the findings collected during the assessment.

Key Findings Summary
Missing Security Headers (Medium Risk)
Some HTTP security headers were not implemented, increasing the risk of client-side attacks.
Information Disclosure (Low Risk)
Server and framework information was exposed in HTTP response headers.
Insecure Cookies (Medium Risk)
Cookies were missing Secure and HttpOnly flags, increasing session security risks.

Overall Risk Level
Low – Medium
The vulnerabilities identified are mainly related to misconfigurations and information disclosure, which could assist attackers during the reconnaissance phase.

Scope and Methodology
Allowed Activities:
•	Target identification 
•	Passive scanning and reconnaissance 
•	Manual inspection using browser tools 
•	Risk classification 
•	Documentation and reporting 

Not Performed:
•	Exploitation 
•	SQL Injection testing 
•	Brute force attacks 
•	Denial-of-Service attacks 
All testing was conducted in read-only mode, following ethical cybersecurity practices.

References
•	OWASP Web Security Testing Guide 
•	Sample vulnerability reports from GitHub (as referenced in the task)

