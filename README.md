# FUTURE_CS_01 – Vulnerability Assessment Report for a Live Website

## Task Overview
     This repository contains Task 1 for the Future Interns Cyber Security Internship Program and the objective of this task is to identify common web security vulnerabilities in a live website, classify risk levels (Low / Medium / High), Explain findings in simple business language and provide clear remediation steps. The assessment was conducted using passive reconnaissance and non-intrusive techniques only. No exploitation, modification, or disruptive attacks were performed during the testing process.Target Application: DVWA (Damn Vulnerable Web Application),Target IP Address: 127.0.0.1,Environment: Oracle Virtual Box Manager

---

## Tools Used
1.	Nmap
            Used for network discovery, port scanning, service detection and security auditing.
             Example command used: nmap -sC -Pn 127.0.0.1
           Purpose:
•	Identify open ports
•	Detect running services and their version.



2.	OWASP ZAP (Passive Scan)
             is an open-source web application security scanner used to identify vulnerabilities in web applications.
            In this task, it used in passive scanning mode only, meaning no attacks or payload injection were performed. Instead, it observed and analyzed the traffic between the browser and the target application.
           Key Functions Used:
•	Intercepts HTTP/HTTPS traffic between browser and server 
•	Detects security misconfigurations 
•	Identifies insecure headers, example missing Content Security Policy
•	Finds information disclosure issues 
•	Highlights potential vulnerabilities without active exploitation

3.	Browser Developer Tools
            are built-in tools in modern browsers (such as Mozilla Firefox) used to inspect and debug web applications.
            Key Functions Used:
•	Inspect HTML, CSS, and JavaScript code 
•	Monitor network requests (HTTP requests and responses) 
•	View cookies, sessions, and local storage 
•	Analyze page structure and behavior 





4.	Canva (Report Design)
             Browser Developer Tools are built-in tools in modern browsers (such as Chrome or Firefox) used to inspect and debug web applications.
              Key Functions Used:
•	Inspect HTML, CSS, and JavaScript code 
•	Monitor network requests (HTTP requests and responses) 
•	View cookies, sessions, and local storage 
•	Identify client-side security issues 
•	Analyze page structure and behavior 


---

## Deliverable Included
•	Vulnerability_Assessment_Report.pdf
•	README.md
•	evidence/
Evidence folder contains:
•	nmap scan.txt
•	headers.txt
•	cookies.txt
•	whatweb.txt

These files document the findings collected during the assessment.

---

## Key Findings Summary

1. Missing Content-Security-Policy (CSP) header - Medium 
2. MySQL database exposed on port 3306 - Medium 
3. Missing X-Frame-Options header - Medium 
4. Cookie missing Secure and SameSite attributes - Low 
5. Server version information disclosure - Low

---


VULNERABILITY
1. Missing Content-Security-Policy (CSP) header - Medium 
2. MySQL database exposed on port 3306 - Medium 
3. Missing X-Frame-Options header - Medium 
4. Cookie missing Secure and SameSite attributes - Low 
5. Server version information disclosure - Low 

---





 ## Overall Risk Level

Low – Medium
The vulnerabilities discovered mainly involve misconfigurations and information disclosure, which could assist attackers during reconnaissance phases.

---


## Scope and Methodology

Allowed activities:
  1. Target identification 
  2. Passive scanning and reconnaissance
  3. Manual inspection using browser tools
  4. Risk classification
 5. Documentation and reporting 

Not performed:
•	Exploitation
•	SQL Injection testing
•	Brute force attacks
•	Denial-of-Service attacks
All testing was conducted in read-only mode, respecting ethical guidelines.

 ## References
•	OWASP Web Security Testing Guide
•	Sample vulnerability reports from GitHub (as suggested in the task)


...
 ## Author
NORAH CYPRIAN NGILIULE  
CIN ID: FIT/MAY26/CS8136  
Future Interns Cyber Security Internship (2026)


 ## Repository Link
https://github.com/NorahCyprian/FUTURE_CS_01











