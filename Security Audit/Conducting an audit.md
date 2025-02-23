# Security Audit -- Botium Toys

## Case Study

This is based on a fictional company:

Botium Toys is a small U.S. business that develops and sells toys. The business has a single physical location, which serves as their main office, a storefront, and warehouse for their products. However, Botium Toy’s online presence has grown, attracting customers in the U.S. and abroad. As a result, their information technology (IT) department is under increasing pressure to support their online market worldwide. 

The manager of the IT department has decided that an internal IT audit needs to be conducted. She expresses concerns about not having a solidified plan of action to ensure business continuity and compliance, as the business grows. She believes an internal audit can help better secure the company’s infrastructure and help them identify and mitigate potential risks, threats, or vulnerabilities to critical assets. The manager is also interested in ensuring that they comply with regulations related to internally processing and accepting online payments and conducting business in the European Union (E.U.).   

The IT manager starts by implementing the National Institute of Standards and Technology Cybersecurity Framework (NIST CSF), establishing an audit scope and goals, listing assets currently managed by the IT department, and completing a risk assessment. The goal of the audit is to provide an overview of the risks and/or fines that the company might experience due to the current state of their security posture.

Your task is to review the IT manager’s scope, goals, and risk assessment report. Then, perform an internal audit by completing a controls and compliance checklist. 

## Scenario
Botium Toys: Scope, Goals, and Risk Assessment Report

### Scope 

The scope is defined as the entire security program at Botium Toys. This means all assets need to be assessed alongside internal processes and procedures related to the implementation of controls and compliance best practices.

### Goals
Assess existing assets and complete the controls and compliance checklist to determine which controls and compliance best practices need to be implemented to  improve Botium Toys’ security posture.

### Current assets
Assets managed by the IT Department include: 
* On-premises equipment for in-office business needs
* Employee equipment: end-user devices (desktops/laptops, smartphones), remote workstations, headsets, cables, keyboards, mice, docking stations, surveillance cameras, etc.
* Storefront products available for retail sale on site and online; stored in the company’s adjoining warehouse
* Management of systems, software, and services: accounting, telecommunication, database, security, ecommerce, and inventory management
* Internet access
* Internal network
* Data retention and storage
* Legacy system maintenance: end-of-life systems that require human monitoring 

### Risk assessment

#### Risk description
Currently, there is inadequate management of assets. Additionally, Botium Toys does not have all of the proper controls in place and may not be fully compliant with U.S. and international regulations and standards. 

#### Control best practices
The first of the five functions of the NIST CSF is Identify. Botium Toys will need to dedicate resources to identify assets so they can appropriately manage them. Additionally, they will need to classify existing assets and determine the impact of the loss of existing assets, including systems, on business continuity.

#### Risk score
On a scale of 1 to 10, the risk score is 8, which is fairly high. This is due to a lack of controls and adherence to compliance best practices.

#### Additional comments
The potential impact from the loss of an asset is rated as medium, because the IT department does not know which assets would be at risk. The risk to assets or fines from governing bodies is high because Botium Toys does not have all of the necessary controls in place and is not fully adhering to best practices related to compliance regulations that keep critical data private/secure. Review the following bullet points for specific details:

## Controls Assessment Checklist

Does Botium Toys currenly have this control in place? 

| Yes / No / ? | Control | Explanation |
| :-------        |    :---:   | :---     |
| No | Least Privilige | Currently employees have access to customer data, this is problematic and can lead to breaches, SPII and PII are vulnerable |
| No | Disaster Recovery Plan | Currently, there is no plan for handling disaster. This needs to be created to ensure business continuity. |
| Yes | Firewall | The organization has a firewall to block traffic based on an appropriately defined set of security rules. |
| No | Password policies | Password policy exists, yet the requirements are considered weak and put the identity management access at risk. Additionally, a centeralized password management system is required for password recovery and resetting in case of any breach |
| Yes | Antivirus | The antivirus software is active and regulary monitored by IT team. |
| No | Backups | This is as same as disaster recovery plan. They are not prepared in the case of breach. They have to implement the backup plan, such as incremental, full, or partial. |
| No | Encryption | Currently there no encryption used in storing sensitive data like credit card details or other SPII, this needs to be fixed |
| No | IDS | This is crucial if the company is exapanding, security team needs to to have an eye on the systems | 
| Yes | Storefront| Although IT team is not responsible for the management at the storefront, however the organization should have sufficient locks.|
| Yes | CCTV | It is working as intended. |
| Yes | Fire detection | The organization has these. However, the team should maintain it and establish a plan on how to use it. |
| No | Separation of duties | Company CEO runs day to day operations and manages payroll. This needs to change |

## Compliance Checklist
Does Botium Toys currenly adhrere to this compliance best practice? 

* Payment Card Industry Data Security Standard (PCI DSS)

| Yes/ No / ? | Best Practice | Explanation |
| :---        |    :---:   | :---     |
| No | Only authorized users have access to customers’ credit card information.  | At the moment, all employees have access to it which is a bad practice in the business.  |
| No | Credit card information is stored, accepted, processed, and transmitted internally, in a secure environment. | Credit card info is stored with encryption. This is a gross violation of SPII and PII that can affect customers privacy and can open your company to fines or class-action lawsuits inj the future |
| No | Implement data encryption procedures to better secure credit card transaction touchpoints and data. | No, there is no encryption systems in place, data is not secure in case of a breach. | 
| No | Adopt secure password management policies. | Password policy not in line with minimal requirements. Centralized Password management is also required at this point |

* GDPR
  
| Yes/ No / ? | Best Practice | Explanation |
| :---        |    :---:   | :---     |
| No | EU customers are kept secured. | The organization does not apply GDPR practice. Thus, it puts them at risk of being fined by the EU government. |
| Yes | Enforce privacy policies, procedures, and processes to properly document and maintain data.| According to the scenario, it has been enforced by the IT Team members and other staff. |
| Yes | There is a plan in place to notify E.U. customers within 72 hours if their data is compromised/there is a breach. | The organization does have this in place |
| No | Ensure data is properly classified and inventoried. | This is not in place, data needs proper classification and there should be proper distinction between SPII and PII data access, even to internal employees. Backups are also not available |


* System and Organizations Controls 

| Yes/ No / ? | Best Practice | Explanation |
| :---        |    :---:   | :---     |
| No | User access policies are established | Currently internal stakeholders have access to sensitive SPII and PII of customers, this is a gross violation and needs to be fixed switly. |
| No | Data integrity ensures the data is consistent, complete, accurate, and has been validated. | Backups are not available and no disaster recovery plans exist at the moment| 
| No | Data is available to individuals authorized to access it. | Currently, since no access policy is in place, employees are able to access SPII and PII |
| No | Sensitive data (PII/SPII) is confidential/private. | It is not private at the movement, since employees can access customer SPII and PII.

## Recommendations 

After researching Botium Toys's security posture, the analysts agreed that the security practice is far from the expectation. It lacks of protection of confidentialiy of sensitive information. The following are:
1. Least privilege
2. Disaster recovery plan
3. Access levels
4. Password policies
5. Centralized password management
6. Backup solutions
7. Encryption systems.

Firstly, Botium should create access levels to maintain data confidentiality. Botium should also be looking into maintaining backups (full or partial) to ensure data loss in case of a ransomware attack. 
Periodic password resetting should become a norm. Employees are needed to be trained on secure practices. SPII should be encrupted by all means. The company also needs to properly classify assets, to identify additional controls that may need to be implemented to
improve their security posture and better protect sensitive information.
