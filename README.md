# System Hardening

**Objective**

Design and implement a layered system hardening strategy that reduces the attack surface, enforces security policies, and improves system resilience through firewall configuration, operating system hardening, automation scripting, and implementing least privilege. 

**Tools Used**

- GNS3
- OPNsense
- Greenbone Vulnerability Management

**Environments**

- Virtualized lab environments (VMware-based)
- Linux (Ubuntu)

**Methodology**

This project followed a layered system-hardening and security monitoring approach implemented in a virtualized Linux environment. Security controls were deployed across network and host layers to reduce the attack surface, enforce least privilege, and improve system visibility for security analysis.

1. Network Security Enforcement & Traffic Control: A virtual enterprise network topology was designed and simulated using GNS3, including an edge firewall, internal network segmentation, and a web server. OPNsense Firewall rules were implemented to restrict inbound and lateral traffic to only required services. Rule effectiveness was validated through controlled access testing to confirm enforcement and identify unauthorized access attempts within the environment.
2. System Hardening and Visibility: Bash-based automation scripts were developed to collect and log active system processes, improving host-level visibility into running services. This supported ongoing monitoring of system behavior and helped identify unexpected or unauthorized processes. File permissions and execution controls were enforced to align with least privilege principles and secure script execution.
3. Vulnerability Assessment and Security Validation: Greenbone Vulnerability Management was used to perform vulnerability scans to assess system exposure and validate the effectiveness of implemented security controls. Scan results were analyzed to confirm mitigation of identified risks and to support continuous security posture improvement. User roles and access permissions within the platform were configured to enforce controlled access to security data.

**Validation & Analysis**

To validate the effectiveness of implemented controls, vulnerability scans were compared before and after firewall configuration and system hardening. Exposed services, access paths, and system processes were analyzed to determine whether controls reduced the attack surface and enforced least privilege. This ensured that security improvements were measurable rather than assumed.

**Analyst Decision-Making**

Key decisions made:
- Restricted inbound traffic to only required services (HTTP/HTTPS) to minimize the attack surface
- Used vulnerability scanning to validate controls rather than assuming their effectiveness
- Implemented automation scripts to improve visibility into system activity
- Applied least privilege principles to reduce the risk of unauthorized access

**Key Findings**

- Firewall rule enforcement reduced exposed services from multiple open ports to only HTTP/HTTPS (80/443), significantly limiting external access to required services
- Bash automation scripts provided consistent visibility into active system processes, supporting system auditing and validation of authorized services
- File permission controls prevented unauthorized file modification
- Initial vulnerability scans identified multiple exposed services and configuration risks, including unnecessary open ports and broader access paths
- After implementing firewall rules and system hardening controls, subsequent scans confirmed a reduced attack surface, with fewer exposed services and improved access restrictions
- A layered security approach provided a stronger security posture than any single control

**Skills Demonstrated**

1. Design - Network topology design, segmentation planning, firewall placement, and lab simulation
2. Protection - Firewall rule configuration, traffic filtering, least privilege design, and traffic control
3. Hardening - Linux system hardening, file permission management, bash scripting for automation, process auditing and system monitoring, secure script execution
4. Validation - Vulnerability scanning and analysis, security control validation, residual risk identification, scan result analysis, verification of firewall effectiveness

<img width="400" height="300" alt="firewall" src="https://github.com/user-attachments/assets/2edf0aae-b0b4-43a1-8462-78a51e5d10ea" />
<img width="400" height="300" alt="Screenshot 2025-10-16 214624" src="https://github.com/user-attachments/assets/324ec8bd-2b54-484b-8588-25a602e1a228" />

- Configured and validated edge firewall rules to restrict inbound traffic to only HTTP/HTTPS (80/443) for a designated web server, while blocking all other unsolicited external requests. Traffic filtering was tested to confirm that only explicitly permitted services were accessible, reducing the external attack surface.

<img width="400" height="300" alt="Running Processes bash script Daisy Haas" src="https://github.com/user-attachments/assets/c59d457c-c458-4fb6-9fae-ecb6bec6e122" />
<img width="400" height="200" alt="Screenshot 2025-10-08 211419" src="https://github.com/user-attachments/assets/1e107ae9-c6de-4a3c-9d71-f64579ee3222" />

- Developed and executed a Bash-based automation script to collect and log active system processes, enabling continuous visibility into system activity. Output logs were reviewed to validate running services and identify any unauthorized or unexpected processes. File permissions and execution controls were applied to ensure secure script usage.

<img width="600" height="300" alt="Greenbone" src="https://github.com/user-attachments/assets/438d8617-76da-46a7-bbba-beef84bb86e1" />

- Configured role-based access controls within Greenbone Vulnerability Management to enforce least privilege and restrict administrative actions to authorized users and IP ranges. Vulnerability scan results were analyzed to validate the effectiveness of implemented firewall and system hardening controls and to identify residual risks.
