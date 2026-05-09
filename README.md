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


## Key Takeaways

## Conclusion

```
Author        : Manuel Aguirre
LinkedIn      : linkedin.com/in/mannyaguirre/
GitHub        : github.com/mannyaguirre
Date Created  : May 8, 2026
Last Modified : May 8, 2026
Version       : 1.0
