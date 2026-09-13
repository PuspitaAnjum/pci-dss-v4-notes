# PCI DSS Requirement 12 — Support Information Security with Organizational Policies and Programs

## 🎯 Objective

Requirement 12 focuses on the organization's overall security governance.

It ensures that cybersecurity is supported through:

- Information security policies
- Acceptable use policies
- Risk management
- PCI DSS compliance management
- Scope management
- Security awareness
- Personnel screening
- Third-party risk management

---

# 12.1 — Information Security Policy

The organization must maintain a comprehensive information security policy that:

- Governs information security
- Provides direction for protecting information assets
- Is known and current

## 12.1.1 — Policy Review

The information security policy must be reviewed at least annually and updated when the environment changes.

### Example

If the organization introduces:

- Cloud services
- Remote work
- New payment systems
- New security technologies

the security policy may need to be updated.

---

# 12.2 — Acceptable Use Policies

Organizations must define and implement acceptable use policies for end-user technologies.

### Examples

The policy may address:

- Company laptops
- Mobile devices
- Internet usage
- Email
- Cloud services
- USB devices
- Personal devices

### Example

Employees may not:

- Install unauthorized software
- Share company credentials
- Upload confidential data to unauthorized services

---

# 12.3 — Targeted Risk Analysis

Risks to the CDE must be formally:

- Identified
- Evaluated
- Managed

Targeted risk analysis is used where PCI DSS allows the organization to determine a frequency or methodology based on its own risk assessment.

### Example

Requirement says an activity must occur at a frequency determined by targeted risk analysis.

The organization should document:

1. Asset/process
2. Threat
3. Vulnerability
4. Impact
5. Likelihood
6. Risk level
7. Selected frequency
8. Justification

---

# 12.4 — PCI DSS Compliance Management

The organization must manage PCI DSS compliance.

This includes defining:

- Responsibility
- Accountability
- Compliance activities
- Assessment processes

### Example

A PCI DSS compliance program may include:

Compliance Manager → overall coordination

IT → technical controls

Security → monitoring

HR → personnel processes

Legal → contractual requirements

---

# 12.5 — PCI DSS Scope

PCI DSS scope must be:

- Documented
- Validated

### Important Concept

Scope determines which:

- Systems
- Networks
- Applications
- People
- Processes

are included in the PCI DSS assessment.

### Example

If a payment application connects directly to the CDE, it may be in scope.

If a properly segmented HR network cannot impact the CDE, it may potentially be out of scope.

But the organization must demonstrate and validate the segmentation/scoping decision.

---

# 12.6 — Security Awareness

Security awareness education must be an ongoing activity.

Employees should understand their security responsibilities.

### Topics may include

- Phishing
- Password security
- Social engineering
- Handling cardholder data
- Incident reporting
- Acceptable use
- Physical security

---

# 12.6.1 — Security Awareness Program

The organization must maintain a security awareness program.

### Example

New employee:

Security awareness training during onboarding.

Existing employees:

Periodic security awareness training.

---

# 12.7 — Personnel Screening

Personnel should be screened to reduce risks from insider threats.

### Example

Depending on applicable law and organizational policy:

- Background checks
- Employment verification
- Reference checks

---

# 12.8 — Third-Party Service Provider (TPSP) Management

Risks associated with third-party service providers must be managed.

### Example TPSPs

- Cloud providers
- Payment processors
- Managed security providers
- Hosting providers
- SaaS providers

---

# 12.8.1 — TPSP Inventory

The organization must maintain a list of TPSPs that:

- Receive account data
- Share account data
- Could affect the security of account data

The list should include a description of services provided.

---

# 12.8.2 — Written Agreements

Written agreements with relevant TPSPs must address security responsibilities.

The agreement should establish that the TPSP is responsible for protecting account data that it possesses or otherwise stores, processes, or transmits on behalf of the entity, or to the extent the TPSP could impact security.

---

# 12.8.3 — TPSP Due Diligence

The organization must have a process for engaging TPSPs, including appropriate due diligence before engagement.

### Example

Before onboarding a cloud provider:

- Security questionnaire
- SOC 2 report
- PCI DSS AOC
- ISO 27001 certificate
- Data protection review
- Contract review
- Risk assessment

---

# 12.8.4 — Monitor TPSP Compliance

The organization must monitor the TPSP's PCI DSS compliance status at least once every 12 months.

### Example

Every year:

Check whether the service provider's:

- AOC
- ROC
- Certification
- Compliance status

is still valid/current.

---

# 12.8.5 — Responsibility Matrix

The organization must maintain information about which PCI DSS requirements are:

- Managed by the TPSP
- Managed by the organization
- Shared between both parties

### Example

Cloud provider:

Infrastructure security → TPSP

Application security → Organization

Access management → Shared

This prevents responsibility gaps.

---

# 12.9 — TPSP Responsibility for Customers

TPSPs must support their customers' PCI DSS compliance where applicable.

### Example

If a TPSP provides a service that is relied upon to meet a PCI DSS requirement, the TPSP must provide appropriate information/evidence about the service and its responsibilities.

---

# 🔎 Audit Evidence for Requirement 12

Auditors may request:

- Information security policy
- Policy review records
- Acceptable Use Policy
- Targeted Risk Analyses
- PCI DSS responsibility matrix
- PCI DSS scope document
- Security awareness training records
- Employee screening procedures
- TPSP inventory
- Vendor risk assessments
- Vendor questionnaires
- Contracts
- AOCs/ROCs
- Annual TPSP compliance reviews
- Responsibility matrix
- PCI DSS compliance program documentation

---

# 🎤 Interview Questions

### Q1. What is the purpose of Requirement 12?

**Answer:**

Requirement 12 establishes the organizational policies and governance processes needed to support PCI DSS compliance and information security.

---

### Q2. What is an information security policy?

**Answer:**

It is a high-level document that defines the organization's security objectives, principles, responsibilities, and direction for protecting information assets.

---

### Q3. Why is policy review important?

**Answer:**

Because the organization's technology, threats, business processes, and regulatory requirements can change. Policies must remain current and relevant.

---

### Q4. What is targeted risk analysis?

**Answer:**

Targeted risk analysis is a documented risk assessment used by an organization to determine an appropriate frequency or approach where PCI DSS allows flexibility based on risk.

---

### Q5. What is PCI DSS scope?

**Answer:**

PCI DSS scope defines the people, processes, technologies, systems, networks, and environments that are subject to PCI DSS because they store, process, transmit cardholder data or could impact its security.

---

### Q6. What is a TPSP?

**Answer:**

TPSP stands for Third-Party Service Provider. It is an external organization that provides services that involve account data or could impact the security of the organization's cardholder data environment.

---

### Q7. What is vendor due diligence?

**Answer:**

Vendor due diligence is the process of assessing a third party's security, compliance, risks, and capabilities before engaging them.

---

### Q8. Why do we need a TPSP inventory?

**Answer:**

To know which third parties have access to account data or can affect the security of the CDE, and to manage their associated risks.

---

### Q9. Why should TPSP compliance be reviewed annually?

**Answer:**

Because a provider's security and PCI DSS compliance status can change. Annual monitoring helps ensure that the organization continues to understand the provider's compliance status.

---

### Q10. What is the responsibility matrix between an organization and TPSP?

**Answer:**

It identifies which PCI DSS requirements are managed by the organization, which are managed by the TPSP, and which are shared between them.

---

# ⭐ Key Takeaway

Requirement 12 = **Governance + Policies + Risk + Compliance + Third Parties**

Think:

**Policy → Risk → Compliance → Scope → Awareness → Personnel → TPSP**
