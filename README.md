# Unauthenticated Basic Network Scan: Linux VM

<img width="705" height="360" alt="TenableLinux" src="https://github.com/user-attachments/assets/1e79adcc-d947-4fde-a385-a2650f9c6a7d" />

---

## Overview

The purpose of this lab was to complete an Unauthenticated Basic Network Scan. An Unauthenticated Basic Network Scan is used to identify possible vulnerabilities that can be discovered without credentials. This type of scan is considered superficial since it does not go in depth vs a Authenticated Network Scan.

In this lab I provisioned a Linux Virtual Machine, performed a ping test in terminal via SSH, logged into the Linux VM in terminal via SSH, created the Unauthenticated Basic Network Scan, reviewed the results from the scan, deleted the virtual machine.

---

## Lab Objectives

By the end of this lab I was able to:

- Provision a Linux Virtual Machine
- Perform ping test in terminal
- Create Unauthenticated Basic Network Scan
- Review scan results
- Clean up virtual machine

---

## Tools Used

- Linux Virtual Machine
- SSH
- Microsoft Azure
- Tenable Vulnerability Management
- Nessus Scanner
- Basic Network Scan

---

## Lab Environment

| Component | Description |
|---|---|
| Endpoint | Linux Virtual Machine |
| Scanner Type | Nessus Scanner |
| Scan Type | Basic Agent Scan |
| Platform | Tenable Vulnerability Management |
| Platform | Microsoft Azure |

---

## Lab Steps

### Step 1: Provision Linux Virtual Machine

The first step in this lab was to configure a Linux Virtual Machine using Microsoft Azure shown in ***Exhibit 1***.

### Why This Matters?

The virtual machine will serve as our endpoint for the Unauthenticated Basic Network Scan.

### Exhitbit 1

<img width="1918" height="919" alt="lab1" src="https://github.com/user-attachments/assets/b8eb53de-f952-4036-be6b-6818f610ad40" />

---

### Step 2: Perform Ping Test in Terminal

The second was to perform a ping test in terminal. ***Exhibit 2***

### Why This Matters?

This is necessary so we can confirm the Tenable scan can reach the VM.

<img width="695" height="277" alt="lab2" src="https://github.com/user-attachments/assets/0df48aae-309a-4d6d-821a-c815d2edd82f" />

---

### Step 3: Create Unauthenticated Basic Network Scan


***NOTE:***  *This lab assumes prior knowledge creating scans. For a step by step with visual instructions on creating an Unauthenticated Basic Network Scan refer to:* ***[Implementing a Tenable Unauthenticated Basic Network Scan: Windows 11 VM](https://github.com/mannyaguirre/Unauthenticated-Basic-Network-Scan-Windows-11)***


The third step was to Create Unauthenticated Basic Network Scan.

This was completed by following the steps outlined below:

1. Log into Tenable Vulnerability Management
2. Scans - Vulnerability Management Scans 
3. Create Scan 
4. Basic Network Scan 
5. Target 10.1.0.11 Exbihit ***Exhibit 3*** 
6. Credentials - None Exbihit ***Exhibit 4***

### Why This Matters?

You need to set the IP address of the target endpoint for the scan to yield accurate results. You need to leave credentials blank because it is a Unauthenticated Basic Network Scan.

### Exhibit 3

<img width="1907" height="898" alt="lab3" src="https://github.com/user-attachments/assets/7c249c52-3001-44c8-8ef4-279bca686464" />

### Exhibit 4

<img width="1926" height="917" alt="lab4" src="https://github.com/user-attachments/assets/84e5853b-39e4-4ac7-b4fc-ebbb2f96663c" />

---

### Step 4: Review Results

The fourth step was to review the results of the scan. Tenable returned the following results:

| Severity | Vulnerabilities |
|---|---|
| High | 0 |
| Medium | 0 |
| Low | 1 |

The Unauthenticated Basic Network Scan was finished in approximately 6 minutes ***Exibit 5***. The results showed the vulnerabilities that were found ***Exibit 6*** , the description for each vulnerability, the affected assets, the risk information such as CVSS scores and the solution to remediate the vulnerability ***Exhibit 7***.

### Why This Matters?

It is important  to review the results of scans to learn about any possible vulnerabilities an organization  may have and take the necessary steps to implement the organization's **Playbook** if necessary. 

### Exhibit 5

<img width="1918" height="917" alt="lab5" src="https://github.com/user-attachments/assets/b504debe-5e10-4aa9-aa13-e73e97ac45c4" />

### Exhibit 6

<img width="1918" height="920" alt="lab6" src="https://github.com/user-attachments/assets/237b076d-8376-48ac-88c2-1e8b69a078d0" />

### Exhibit 7

<img width="1918" height="918" alt="lab7" src="https://github.com/user-attachments/assets/0c7923c6-28ca-4836-92d3-60d82c508391" />

---

### Step 5: Clean Up

The final step was to perform cleanup by deleting the virtual machine to prevent unnecessary resource usage.

---

## Key Takeaways

- Credentials are not needed to perform a Unauthenticated Basic Network Scan.
- Perform Ping Test in Terminal to ensure connection.
- Unauthenticated Basic Network Scan is not as detailed as a Authenticated Basic Network Scan.
- Always review scan results for possible vulnerabilities.

---

## Conclusion

```
Author        : Manuel Aguirre
LinkedIn      : linkedin.com/in/mannyaguirre/
GitHub        : github.com/mannyaguirre
Date Created  : May 9, 2026
Last Modified : May 9, 2026
Version       : 1.0
