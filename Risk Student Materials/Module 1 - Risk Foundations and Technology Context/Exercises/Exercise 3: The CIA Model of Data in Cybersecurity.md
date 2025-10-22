## Introduction

While this model focuses on data security, we will be using it frequently in the discussion, labs and case studies in the course

This first exercise is intended to give you some initial practice is risk analysis in an informal manner.

## The CIA Model

Acronym for: confidentiality, integrity, and  availability
- Core framework used to guide the design, implementation, and evaluation of information security controls
- Ensuring that information remains secure, trustworthy, and accessible throughout its lifecycle
- Ensures that data is protected from unauthorized access, remains accurate and unaltered, and is available when and where it’s needed

## Confidentiality: protecting sensitive information

Confidentiality ensures that only authorized people or systems can access specific information
- Protects sensitive data such as customer records, financial statements, and personal information from unauthorized disclosure
- For example:
  - Encryption of customer account data at rest and in transit
  - Limiting database access to authorized personnel
  - Using role-based access control (RBAC) in cloud environments
- Maintaining confidentiality supports trust and compliance, especially with privacy regulations (GDPR, GLBA, HIPAA).

## Integrity: ensuring trustworthy and accurate data

Integrity ensures that data remains complete, correct, and uncorrupted
- Whether stored, transmitted, or processed.
- Prevents malicious or accidental alterations that could cause system errors, fraud, or misinformation
- For example
  - A stock trading system must ensure that transaction data isn’t modified mid-transmission
  - Digital signatures verify that a document hasn’t been tampered with after approval
  - Checksums or hashes confirm that backup files are intact and unaltered
- Ensures that recovery or continuity processes restore accurate information and not corrupted or falsified versions
  - This is essential for maintaining operational trust during and after incidents.
 
## Availability: ensuring reliable access

Availability ensures that authorized users have timely and reliable access to information and systems when needed
- Data is useless if it’s unavailable.
- For example:
  - Redundant data centers and load-balanced web servers
  - Backup power systems and network failover configurations
  - Cloud disaster recovery sites to maintain uptime
- Aligns directly with business continuity and operational resilience
  - Ensures the organization can sustain critical functions even under adverse conditions

---

## Summary
| **Dimension**       | **Definition**                                                                                                                   | **Typical Threats**                                                             | **Example Controls**                                                                              |
|---------------------| -------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- |
| **Confidentiality** | Protecting information from unauthorized access or disclosure.                                                                   | Data breaches, insider leaks, eavesdropping, phishing.                          | Encryption, access controls (RBAC), data classification, multi-factor authentication (MFA), VPNs. |
| **Integrity**       | Ensuring information remains **accurate, consistent, and unaltered** from its original state, except through authorized actions. | Malware, unauthorized modification, data corruption, man-in-the-middle attacks. | Checksums, hashing, digital signatures, version control, audit logs.                              |
| **Availability**    | Ensuring that information and systems are **accessible and usable** by authorized users when needed.                             | DDoS attacks, hardware failure, ransomware, service outages.                    | Redundancy, backups, failover systems, load balancing, disaster recovery plans.                   |


---

## Trade-offs

The CIA elements often exist in some sort of equilibrium
- Strengthening one may impact another, sometimes in unexpected ways
- The balance of these elements are based on business needs and risk appetite

For example:
- Increasing confidentiality: stronger encryption or authentication can slow performance and reduce availability
- Improving availability: can increase exposure and reduce confidentiality
- Enhancing integrity: strict change controls may delay updates, impacting availability

---

## Exercise 3-1:

You are developing a fitness tracking App that has the following functionality:
- Uploads biometric data from a health monitoring wearable (heart rate, respiration, etc.)
- Uses a food diary to record the users calorie, macro and other nutrients
- Produces daily health profiles compared against similar age and gender
- Records data to provide long and short term trend analyses

Do an CIA analysis of the data your app collects and uses

## Exercise 3-2:

As a bank customer, what are your expectations for the CIA model should be implemented by the bank?
- How does this compare with what the bank's expectations might be (make an educated guess)


## Exercise 3-3:

Prepare an analysis of the CIA problems for police databases based on these links (pdfs of these links are in this folder)

[California Law Enforcement Misused State Databases More Than 7,000 Times in 2023](https://www.eff.org/deeplinks/2025/01/california-police-misused-state-databases-more-7000-times-2023)

[Las Vegas SWAT Raid Hits Wrong House During Brothel Bust](https://hoodline.com/2025/08/las-vegas-swat-raid-hits-wrong-house-during-brothel-bust/)

---