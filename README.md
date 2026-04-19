# System-Hardening

Objective

Design and implement a layered system hardening strategy that reduces the attack surface, enforces security policies, and improves system resilience through firewall configuration, operating system hardening, automation scripting, and implementing least privilege. 

Tools Used

- GNS3
- OPNsense
- Greenbone Vulnerability Management

Environments

- Linux (Ubuntu)

Methodology

- This project followed a layered system hardening approach implemented within a virtualized Linux environment. Security controls were applied incrementally across network and host layers to reduce the attack surface and enforce least privilege.
1. Network Security Enforcement: A virtual network topology was designed and simulated using GNS3 to replicate an enterprise environment, including an edge firewall, internal segmentation, and web server. Firewall rules were configured using OPNsense to restrict inbound traffic, allowing only required services while blocking unauthorized access attempts.
2. System Automation & Hardening: Developed Bash-based automation scripts to validate running services and export logs for security audits. File permissions and execution controls were applied within the Linux environment.
3. Vulnerability Assessment & Validation: Performed vulnerability scans using Greenbone Vulnerability Management to validate the effectiveness of implemented firewall and system hardening controls. Configured platform user roles and permissions to support controlled access.

Key Findings

- Firewall rule enforcement significantly reduced exposed network services, limiting external access to only explicitly permitted traffic.
- Linux-based automation scripts improved visibility into active system processes.
- File permission controls prevented unauthorized file modification.
- Greenbone scans identified residual configuration risks, highlighting the importance of continuous security validation.
- A layered security approach provided stronger security posture than any single control.

Skills Learned
1. Design - Network topology design, segmentation planning, firewall placement, lab simulation.
2. Protection - Firewall rule configuration, traffic filtering, least privilege design, traffic control.
3. Hardening - Linux system hardening, file permission management, bash scripting for automation, process auditing and system monitoring, secure script execution.
4. Validation - Vulnerability scanning and analysis, security control validation, residual risk identification, scan result analysis, verification of firewall effectiveness.

<img width="400" height="300" alt="firewall" src="https://github.com/user-attachments/assets/2edf0aae-b0b4-43a1-8462-78a51e5d10ea" />
<img width="400" height="300" alt="Screenshot 2025-10-16 214624" src="https://github.com/user-attachments/assets/324ec8bd-2b54-484b-8588-25a602e1a228" />

- Set up an edge firewall on the network and configured rules to allow HTTP/HTTPS traffic from WAN to a designated web server while blocking all other inbound HTTP/HTTPS traffic.

<img width="400" height="300" alt="Running Processes bash script Daisy Haas" src="https://github.com/user-attachments/assets/c59d457c-c458-4fb6-9fae-ecb6bec6e122" />
<img width="400" height="200" alt="Screenshot 2025-10-08 211419" src="https://github.com/user-attachments/assets/1e107ae9-c6de-4a3c-9d71-f64579ee3222" />

- Bash-based automation script capturing active system processes with output to a log file. Execution permissions were configured and script output was validated to confirm successful data capture in a Linux environment.

<img width="600" height="300" alt="Greenbone" src="https://github.com/user-attachments/assets/438d8617-76da-46a7-bbba-beef84bb86e1" />

- Configured access control and permissions within Greenbone Vulnerability Management to enforce the least privilege principle and restrict administrative functions to authorized users and IP address ranges.
