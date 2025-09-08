Mini SIEM Lab

A lightweight, all-in-one Security Operations Center (SOC) lab for threat hunting and log analysis. This project integrates Suricata (IDS/IPS), Zeek (network analysis), Fluent Bit (log shipper), and OpenSearch into a functional mini-SIEM.

Overview
This lab is designed to collect, process, and visualize security-relevant data on a single Ubuntu server. It's ideal for learning about network security monitoring, log analysis, and threat hunting in a controlled environment.

Core Components:

Suricata: Generates JSON-based security alerts from network traffic.

Zeek: Provides rich, protocol-level network logs.

Fluent Bit: Collects and ships logs to OpenSearch.

OpenSearch: Stores and indexes all logs.

OpenSearch Dashboards: Provides a web interface for visualizing and analyzing the data.

Prerequisites
OS: Ubuntu Server (22.04 or 24.04 LTS)

Resources: Minimum 2 vCPUs, 4 GB RAM (8 GB recommended)

Network: Bridged adapter mode to monitor network traffic.

Access: sudo privileges.

Quick Start (Summary)
Update System: sudo apt update && sudo apt -y upgrade

Install Suricata: Install from APT, configure interface, and update rules.

Install Zeek: Build from source for the latest features.

Install Fluent Bit: Use the official script, configure to tail Suricata/Zeek logs.

Install OpenSearch: Tarball installation with security disabled for the lab.

Install Dashboards: Tarball installation; remove the security plugin.

Generate Test Traffic: Use nmap or curl to create logs and alerts.

Visualize: Access Dashboards at http://<your-server-ip>:5601.

Detailed Installation Guide
The quick start commands are a high-level summary. For the complete, step-by-step guide with detailed explanations for every command, please see the comprehensive documentation file: T hunt.docx.

This in-depth guide includes:

Copy-paste ready commands with explanations.

Crucial configuration file snippets.

Common pitfalls and how to avoid them.

Troubleshooting tips for each component.

Important security notes for lab isolation.

Important Note
This lab setup disables security features for simplicity and is intended for isolated, private networks only. Never expose this environment to the internet.

License
This project is provided for educational purposes.
