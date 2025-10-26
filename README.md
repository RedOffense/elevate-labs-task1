# Gogulothu sai / Task1 scan-Your-local-Network For Open-Port

# Nmap Local Network Scanning Task

# Task Overview

This task involves scanning the local network using Nmap to discover active devices, open ports, and running services.
The goal is to understand the basics of network reconnaissance and potential security risks.

# Tools Used

Nmap (Network Mapper) → https://nmap.org/download.html

Wireshark (Optional for packet analysis) → https://www.wireshark.org/

 # Steps Followed

 **1. Install Nmap**
 
 Windows: Download installer from Nmap.org and install with default settings.
 
Linux (Ubuntu/Debian):

       sudo apt update && sudo apt install nmap -y

# Identify Local IP Range

Windows:

      ipconfig

Linux (Ubuntu/Debian):

          ifconfig
              #or 
            ip a
            
Run TCP SYN Scan:

     nmap -sS 192.168.1.0/24

            -sS → Stealth SYN scan
             192.168.1.0/24 → Scan all IPs in the subnet

# Analyze Results             

Example Output:


     Starting Nmap 7.97 ( https://nmap.org ) at 2025-08-04 12:16 +0530
     NSE: Loaded 158 scripts for scanning.
     NSE: Script Pre-scanning.
     Initiating NSE at 12:16
    Completed NSE at 12:16, 0.00s elapsed
    Initiating NSE at 12:16
    Completed NSE at 12:16, 0.00s elapsed
    Initiating NSE at 12:16
    Completed NSE at 12:16, 0.00s elapsed
    Initiating Ping Scan at 12:16
    ...
    > *(The scan continues showing discovered hosts and their open ports.)*
