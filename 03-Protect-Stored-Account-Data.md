# PCI DSS Requirement 3
## Protect Stored Account Data

### Objective

The objective of Requirement 3 is to protect stored account data and reduce the risk associated with storing payment card information.

A key principle is:

> If account data is not needed, do not store it.

PCI DSS emphasizes limiting stored account data to what is necessary for business, legal, or regulatory purposes.

---

## What is Account Data?

Account data includes:

### Cardholder Data (CHD)

Examples include:

- Primary Account Number (PAN)
- Cardholder name
- Expiration date
- Service code

### Sensitive Authentication Data (SAD)

Examples include:

- Full track data
- Card verification codes/values
- PINs and PIN blocks

---

## Requirement 3.1 — Protect Stored Account Data

Organizations should define and maintain processes for protecting stored account data.

Relevant policies and procedures should be:

- Documented
- Kept up to date
- In use
- Known to affected personnel

Roles and responsibilities should also be documented and assigned.

---

## Data Retention and Minimization

Organizations should limit the amount of stored account data and retain it only for as long as required for:

- Business purposes
- Legal requirements
- Regulatory requirements

When data is no longer required, it should be securely deleted or rendered unrecoverable.

### Example

If a company only needs the last four digits of a card number for customer support, storing the full PAN creates unnecessary risk.

Data minimization can therefore reduce both security risk and PCI DSS scope.

---

## Sensitive Authentication Data (SAD)

Sensitive Authentication Data must not be retained after authorization.

This includes data such as:

- Full track data
- Card verification codes/values
- PIN data

Encryption does not make post-authorization storage of prohibited SAD acceptable.

---

## Protecting PAN

When PAN is stored, PCI DSS requires it to be rendered unreadable using an applicable protection method.

Examples can include:

- Strong cryptography
- Truncation
- Tokenization
- One-way hashing

The appropriate method depends on the business and technical requirements.

---

## PAN Display

When PAN is displayed, it should be masked so that only authorized personnel with a legitimate business need can view the required information.

### Example

Instead of displaying:

`4111111111111111`

A system may display:

`411111******1111`

The exact masking requirements must be evaluated against the applicable PCI DSS requirement and business need.

---

## Encryption

Encryption can be used to protect stored account data.

Encryption converts:

**Plaintext → Ciphertext**

Only an authorized party with the appropriate cryptographic key should be able to recover the original data.

---

## Key Management

Encryption alone is not enough.

Organizations also need appropriate processes for managing cryptographic keys.

Examples include:

- Key generation
- Key storage
- Key access control
- Key rotation
- Key retirement
- Protection against unauthorized disclosure

---

## Where Stored Account Data May Exist

Account data may exist in many locations, including:

- Databases
- Application servers
- Backup systems
- Logs
- Portable storage
- Cloud storage
- Paper records
- Images or scanned documents

All relevant storage locations need to be considered when assessing the protection of account data.

---

## Example Control

### Control

The organization shall minimize stored PAN and protect stored PAN using an approved method that renders it unreadable.

### Possible Evidence

- Data retention policy
- Data flow diagrams
- Database configuration
- Encryption configuration
- Tokenization documentation
- Key management procedures
- Database screenshots
- Data deletion records
- Access control records

---

## GRC / Audit Perspective

For Requirement 3, an auditor should not only ask:

> "Is the data encrypted?"

The assessment should also consider:

- Why is the data being stored?
- How long is it retained?
- Where is it stored?
- Is PAN rendered unreadable?
- Is prohibited SAD being retained?
- Who can access it?
- How are encryption keys managed?
- Is unnecessary data securely deleted?

---

## Example Risk Scenario

### Scenario

A company stores complete card numbers in an old database even though the application only needs the last four digits.

### Risk

If the database is compromised, attackers could obtain unnecessary payment account data.

### GRC Recommendation

- Identify the business requirement.
- Determine whether full PAN is actually necessary.
- Minimize stored data.
- Protect required PAN appropriately.
- Securely delete unnecessary data.
- Document retention requirements.

---

## Interview Questions

### Q1. What is the main objective of PCI DSS Requirement 3?

To protect stored account data and minimize unnecessary storage of payment account information.

### Q2. Can Sensitive Authentication Data be stored after authorization if it is encrypted?

No. PCI DSS Requirement 3.3.1 prohibits retaining SAD after authorization, even if encrypted.

### Q3. Does PCI DSS require every piece of cardholder data to be encrypted?

No. PAN must be rendered unreadable when stored, while other cardholder data elements have different protection requirements depending on how they are stored, processed, or transmitted.

### Q4. Why is data minimization important?

Storing unnecessary account data increases the potential impact of a compromise and can increase the organization's security and compliance burden.

---

## GRC / Audit Evidence Checklist

| Evidence | Purpose |
|---|---|
| Data Retention Policy | Demonstrates retention requirements |
| Data Flow Diagram | Identifies where account data moves |
| Data Inventory | Identifies stored account data |
| Database Configuration | Demonstrates protection of stored data |
| Encryption Evidence | Demonstrates unreadability mechanisms |
| Key Management Documentation | Demonstrates cryptographic key controls |
| Deletion Records | Demonstrates secure disposal |
| Access Review | Demonstrates restricted access |

---

## Key Takeaways

- Minimize stored account data.
- Retain data only when there is a legitimate requirement.
- Do not retain prohibited SAD after authorization.
- PAN must be rendered unreadable when stored.
- Consider databases, backups, logs, cloud storage, and physical records.
- Encryption requires appropriate key management.
- Securely delete data when it is no longer required.
- Maintain documentation and evidence for assessment.

---

## Reference

PCI Security Standards Council — PCI DSS

https://www.pcisecuritystandards.org/standards/pci-dss/

PCI SSC FAQ — Cardholder Data Protection:

https://www.pcisecuritystandards.org/faqs/1222/

PCI SSC FAQ — Data Retention:

https://www.pcisecuritystandards.org/faqs/1318/

These notes are for personal learning purposes and contain no confidential company or client information.
