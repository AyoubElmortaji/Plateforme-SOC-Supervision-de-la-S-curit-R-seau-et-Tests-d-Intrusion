# Plateforme-SOC-Supervision-de-la-S-curit-R-seau-et-Tests-d-Intrusion

<img width="1164" height="746" alt="image" src="https://github.com/user-attachments/assets/bce4cf46-92d2-4a96-917d-8ef3e1d38ab4" />

This project focuses on designing and deploying a compact cybersecurity monitoring and detection environment that integrates SOC capabilities with attack simulation across a segmented network.

1. SOC & Monitoring Layer

A SOC Analyst monitors security events using the Wazuh SIEM, which centralizes logs and alerts from all network segments to provide real-time visibility and incident detection.

2. Perimeter Security & IDS

A firewall and Suricata IDS/IPS sensors protect the network perimeter, inspecting traffic and generating alerts for suspicious activities such as scanning, exploitation attempts, or lateral movement.

3. DMZ Environment

The DMZ hosts a Docker-based web server, acting as an internet-facing application for realistic external attack simulations, including reconnaissance and web exploitation.

4. Internal Network (Local Subnet)

An Active Directory Domain Controller manages authentication for four Windows VMs representing employee workstations. These machines serve as targets for phishing and malware-based initial access. A Metasploitable VM is included to practice exploitation, lateral movement, and privilege escalation.

5. Attack Simulation

The environment enables various attack scenarios such as phishing, web exploitation, and internal network compromise, allowing the SOC to observe, detect, and analyze malicious activity end-to-end.
