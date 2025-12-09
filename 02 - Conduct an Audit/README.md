# Case Study (based on a fictional company)
## Botium Toys: Scope, goals, and risk assessment report

### Scope and goals of the audit
**Scope:** The scope is defined as the entire security program at Botium Toys. This means all assets need to be assessed alongside internal processes and procedures related to the implementation of controls and compliance best practices.

**Goals:** Assess existing assets and complete the controls and compliance checklist to determine which controls and compliance best practices need to be implemented to  improve Botium Toys’ security posture.

### Current assets:
#### Assets managed by the IT Department include: 

- On-premises equipment for in-office business needs  

- Employee equipment: end-user devices (desktops/laptops, smartphones), remote workstations, headsets, cables,         keyboards, mice, docking stations, surveillance cameras, etc.

- Storefront products available for retail sale on site and online; stored in the company’s adjoining warehouse

- Management of systems, software, and services: accounting, telecommunication, database, security, ecommerce, and inventory management

- Internet access

- Internal network

- Data retention and storage

- Legacy system maintenance: end-of-life systems that require human monitoring 

### Risk assessment
#### Risk description:

Currently, there is inadequate management of assets. Additionally, Botium Toys does not have all of the proper controls in place and may not be fully compliant with U.S. and international regulations and standards. 

#### Control best practices
The first of the five functions of the NIST CSF is Identify. Botium Toys will need to dedicate resources to identify assets so they can appropriately manage them. Additionally, they will need to classify existing assets and determine the impact of the loss of existing assets, including systems, on business continuity.

#### Risk score
On a scale of 1 to 10, the risk score is 8, which is fairly high. This is due to a lack of controls and adherence to compliance best practices.

#### Additional comments
The potential impact from the loss of an asset is rated as medium, because the IT department does not know which assets would be at risk. The risk to assets or fines from governing bodies is high because Botium Toys does not have all of the necessary controls in place and is not fully adhering to best practices related to compliance regulations that keep critical data private/secure. Review the following bullet points for specific details:

- Currently, all Botium Toys employees have access to internally stored data and may be able to access cardholder data and customers’ PII/SPII.

- Encryption is not currently used to ensure confidentiality of customers’ credit card information that is accepted, processed, transmitted, and stored locally in the company’s internal database. 
	
- Access controls pertaining to least privilege and separation of duties have not been implemented.
	
- The IT department has ensured availability and integrated controls to ensure data integrity.
	
- The IT department has a firewall that blocks traffic based on an appropriately defined set of security rules.
	
- Antivirus software is installed and monitored regularly by the IT department. 
	
- The IT department has not installed an intrusion detection system (IDS).
	
- There are no disaster recovery plans currently in place, and the company does not have backups of critical data. 
	
- The IT department has established a plan to notify E.U. customers within 72 hours if there is a security breach. Additionally, privacy policies, procedures, and processes have been developed and are enforced among IT department members/other employees, to properly document and maintain data.
	
- Although a password policy exists, its requirements are nominal and not in line with current minimum password complexity requirements (e.g., at least eight characters, a combination of letters and at least one number; special characters). 
	
- There is no centralized password management system that enforces the password policy’s minimum requirements, which sometimes affects productivity when employees/vendors submit a ticket to the IT department to recover or reset a password.
	
- While legacy systems are monitored and maintained, there is no regular schedule in place for these tasks and intervention methods are unclear.
	
- The store’s physical location, which includes Botium Toys’ main offices, store front, and warehouse of products, has sufficient locks, up-to-date closed-circuit television (CCTV) surveillance, as well as functioning fire detection and prevention systems.

# 02 – Conduct an Audit (Controls & Compliance Checklist)

This activity demonstrates how to perform an internal security audit for Botium Toys, a fictional U.S. toy company expanding its online operations.
The audit is based on the NIST Cybersecurity Framework (CSF) and evaluates:

- Existing administrative, technical, and physical controls

- PCI DSS, GDPR, and SOC 1/SOC 2 compliance gaps

- Risks related to the company’s infrastructure

- Recommendations to improve security posture


## 1. Controls Assessment Checklist

| Control                                   | Implemented? | Notes                                                          |
| ----------------------------------------- | ------------ | -------------------------------------------------------------- |
| **Least Privilege**                       | ❌ No         | No formal access control or privilege policy exists.           |
| **Disaster Recovery Plans**               | ❌ No         | No documented DR or business continuity plan.                  |
| **Password Policies**                     | ❌ No         | No defined password rules or complexity requirements.          |
| **Separation of Duties**                  | ❌ No         | Small team; roles overlap and create risk.                     |
| **Firewall**                              | ✔️ Yes        | Basic firewall likely present as part of network setup.        |
| **Intrusion Detection System (IDS)**      | ❌ No         | No monitoring or alerting technology in place.                 |
| **Backups**                               | ❌ No         | No formalized backup or recovery strategy documented.          |
| **Antivirus Software**                    | ✔️ Yes        | Standard AV installed on internal systems.                     |
| **Manual Monitoring (Legacy Systems)**    | ✔️ Yes        | Team relies on manual checks due to lack of automation.        |
| **Encryption**                            | ❌ No         | No encryption mentioned for payment or sensitive data.         |
| **Password Management System**            | ❌ No         | No central password vault or credential tool.                  |
| **Locks (Storefront, Office, Warehouse)** | ✔️ Yes        | Physical access control through basic locks.                   |
| **CCTV Surveillance**                     | ❌ No         | No mention of surveillance or monitoring cameras.              |
| **Fire Detection / Prevention**           | ✔️ Yes        | Standard fire detection systems expected at physical location. |

## 2. Compliance Assessment Checklist

### PCI DSS
| Best Practice                                 | Implemented? | Notes                                              |
| --------------------------------------------- | ------------ | -------------------------------------------------- |
| Only authorized users access credit card data | ❌ No         | No access control or authorization rules.          |
| Credit card data stored/processed securely    | ❌ No         | Manager explicitly worried about payment security. |
| Data encryption for card transactions         | ❌ No         | No encryption controls in place.                   |
| Secure password management policies           | ❌ No         | No documented password policy.                     |

### GDPR
| Best Practice                            | Implemented? | Notes                                      |
| ---------------------------------------- | ------------ | ------------------------------------------ |
| EU customer data kept private/secure     | ❌ No         | No GDPR compliance program.                |
| Breach notification plan within 72 hours | ❌ No         | No incident response or IR plan mentioned. |
| Proper data classification and inventory | ❌ No         | No structured data governance.             |
| Privacy policies and enforcement         | ❌ No         | No defined privacy rules or procedures.    |

### SOC 1 / SOC 2
| Best Practice                          | Implemented? | Notes                                        |
| -------------------------------------- | ------------ | -------------------------------------------- |
| User access policies established       | ❌ No         | No defined IAM or access policy.             |
| Sensitive data (PII/SPII) confidential | ❌ No         | Missing encryption, policy, and safeguards.  |
| Data integrity ensured                 | ❌ No         | No validation or audit controls.             |
| Data available to authorized users     | ✔️ Yes        | Systems function but lack security controls. |

## 3. Summary & Recommendations

Based on the audit, Botium Toys lacks many foundational administrative, technical, and compliance controls required to safely operate, scale internationally, and process online payments.

Key Recommendations:

### 🔐 Administrative Controls

- Implement least privilege and role-based access control (RBAC).

- Create a formal password policy and enforce MFA.

- Establish separation of duties between IT, finance, and operations.

### 🖥️ Technical Controls

- Deploy IDS/IPS for threat detection.

- Encrypt all sensitive and payment-related data.

- Implement automated backups with off-site redundancy.

- Adopt a password management system (e.g., Bitwarden, 1Password).

### 🏢 Physical & Operational Controls

- Add CCTV surveillance in office, storefront, and warehouse areas.

- Document fire safety procedures and test systems regularly.

### 📜 Compliance Requirements

- Establish PCI DSS controls for secure card handling.

- Implement GDPR-compliant privacy and breach notification processes.

- Align internal procedures with SOC 1/SOC 2 principles.

