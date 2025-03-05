---
layout: default
---

# **Overview**

This project involved setting up a mini Security Operations Center (SOC) environment using Microsoft Azure. The goal was to simulate real-world cybersecurity monitoring by exposing a virtual machine (VM) to public internet traffic, capturing events, and analyzing security logs using Microsoft Sentinel, a cloud-native Security Information and Event Management (SIEM) solution.

![Overview](Screenshot 2025-02-11 012331.png)

# Implementation Details


### Virtual Machine (VM) Deployment & Exposure
*   A Windows-based **VM** was created in Microsoft Azure and configured to allow Remote Desktop Protocol **(RDP)** access from public IP addresses.
*   This setup intentionally exposed the VM to potential security threats to simulate **real-world attack scenarios** and unauthorized access attempts.

### Data Connection to Microsoft Sentinel

*   **Microsoft Sentinel** was used as the **SIEM** platform to aggregate and analyze security logs.
*   A data connector was established between the Azure VM and Sentinel to collect security events, focusing on RDP access logs and user authentication attempts.

### Log Collection and Monitoring

- Configured data collection rules in Sentinel to track and analyze specific security events, including:
  - **Successful & Failed Sign-ins**: Recorded login attempts to identify suspicious activity.
  - **RDP Events**: Logged remote access sessions for threat detection.
  - **Incidents & Alerts**: Used Sentinel’s AI-driven analytics to detect potential security breaches.
- During the testing phase, **more than 1,000 RDP** events were recorded, along with all detected security incidents for analysis.

![Overview](Screenshot 2025-02-11 012504.png)

# Key Metrics & Results

*   Recorded over 1,000 RDP events within the testing period.
*   Successfully detected multiple security incidents related to unauthorized access.
*   Demonstrated real-world cybersecurity monitoring using cloud-based SIEM tools.

# Skills Acquired

*   **Cloud Computing & Virtualization** – Setting up and managing Azure-based virtual machines and networking configurations.
*   **Security Information and Event Management (SIEM) & Log Analysis** – Collecting, analyzing, and monitoring security logs in Microsoft Sentinel.
*   **Cybersecurity & Threat Intelligence** – Detecting threats, monitoring RDP events, and identifying unauthorized access attempts.
*   **Incident Response & Forensics** – Investigating security incidents, applying mitigation techniques, and enforcing security policies.

# **Challenges & Solutions**

## Challenges Faced

*   Managing public RDP exposure while preventing actual compromise.
*   Automating incident detection efficiently.
*   Writing optimized KQL queries for log analysis.

## Solutions Implemented

*   Applied NSG & firewall rules to restrict unwanted traffic.
*   Used Sentinel AI analytics to correlate security events.
*   Developed automation scripts for incident response.

# **Conclusion & Future Enhancements**

### Final Thoughts:
> This project provided hands-on experience in simulating a **real-world SOC environment**, demonstrating the importance of **proactive threat monitoring, incident response, and cloud security strategies** using Microsoft Sentinel and Azure-based SIEM tools. It reinforced key cybersecurity principles, emphasizing the value of log analysis, automation, and continuous security improvements in cloud infrastructure.

## Next Steps:

*   Implement machine learning-based anomaly detection for better threat identification.
*   Integrate Azure Logic Apps for automated incident response workflows.
*   Expand monitoring to include additional security logs (firewall, endpoint security).

## Connect with me:

*   Contact me: fulsundars.omkar@gmail.com
*   Linkedin: [Linkedin]((https://www.linkedin.com/in/omkarfulsundar/)).
