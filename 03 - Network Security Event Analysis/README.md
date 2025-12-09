# Scenario
You are a cybersecurity analyst working for a multimedia company that offers web design services, graphic design, and social media marketing solutions to small businesses. Your organization recently experienced a DDoS attack, which compromised the internal network for two hours until it was resolved.


During the attack, your organization’s network services suddenly stopped responding due to an incoming flood of ICMP packets. Normal internal network traffic could not access any network resources. The incident management team responded by blocking incoming ICMP packets, stopping all non-critical network services offline, and restoring critical network services. 


The company’s cybersecurity team then investigated the security event. They found that a malicious actor had sent a flood of ICMP pings into the company’s network through an unconfigured firewall. This vulnerability allowed the malicious attacker to overwhelm the company’s network through a distributed denial of service (DDoS) attack. 


### To address this security event, the network security team implemented: 

- A new firewall rule to limit the rate of incoming ICMP packets

- Source IP address verification on the firewall to check for spoofed IP addresses on incoming ICMP packets

- Network monitoring software to detect abnormal traffic patterns

- An IDS/IPS system to filter out some ICMP traffic based on suspicious characteristics


As a cybersecurity analyst, you are tasked with using this security event to create a plan to improve your company’s network security, following the National Institute of Standards and Technology (NIST) Cybersecurity Framework (CSF). You will use the CSF to help you navigate through the different steps of analyzing this cybersecurity event and integrate your analysis into a general security strategy. We have broken the analysis into different parts in the template below. You can explore them here:


- Identify security risks through regular audits of internal networks, systems, devices, and access privileges to identify potential gaps in security. 

- Protect internal assets through the implementation of policies, procedures, training and tools that help mitigate cybersecurity threats. 

- Detect potential security incidents and improve monitoring capabilities to increase the speed and efficiency of detections. 

- Respond to contain, neutralize, and analyze security incidents; implement improvements to the security process. 

- Recover affected systems to normal operation and restore systems data and/or assets that have been affected by an incident.

# 03 – Network Security Event Analysis (NIST CSF)

This activity analyzes a Distributed Denial-of-Service (DDoS) security event targeting the internal network of a multimedia company.

#### The goal is to use the NIST Cybersecurity Framework (CSF) to:

- Identify risks that led to the attack

- Protect internal assets

- Detect malicious activity

- Respond effectively

- Recover normal operations

## Security Event Summary

The organization experienced a DDoS attack using a flood of ICMP packets, causing internal network services to stop responding for two hours. Investigation revealed:

- The attacker exploited an unconfigured firewall, allowing unrestricted ICMP traffic.

- The attack overwhelmed internal systems, preventing normal traffic from accessing resources.

- The incident response team mitigated the attack by:

- Blocking incoming ICMP packets

- Disabling non-critical network services

- Restoring critical services
  

After the incident, the network security team implemented:

- ICMP rate-limiting firewall rules

- Source IP address verification

- Network monitoring for abnormal traffic

- IDS/IPS filtering for suspicious ICMP activity

# NIST CSF Analysis
## 1. Identify (What risks existed?)

### Identified weaknesses

- Unconfigured firewall allowed unrestricted ICMP packets

- No defined ICMP traffic policy

- No monitoring for unusual network traffic volumes

- No regular audits of firewall configurations

- Lack of documentation for network service prioritization

### Improvements Needed

- Perform scheduled internal network audits

- Document all firewall rules and verify configurations

- Maintain an updated network asset inventory

- Identify critical systems and map dependencies

- Create a policy for ICMP traffic handling

## 2. Protect (How to prevent this in future?)

### Protective measures

- Implement strict inbound/outbound ICMP traffic policies

- Configure firewall rules to limit ICMP rate

- Apply least privilege to network services

- Provide employee training on DDoS risks and reporting

- Ensure firewall firmware and network devices remain updated

- Harden internal network settings following CIS benchmarks

### Long-term protective controls

- Enforce network segmentation

- Deploy anti-DDoS configurations on perimeter devices

- Restrict access to administrative interfaces

## 🛰️ 3. Detect (How to detect earlier next time?)

### Detection improvements

- Deploy IDS/IPS to detect abnormal ICMP traffic

- Implement continuous network monitoring tools

- Configure alerts for:

  - High ICMP packet volume
  - Repeated requests from suspicious or spoofed IPs
  - Unusual spikes in inbound traffic

- Maintain logs for firewall, IDS/IPS, and network activity

- Enable centralized log management (e.g., SIEM)

## 4. Respond (How to contain and eliminate the threat?)

### Improvements to response capability

- Establish a DDoS-specific incident response procedure

- Maintain a list of steps to isolate affected segments

- Automate blocking rules for suspicious network patterns

- Document the event timeline for future reference

- Include DDoS events in staff training and playbooks

- Create pre-approved emergency firewall rules

### Communication

- Notify IT leadership and stakeholders

- Escalate to external partners if attack volume exceeds capacity

## 5. Recover (How to restore normal operations?)

### Recovery actions

- Restore all network services in priority order

- Validate service functionality after blocking the attack

- Review and apply patches or updated firewall configurations

- Conduct a post-incident review to analyze root cause

- Update policies, training, and configuration based on lessons learned

### Future recovery planning

- Create a DDoS recovery checklist

- Test recovery procedures regularly

- Maintain offline and secure backups of network configurations
