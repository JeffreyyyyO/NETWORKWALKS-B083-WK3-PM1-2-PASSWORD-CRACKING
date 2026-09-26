# **PENETRATION TESTING REPORT**

## PASSWORD CRACKING

W3-PM1 | W3-PM2 | CYBERSECURITY |  NETWORKWALKS

| **Penetration Tester** /(Cybersecurity Professional) | Jeffrey Obi |
| :---- | :---- |
| **Program/Batch** | B083-Networkwalks |
| **Date** | 26 September, 2026 |
| **Modules completed** | W3-PM1: Jack the Ripper (Windows)<br>W3-PM2: Network Walks Tools (Web) |
| **Target Files** | 1\. My Locked PDF1.pdf<br>2\. My Locked PDF2.pdf |
| **Downloads (PDFs)** | ![Full Report](./documents/password_cracking_project_report.pdf) |

# **1\. Liability Disclaimer**

All activities were performed only on the systems & devices where I had secured written permission and on the devices, networks and systems that I own myself. This project was executed for education and research purposes only. Do not use anything from here to break the law. The instructor, the authors and Networkwalks are not responsible for what you do with this knowledge. Every action you take is your own responsibility. Misuse can lead to criminal charges, heavy fines, loss of your job and a permanent record. In most countries unauthorized access is a crime even when nothing is damaged.

# **2\. Introduction**

This report covers footprinting the **networkwalks.com** domain using multiple Kali Linux tools and scanning my own local network with Zenmap. One module covers the footprinting phase and the other covers the scanning phase, so together they show how an attacker moves from gathering public information to mapping live hosts on a network. It is the Week 2 part of my ongoing internship program at Networkwalks.

All commands were run in Kali Linux (footprinting) and on a Windows PC with Zenmap installed (scanning). Every step below includes the exact command used, the result I observed, a screenshot as evidence, and a short note on why the finding matters from an attacker's point of view.

# **3\. Tools Used**

The table below lists each tool used in this report and its purpose.

| Tool | Purpose |
| :---- | :---- |
| **Windows** | Operating systems used for file password cracking activities. |
| **John the Ripper** | Extract hashes and use them to crack passwords. |
| **Network Walks's Hash Calculator** | Hash extraction and password cracking. |
| **Network Walks's Password Cracker** | Crack file passwords using the extracted hash. |
| **GitHub** | Project reporting. |

# **4\. Activities Performed**

## **4.1 Footprinting & Reconnaissance**

I performed reconnaissance against the networkwalks.com domain using six Kali Linux tools: **WHOIS, WhatWeb, Nslookup, Curl, Wafw00f and DNSRecon.** Each tool was used to collect a different type of information about the target.
