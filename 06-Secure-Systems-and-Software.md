# PCI DSS Requirement 6
## Develop and Maintain Secure Systems and Software

### Objective

The objective of Requirement 6 is to ensure that systems and software are developed, maintained, and changed securely so that vulnerabilities do not expose account data.

Security needs to be considered throughout the software and system lifecycle rather than being added only after deployment.

---

# 6.1 — Processes and Mechanisms

## What does 6.1 mean?

PCI DSS Requirement 6.1 requires organizations to define and understand the processes and mechanisms used to develop and maintain secure systems and software.

In simple words:

> The organization must have a defined process for keeping systems and software secure.

This includes having documented processes, assigned responsibilities, and mechanisms that support the activities under Requirement 6.

---

## Why is 6.1 important?

If an organization does not have a defined process, security activities can become inconsistent.

For example:

Developer A:
- Performs security testing before release.

Developer B:
- Releases software without security testing.

A documented process creates consistency.

---

## GRC Perspective

From a GRC perspective, 6.1 is about:

**Process + Ownership + Documentation + Implementation**

An organization should be able to demonstrate:

1. What the process is
2. Who is responsible
3. How the process works
4. What evidence demonstrates that it is being followed

---

## Roles and Responsibilities

Responsibilities for Requirement 6 activities should be assigned.

Examples:

- Developers
- Security team
- IT operations
- System administrators
- Change management team
- Application owners

A RACI matrix can be used to document responsibilities.

---

## Example

### Control

The organization maintains a documented secure software development process.

### Responsible

Application Development Team

### Accountable

Application Owner / Security Management

### Evidence

- Secure SDLC document
- RACI matrix
- Security procedures
- Development standards
- Training records
- Change records

---

# 6.2 — Bespoke and Custom Software Are Developed Securely

## What does 6.2 mean?

Requirement 6.2 focuses specifically on **bespoke and custom software**.

The software must be developed securely using recognized secure-development practices and PCI DSS requirements.

PCI SSC explains that 6.2 applies to software developed by or for the entity for its own use, including bespoke and custom software; it does not apply to third-party software itself. :contentReference[oaicite:1]{index=1}

---

# 6.2.1 — Secure Software Development

Bespoke and custom software must be developed securely:

### 1. Based on industry standards or best practices

Examples:

- Secure SDLC
- OWASP guidance
- NIST guidance
- Secure coding practices

### 2. In accordance with PCI DSS

Security requirements should be considered during development.

Examples:

- Secure authentication
- Secure logging
- Access control
- Protection of account data

### 3. Throughout the SDLC

Security should be considered during:

- Requirements
- Design
- Development
- Testing
- Deployment
- Maintenance

PCI SSC's testing procedure for 6.2.1 specifically looks for documented software-development procedures covering these elements. :contentReference[oaicite:2]{index=2}

---

# 6.2.2 — Developer Security Training

Personnel working on bespoke and custom software must receive security training at least once every 12 months.

Training should be relevant to:

- Their job function
- Development languages
- Secure software design
- Secure coding techniques
- Security testing tools, where used

This means developers should not simply know how to write code—they should understand how to write **secure code**. :contentReference[oaicite:3]{index=3}

---

# 6.2.3 — Code Review

Bespoke and custom software should undergo appropriate review before release.

The purpose is to identify security vulnerabilities before software reaches production.

Possible review methods include:

- Manual code review
- Automated code analysis
- Security-focused review processes

If manual code review is used, additional requirements apply regarding who performs the review and how independence is maintained.

---

# 6.2.4 — Prevent Common Software Attacks

Software development techniques should be used to prevent or mitigate common software attacks.

Examples include:

- SQL Injection
- Command Injection
- Cross-Site Scripting (XSS)
- Authentication weaknesses
- Access control weaknesses
- Other injection vulnerabilities

Example:

Instead of building SQL queries using unsanitized user input:

    SELECT * FROM users WHERE id = ' + user_input

Use parameterized queries.

---

# 6.3 — Security Vulnerabilities Are Identified and Addressed

Requirement 6.3 focuses on identifying and addressing security vulnerabilities.

Organizations should have processes for:

- Identifying vulnerabilities
- Risk-ranking vulnerabilities
- Addressing vulnerabilities
- Managing software components
- Applying appropriate security updates

---

# 6.3.1 — Vulnerability Identification

Security vulnerabilities should be identified using appropriate sources.

Examples:

- Vendor security advisories
- Vulnerability databases
- Security alerts
- Vulnerability scanning
- Security monitoring

---

# 6.3.2 — Software Inventory

Organizations should maintain an inventory of bespoke and custom software.

The inventory helps identify:

- What software exists
- Who owns it
- Where it is used
- Which software is in scope
- Which applications need security attention

---

# 6.4 — Protect Public-Facing Web Applications

Public-facing web applications require protection against web-based attacks.

Examples of security mechanisms include:

- Web Application Firewall (WAF)
- Application security testing
- Vulnerability assessments
- Secure coding
- Attack detection mechanisms

Important:

PCI DSS v4.0.1 includes **6.4.2**, which requires an automated technical solution to continually detect and prevent web-based attacks against public-facing web applications. PCI SSC notes that 6.4.2 superseded 6.4.1 effective March 31, 2025. :contentReference[oaicite:4]{index=4}

---

# 6.5 — Manage Changes Securely

Changes to system components must be managed securely.

Examples:

- New software deployment
- Configuration changes
- Firewall changes
- Database changes
- Application updates

A change management process should help ensure that changes are:

1. Requested
2. Reviewed
3. Approved
4. Tested
5. Implemented
6. Documented

---

# Audit Evidence Examples

An auditor may request:

- Secure SDLC policy
- Software development procedures
- Developer training records
- Code review evidence
- Vulnerability scan results
- Software inventory
- Change tickets
- Security testing reports
- WAF configuration
- Application security assessment reports

---

# GRC / Audit Perspective

For Requirement 6, an auditor is essentially asking:

> "Can you demonstrate that security is built into the system/software lifecycle?"

The organization should be able to demonstrate:

**Policy → Process → Implementation → Evidence → Review**

---

# Example Audit Scenario

### Situation

A company develops a payment application.

### Auditor asks:

"Show me evidence that security was considered before deployment."

### Possible Evidence:

- Secure SDLC
- Threat modeling
- Code review
- Vulnerability testing
- Developer training
- Change approval
- Deployment record

If the organization only has a policy but cannot demonstrate implementation, the control may not be adequately supported.

---

# Interview Questions

### Q1. What is the purpose of PCI DSS Requirement 6?

To ensure systems and software are developed, maintained, and changed securely to reduce vulnerabilities that could expose account data.

### Q2. What is 6.1?

6.1 focuses on defining and understanding the processes and mechanisms used to develop and maintain secure systems and software.

### Q3. What is 6.2?

6.2 focuses on securely developing bespoke and custom software.

### Q4. What is the difference between 6.1 and 6.2?

6.1 = Secure system/software processes and mechanisms.

6.2 = Secure development of bespoke and custom software.

### Q5. How often must software development personnel receive security training?

At least once every 12 months, with content relevant to their job functions and development technologies.

### Q6. Why is secure coding important?

Because vulnerabilities introduced during development can later be exploited to gain unauthorized access or compromise account data.

### Q7. Give examples of common software attacks.

Examples include SQL injection, command injection, XSS, authentication weaknesses, and access-control vulnerabilities.

### Q8. What evidence could an auditor request for Requirement 6?

Examples include secure SDLC procedures, training records, code review evidence, vulnerability reports, software inventories, and change-management records.

---

# Key Takeaways

- 6.1 = Defined secure development and maintenance processes.
- 6.2 = Secure development of bespoke/custom software.
- 6.2.1 = Secure development throughout the SDLC.
- 6.2.2 = Developer security training.
- 6.2.3 = Code review.
- 6.2.4 = Prevent/mitigate common software attacks.
- 6.3 = Identify and address vulnerabilities.
- 6.4 = Protect public-facing web applications.
- 6.5 = Manage changes securely.

---

## Reference

PCI Security Standards Council — PCI DSS

https://www.pcisecuritystandards.org/standards/pci-dss/

These notes are for personal learning purposes and contain no confidential company or client information.

