# Snort IDS/IPS Detection and Evasion

This repository contains the detailed project report and configuration files for a Proof of Concept (PoC) demonstrating the capabilities of Snort as an Intrusion Detection System (IDS) and Intrusion Prevention System (IPS) on a Windows 10 host.

The project simulates a real-world scenario where a Windows 10 machine is the protected target and a Kali Linux virtual machine (VM) acts as the attacker. The primary goal is to install and configure Snort on the Windows host to effectively detect and prevent various cyber-attacks originating from the Kali VM.

This PoC offers a comprehensive, hands-on experience, covering a wide range of security activities:

## Project Highlights & Features

  - **Basic Network Monitoring:** Learn to use Snort as a packet sniffer and logger to gain fundamental network visibility and capture traffic for analysis.

  - **Reconnaissance Detection:** Implement rules to identify common reconnaissance techniques, including:

    - *Port Scans:* Detecting various Nmap scan types (SYN, FIN, NULL, XMAS, UDP).

    - *Operating System Fingerprinting:* Identifying attempts to determine the target's OS.

    - *Network Sweeps:* Catching ping sweeps and other network enumeration efforts.

  - **Intrusion Detection System (IDS):** Configure Snort to act as an IDS, leveraging signature-based detection to identify:

    - *Malware Signatures:* Basic detection of malicious file transfers.

    - *Exploit Attempts:* Conceptual detection of common exploit patterns.

    - *Denial-of-Service (DoS) Attacks:* Identifying SYN floods and other DoS indicators.

    - *Protocol Anomalies:* Detecting suspicious behavior within specific protocols (e.g., FTP brute force).

  - **Intrusion Prevention System (IPS):** Transition Snort into an active IPS to block malicious traffic in real-time, demonstrating proactive threat mitigation and policy enforcement.

    - *Custom Rule Creation:* Develop bespoke Snort rules to detect "unknown" or highly specific attack patterns, showcasing the flexibility and extensibility of Snort.

## Repository Contents

  - *`README.md:`* This file, providing an overview of the project.

  - *Project report:* The full, detailed project report outlining the lab setup, Snort configuration steps, specific attack simulations from Kali Linux, and a thorough analysis of Snort's detection and prevention results. This document is designed to be a comprehensive guide and a template for your own security PoCs.

  - *Screenshots:* Screenshots included in report, containing visual evidence of Snort alerts, network logs, and the impact of IPS actions within the lab environment.

  - *`snort.conf:`* The primary Snort configuration file used in this project, with inline comments explaining crucial settings and rule inclusions.

  - *`local.rules:`* A collection of custom Snort rules specifically crafted for this PoC, covering various reconnaissance, intrusion, and prevention scenarios.

  

## Getting Started

To replicate this Proof of Concept in your own lab, you will need the following:

  - **Host Machine:** A computer running Windows 10 (this will be your protected system).

  - **Virtual Machine:** A Kali Linux VM (this will be your attacking system).

  - **Virtualization Software:** Recommended options include VMware Workstation or Oracle VirtualBox.

  - **Snort for Windows:** Download the latest stable installer from the official Snort website.

  - **Npcap:** Install Npcap (recommended over WinPcap) for packet capture, available from the Npcap website.

Follow the detailed, step-by-step instructions provided in the project report file to set up your environment, configure Snort, execute the attack simulations, and analyze the results.

## Disclaimer

This project is developed for educational and demonstration purposes only. It is crucial that you do not perform any of the attack simulations or test any security tools on networks or systems that you do not own or for which you do not have explicit, written permission from the owner. Unauthorized access or testing of computer systems is illegal and unethical.
