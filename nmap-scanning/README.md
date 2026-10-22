# Nmap Network Scanning Lab

## 1. Overview

- **Project:** Nmap Network Scanning and Service Discovery
- **Category:** Network Security
- **Tool:** Nmap
- **Environment:** Kali Linux and an authorized training target
- **Status:** In progress

## 2. Objective

The objective of this lab is to understand how Nmap identifies accessible hosts, scans network ports, detects services, and reports port states.

## 3. Scope and Authorization

Testing is restricted to the designated training target for which I have authorization.

- **Target:** [Training target or sanitized identifier]
- **Environment:** [Lab platform or local lab]
- **Date performed:** [Date]

## 4. Tools Used

- Kali Linux
- Nmap
- Terminal for executing and documenting commands

## 5. Methodology

### Step 1: Identify the target

I confirmed the target address and verified that it belonged to my authorized lab environment.

### Step 2: Perform a basic scan

Command:

`nmap 10.80.138.42`

Purpose: Scan the target's commonly scanned TCP ports and report the observed port states.

### Step 3: Investigate discovered services

Command:

`nmap -sV 10.80.138.42`

Purpose: Attempt to identify the services and versions running on discovered ports.

### Step 4: Save scan output

Command:

`nmap -sV -oN nmap-results.txt 10.80.138.42`

Purpose: Save the scan output in normal text format for analysis and documentation.

## 6. Results and Findings

Record only the results observed during the actual scan.

| Port | State | Service | Observation |
|---|---|---|---|
| [Actual port] | [Actual state] | [Actual service] | [Your interpretation] |

If no scan has been performed yet, leave this table empty until you collect results.

## 7. Understanding Port States

- **Open:** An application is listening on the port.
- **Closed:** The port responded, but no application was listening on it at the time of the scan.
- **Filtered:** Nmap could not determine whether the port was open or closed because network filtering prevented a conclusive result.
- **Open|filtered:** Nmap could not distinguish between an open port and a filtered port.

## 8. Security Analysis

Explain which discovered services need further investigation and why. An open port is not automatically a vulnerability; additional validation is needed to determine whether a service is exposed unnecessarily or has a security weakness.

## 9. Recommendations

Depending on the actual findings:

- Disable unnecessary services.
- Restrict access to administrative services.
- Apply security updates to vulnerable software.
- Use firewall rules to limit exposure.
- Reassess the system after remediation.

## 10. Evidence

Add sanitized screenshots or relevant command output to the `screenshots/` folder.

- Basic scan output
- Service detection output
- Relevant analysis

## 11. What I Learned

Complete this section after performing the lab. Explain what you learned about port states, service discovery, scan options, and interpreting results.

## 12. References

- Nmap Reference Guide: https://nmap.org/book/man.html
- Nmap Service and Version Detection: https://nmap.org/book/man-version-detection.html
