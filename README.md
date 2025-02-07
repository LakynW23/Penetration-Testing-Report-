# Penetration-Testing-Report-
Penetration Testing Report

This report outlines the findings of a penetration test performed on the target system to assess its security posture and identify vulnerabilities that could be exploited by attackers.

Test Date: January 10, 2025
Tested By: Lakyn Wheeler
Target System: Web Application (TryHackMe)

The test was conducted on the following systems:

Web Application: example.com
Testing Type: Black-box (no prior knowledge)
Methods: Scanning, vulnerability assessment, exploitation, reporting

The test followed a structured methodology:

Reconnaissance: Information gathering (OSINT, DNS, WHOIS)
Scanning: Network and vulnerability scanning (Nmap, Nessus)
Exploitation: Manual exploitation of identified vulnerabilities
Reporting: Documentation of findings and recommendations

Critical
Vulnerability: Remote Code Execution (RCE) in File Upload
Risk: Full server compromise
Recommendation: Validate file types, store outside web root
High
Vulnerability: SQL Injection in Login Form
Risk: Authentication bypass and data leakage
Recommendation: Use parameterized queries, sanitize user input
Medium
Vulnerability: Cross-Site Scripting (XSS) in Contact Form
Risk: User session hijacking
Recommendation: Implement input validation and output encoding
Low
Vulnerability: Open Unused Ports (Telnet, FTP)
Risk: Increased attack surface
Recommendation: Close unused ports and restrict access

Secure file upload functionality (validate file types, restrict uploads).
Implement prepared statements for all database queries.
Sanitize and encode user input to prevent XSS attacks.
Close unnecessary ports (Telnet, FTP) and restrict access with a firewall.

The penetration test revealed critical vulnerabilities such as RCE and SQL Injection, requiring immediate attention. Medium and low risks were also identified and should be addressed for improved security. Regular security reviews and testing are recommended to maintain a strong security posture.
