# Wazuh-Homelab-Lite

# SOC Monitoring Lab using Wazuh SIEM

## Overview

This project demonstrates the deployment and configuration of a Wazuh Security Information and Event Management (SIEM) environment for endpoint monitoring, security configuration assessment, file integrity monitoring, and audit logging on a Linux system.

The lab was created to gain practical exposure to Security Operations Center (SOC) workflows, endpoint visibility, security monitoring, and Linux security hardening concepts.

---

## Objectives

* Deploy and configure a Wazuh SIEM environment.
* Integrate a Linux endpoint for centralized monitoring.
* Analyze Security Configuration Assessment (SCA) findings.
* Implement File Integrity Monitoring (FIM) for sensitive files and directories.
* Configure Linux audit logging using auditd.
* Generate and review security monitoring reports.

---

## Lab Environment

| Component           | Description             |
| ------------------- | ----------------------- |
| SIEM Platform       | Wazuh                   |
| Endpoint            | Kali Linux              |
| Operating System    | Kali GNU/Linux 2026.1   |
| Monitoring Features | SCA, FIM, Audit Logging |
| Audit Framework     | auditd                  |

---

## Architecture

```text
+--------------------+
|    Kali Linux      |
|--------------------|
| Wazuh Agent        |
| auditd             |
+---------+----------+
          |
          |
          v
+--------------------+
|   Wazuh Manager    |
|--------------------|
| Log Collection     |
| SCA Analysis       |
| FIM Monitoring     |
| Event Correlation  |
| Reporting          |
+--------------------+
```

---

## Features Implemented

### Endpoint Integration

* Installed and configured a Wazuh agent on a Kali Linux endpoint.
* Registered the endpoint with the Wazuh manager.
* Enabled centralized collection of security telemetry and system events.

---

### Security Configuration Assessment (SCA)

Utilized Wazuh's Security Configuration Assessment module to evaluate the endpoint's security posture.

Examples of reviewed findings included:

* SSH hardening recommendations
* Password policy configuration
* Audit logging configuration
* Access control settings
* Password hashing requirements
* Linux system hardening checks

The assessment provided visibility into security control gaps and configuration weaknesses.

---

### File Integrity Monitoring (FIM)

Configured Wazuh File Integrity Monitoring policies to monitor sensitive directories and files.

Validation activities included:

* File creation detection
* File modification detection
* Metadata change detection
* File deletion detection

This demonstrated the ability to identify unauthorized changes within monitored locations.

---

### Audit Logging

Installed and configured Linux Audit Daemon (auditd).

Audit policies were configured to:

* Monitor process execution events
* Capture system-call activity
* Improve visibility into endpoint actions
* Support forensic and security monitoring activities

---

## Sample Findings

Examples of findings observed through Wazuh include:

* Security Configuration Assessment alerts
* Linux package installation events
* Configuration change events
* Host-based anomaly detection events
* Agent lifecycle events

---

## Skills Demonstrated

### Security Operations

* Security Monitoring
* Endpoint Monitoring
* SIEM Operations
* Security Event Analysis
* Log Analysis

### System Security

* Linux Hardening
* SSH Security
* File Integrity Monitoring (FIM)
* Audit Logging
* Access Control Monitoring

### Governance & Compliance

* Security Configuration Assessment (SCA)
* Security Baseline Review
* Compliance Monitoring
* Control Assessment

### Tools & Technologies

* Wazuh
* Kali Linux
* auditd
* Linux

---

## Screenshots

### Wazuh Dashboard

*Add screenshot here*

### Security Configuration Assessment Findings

*Add screenshot here*

### File Integrity Monitoring Events

*Add screenshot here*

### Security Events Report

!(./assets/security events.png)[security events]

---

## Learning Outcomes

Through this lab, I gained hands-on experience with:

* Deploying and configuring a SIEM platform
* Endpoint onboarding and monitoring
* Security Configuration Assessment (SCA)
* File Integrity Monitoring (FIM)
* Linux audit logging
* Security event analysis
* Security reporting and documentation

---

## Author

Dhruti Avadhani

Cybersecurity Student | Security Operations | Application Security | Cloud Security
