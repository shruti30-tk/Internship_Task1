# Task 1 
This repository contains all the submission material regarding task 1 for the internship.

## Task: Scan Your Local Network for Open Ports
- Objective: Learn to discover open ports on devices in your local network to understand network exposure.
- Tools: Nmap (free), Wireshark (optional)
Steps
1. I was working on **Windows**, so I downloaded and installed **Nmap** from the official website: [Nmap Download](https://nmap.org/download.html). The installation includes both the command-line tool and the **Zenmap GUI** for easier use.
2. To find the IP address for my local network, I opened **Command Prompt** and ran the command `ipconfig`. This provided me with the IP address and network range, including the IPv4 address. From there, I was able to identify my subnet (e.g., `192.168.0.0/24`).
![Screenshot 2025-06-23 191452](https://github.com/user-attachments/assets/5ece2fee-1e98-4d02-90c8-c095a7ae1040)
3. I then ran the help command to familiarize myself with Nmap’s options: `nmap -h`.
4. Based on the context, I selected the following Nmap scan options:
   * `-sS`: To perform a stealth SYN scan.
   * `-Pn`: To skip host discovery (useful if ping responses are blocked).
   * `-p-`: To scan all 65535 ports.
   * `-oN`: To save the results in a standard text file format.
   ![image](https://github.com/user-attachments/assets/4c045b55-a284-4219-8f9e-e3797e97ba4e)
 5. Once the scan was complete, I reviewed the output file (`scan_results.txt`) to examine the results.
6. After analyzing the open ports, I looked into the **security risks** associated with those services. The detailed risk assessment can be found in the `Risk_Assessed` file.

### Outcome : By completing this task, I learned how to:
- Find devices on my local network  
- Detect open ports and their services  
- Identify basic security risks from exposed or unknown ports

Conclusion:
This exercise provided hands-on experience with an essential part of cybersecurity — scanning networks. With Nmap, I was able to explore my local network, spot open services, and understand potential security vulnerabilities.
