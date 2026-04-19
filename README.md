# System-Hardening

Objective

Design and implement a layered system hardening strategy that reduces the attack surface, enforces security policies, and improves system resilience through firewall configuration, operating system hardening, and automation scripting. 

Tools Used

- OPNsense

Methodology

- Captured and analyzed network traffic using packet analysis tools
- Filtered traffic by IP addresses, ports, and protocols to isolate activity
- Examined normal network behavior
- Investigated IDS alerts to identify potentially suspicious connections
- Correlated packet data with alert information to understand network activity patterns

Key Findings

- Identified normal network traffic patterns, including DHCP and broadcast communications
- Detected IDS alerts indicating potential unauthorized connection attempts
- Differentiated between baseline network activity and flagged suspicious behavior

Skills Learned

- Network traffic analysis and packet inspection
- The ability to distinguish normal network patterns from potential security events

<img width="400" height="300" alt="Screenshot 2025-10-16 214624" src="https://github.com/user-attachments/assets/324ec8bd-2b54-484b-8588-25a602e1a228" />
- Configured rules to allow HTTP/HTTPS traffic from WAN to a designated web server while blocking all other inbound HTTP/HTTPS traffic.

<img width="400" height="300" alt="Running Processes bash script Daisy Haas" src="https://github.com/user-attachments/assets/c59d457c-c458-4fb6-9fae-ecb6bec6e122" />
<img width="400" height="500" alt="Screenshot 2025-06-01 090510" src="https://github.com/user-attachments/assets/dcc8af3d-4c04-4312-8d0f-937157e24ed3" />
- Bash-based automation script capturing active system processes with output to a secured log file. File permissions configured to enforce access control within the Linux environment.
