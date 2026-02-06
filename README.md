# Enterprise Cloud & VM Hardening – Multi Platform Security Architecture

## Overview
This repository documents a hands-on enterprise security hardening and monitoring lab performed across multiple local virtual machines and cloud platforms.  

The project simulates the role of a security analyst tasked with securing endpoints, servers, network infrastructure, and cloud resources while performing vulnerability assessments and implementing remediation.

The lab demonstrates real-world defensive security operations including system hardening, firewall configuration, centralized logging, vulnerability scanning, cloud IAM security, and incident prevention.

---

## Objectives
- Harden Windows and Linux systems
- Configure firewall and IDS/IPS protections
- Deploy centralized monitoring using Wazuh SIEM
- Secure Azure, AWS, and GCP cloud environments
- Perform vulnerability scanning and remediation
- Produce security audit and remediation reports

---

## Lab Environment

### Local Virtual Machines
- OPNSense Router  
- Windows 11  
- Windows Server 2022  
- Ubuntu Desktop 22.04  
- Ubuntu Server 22.04  
- CentOS Stream  
- Kali Linux  
- Wazuh Manager  

### Cloud Platforms
- Microsoft Azure  
- Amazon Web Services (AWS)  
- Google Cloud Platform (GCP)  

---

## Tools Used

### Endpoint & Network Security
- OPNSense Firewall  
- Windows Defender  
- Group Policy Editor  
- UFW / Firewalld  
- SELinux  
- Fail2ban  

### Monitoring & SIEM
- Wazuh Manager & Agents  

### Vulnerability Scanning
- Lynis  
- OpenVAS / Nessus  
- Amazon Inspector  

### Cloud Security
- Azure Defender for Cloud  
- AWS IAM & CloudTrail  
- GCP Security Command Center  

---

## Task 1 – Hardening Local Virtual Machines

### OPNSense Router
- Configured LAN firewall rules  
- Enabled Intrusion Detection System (IDS)  
- Applied rule sets  

### Windows 11
- Enabled all Windows Defender protections  
- Configured auditing via Group Policy  

### Windows Server 2022
- Configured firewall rules  
- Applied password and lockout policies  
- Enabled security auditing  

### Ubuntu Desktop & Server
- Enabled UFW  
- Hardened SSH configuration  
- Enabled unattended upgrades  
- Installed Fail2ban  

### CentOS
- Set SELinux to enforcing  
- Configured firewalld  
- Enabled auditd  

### Kali Linux
- Updated system  
- Installed OpenVAS  
- Configured Metasploit  

### Wazuh
- Installed Wazuh Manager  
- Installed agents on all VMs  
- Enabled log collection, FIM, and vulnerability detection  

---

## Task 2 – Hardening Cloud Platforms

### Azure
- Enabled Microsoft Defender for Cloud  
- Enforced MFA  
- Reviewed security recommendations  
- Configured IAM with least privilege  

### AWS
- Created IAM users, groups, and roles  
- Applied least-privilege policies  
- Enabled CloudTrail  

### GCP
- Configured IAM roles  
- Enabled Security Command Center  
- Closed unused firewall ports  

---

## Task 3 – Security Auditing & Reporting

### Local VM Findings (Examples)
- Outdated Lynis version  
- Multiple SUID/SGID binaries  
- VM environment risks  

### Remediation
- Updated Lynis  
- Audited and removed unnecessary SUID/SGID binaries  
- Enabled unattended upgrades  

### Cloud Findings
- MFA not enabled on some accounts  
- Overly permissive IAM roles  
- Open inbound firewall rules  

### Remediation
- Enabled MFA  
- Restricted IAM permissions  
- Hardened firewall rules  
- Enabled CloudTrail and SCC  

---

## Security Measures Implemented

- Centralized SIEM using Wazuh  
- Host-based firewalls enabled  
- Strong password and lockout policies  
- SELinux enforcing  
- SSH hardening  
- Least privilege IAM across clouds  
- Continuous monitoring and auditing  

---

## Report

📄 Full technical report with screenshots and remediation details:

[View Report](Report.pdf)

---

## Disclaimer
All activities were performed in isolated lab environments for educational purposes.  
No production systems were impacted.

---
