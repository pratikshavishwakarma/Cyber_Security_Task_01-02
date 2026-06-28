# Ethical Hacking Task 02 – Network Scanning & Service Enumeration

## Overview

This repository contains the deliverables for **Ethical Hacking Task 02 – Network Scanning & Service Enumeration**, completed as part of the **White Band Associates Ethical Hacking Internship Program**.

The objective of this task was to understand the **Scanning and Enumeration** phase of the ethical hacking lifecycle by using **Nmap** to perform authorized network reconnaissance against a local target. The assessment involved verifying the scanning environment, identifying open ports, detecting running services, attempting operating system fingerprinting, and analyzing the security posture of the target system.

All activities were performed in a controlled and authorized laboratory environment for educational purposes only.

---

# Objectives

* Verify the installation and configuration of Nmap.
* Perform a default TCP port scan.
* Identify running services using version detection.
* Attempt operating system fingerprinting.
* Study commonly used network ports and their security implications.
* Analyze scan results and document security observations.
* Understand the role of network scanning in penetration testing.

---

# Technologies Used

| Component        | Details                                            |
| ---------------- | -------------------------------------------------- |
| Operating System | Kali Linux                                         |
| Target Host      | localhost (127.0.0.1)                              |
| Scanning Tool    | Nmap 7.98                                          |
| Scan Types       | TCP SYN Scan, Service Detection, OS Fingerprinting |
| Environment      | Authorized Internal Lab                            |

---

# Repository Structure

```text
Ethical-Hacking-Task-02/
│
├── README.md
├── Ethical_Hacking_Task_02_Pratiksha_Vishwakarma.pdf
├── Research_Notes.pdf
└── Screenshots/
```

---

# Nmap Commands Executed

## Verify Installation

```bash
nmap --version
```

Verifies that Nmap is correctly installed and displays the current version.

---

## Default TCP Port Scan

```bash
nmap localhost
```

Scans the default 1000 TCP ports to identify open or closed ports.

---

## Service Version Detection

```bash
nmap -sV localhost
```

Attempts to identify services and software versions running on discovered ports.

---

## Operating System Detection

```bash
sudo nmap -O localhost
```

Performs operating system fingerprinting using raw packet analysis.

---

# Scan Summary

| Assessment                 | Result                 |
| -------------------------- | ---------------------- |
| Nmap Installation          | Successful             |
| Host Status                | Up                     |
| Target                     | localhost (127.0.0.1)  |
| TCP Ports Scanned          | 1000                   |
| Open Ports                 | None                   |
| Running Services           | None Detected          |
| Service Detection          | Completed Successfully |
| Operating System Detection | Inconclusive           |

---

# Key Findings

* Successfully verified **Nmap 7.98** installation.
* Completed reconnaissance using multiple Nmap scanning techniques.
* All scanned TCP ports were reported as **closed**.
* No active services were detected on the target.
* Service enumeration completed successfully but no service banners were available.
* Operating system fingerprinting was inconclusive because no open ports were available for reliable analysis.
* The target system presented a minimal network attack surface during testing.

---

# Common Network Ports Studied

The following ports were researched to understand their functionality and associated security risks.

| Port  | Service                       |
| ----- | ----------------------------- |
| 20/21 | FTP                           |
| 22    | SSH                           |
| 23    | Telnet                        |
| 25    | SMTP                          |
| 53    | DNS                           |
| 80    | HTTP                          |
| 110   | POP3                          |
| 143   | IMAP                          |
| 443   | HTTPS                         |
| 445   | SMB                           |
| 3389  | Remote Desktop Protocol (RDP) |

---

# Security Recommendations

* Disable unused network services.
* Replace insecure protocols such as FTP and Telnet with secure alternatives.
* Enable encryption for all remote communication.
* Perform periodic network scans to identify unauthorized services.
* Restrict remote administrative access through VPNs and Multi-Factor Authentication.
* Follow the Principle of Least Privilege by exposing only essential services.
* Conduct network scanning only with explicit authorization.

---

# Skills Demonstrated

* Network Reconnaissance
* Network Scanning
* Service Enumeration
* Operating System Fingerprinting
* Port Analysis
* TCP/IP Fundamentals
* Nmap Command Usage
* Security Assessment
* Cybersecurity Documentation
* Ethical Hacking Methodology

---

# Learning Outcomes

This task provided practical experience in:

* Understanding the Scanning and Enumeration phase of penetration testing.
* Using Nmap for network discovery.
* Interpreting port scan results.
* Identifying network exposure.
* Understanding service detection techniques.
* Learning the importance of operating system fingerprinting.
* Evaluating the security posture of a target system.
* Applying ethical hacking practices in a controlled environment.

---

# Deliverables

* Comprehensive Task Report
* Professional Research Notes
* Command Outputs
* Supporting Screenshots
* GitHub Documentation (README)

---

# Disclaimer

This project was completed exclusively for educational purposes under the White Band Associates Ethical Hacking Internship Program.

All scans were performed against the analyst's own machine (`127.0.0.1`) within an authorized laboratory environment. No unauthorized systems, devices, or networks were scanned. This repository is intended solely for academic learning and ethical cybersecurity training.

---

# Author

**Pratiksha Vishwakarma**

Ethical Hacking Intern
White Band Associates

---

# Acknowledgements

Special thanks to **White Band Associates** for providing the internship program and hands-on cybersecurity tasks that enabled practical learning in network scanning, service enumeration, and ethical hacking methodologies.
