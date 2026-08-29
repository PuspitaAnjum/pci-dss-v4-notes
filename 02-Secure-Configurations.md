# PCI DSS Requirement 2
## Apply Secure Configurations to All System Components

### Objective

The objective of Requirement 2 is to ensure that system components within the PCI DSS scope are securely configured and managed.

Secure configurations help reduce vulnerabilities caused by unnecessary services, insecure settings, vendor defaults, and weak system configurations.

---

## Key Concept

A secure configuration means that systems are configured according to defined security standards rather than relying on default or insecure settings.

This applies to system components such as:

- Operating systems
- Servers
- Network devices
- Applications
- Databases
- Security technologies
- Cloud-based system components

---

## Requirement 2.1 — Processes and Mechanisms

Organizations should define and understand processes and mechanisms for applying secure configurations.

Security policies and operational procedures should be:

- Documented
- Kept up to date
- In use
- Known to affected personnel

Roles and responsibilities should also be documented, assigned, and understood.

### GRC Perspective

From an audit perspective, it is not enough for a company to have a configuration standard.

The organization should be able to demonstrate that the standard is:

1. Documented
2. Approved
3. Implemented
4. Maintained
5. Followed by responsible personnel

---

## Requirement 2.2 — Secure System Configuration

System components should be configured and managed securely.

Examples include:

- Removing unnecessary services
- Disabling unnecessary ports and protocols
- Implementing secure configuration standards
- Restricting administrative access
- Reviewing configuration settings
- Keeping configuration standards updated

---

## Vendor Default Accounts

Vendor-supplied default accounts are an important security concern.

Organizations should:

- Change default passwords when default accounts are required
- Remove or disable default accounts when they are not required
- Ensure default credentials are not left active

### Example

A newly installed network device uses:

Username: `admin`

Password: `admin`

Leaving these credentials unchanged creates an unnecessary security risk.

A secure configuration process would require the default credentials to be changed or the account to be disabled if it is not required.

---

## Why Requirement 2 Matters

Attackers can exploit weak or default configurations to gain unauthorized access.

Secure configuration helps reduce:

- Attack surface
- Unauthorized access
- Exploitation of unnecessary services
- Configuration-related vulnerabilities
- Risk caused by default credentials

---

## Examples of Audit Evidence

During a PCI DSS assessment, an assessor may review evidence such as:

- System configuration standards
- Network device configurations
- Server hardening standards
- Configuration review records
- Change management records
- Lists of enabled services
- Vendor documentation
- Evidence showing default accounts were changed or disabled
- Configuration scan results

---

## Example Control

### Control

All production servers must follow the organization's approved secure configuration baseline before being deployed.

### Possible Evidence

- Approved configuration baseline
- Server build checklist
- Configuration screenshots
- Change tickets
- Periodic configuration review records

---

## Interview Questions

### Q1. Why are secure configurations important in PCI DSS?

Secure configurations reduce unnecessary attack surfaces and help prevent unauthorized access caused by insecure system settings.

### Q2. What should an organization do with vendor default accounts?

If a vendor default account is not required, it should be removed or disabled. If it is required, the default password must be changed according to applicable PCI DSS requirements.

### Q3. What would an auditor look for?

An auditor may examine configuration standards, system configurations, vendor documentation, and evidence that secure configuration requirements are actually implemented.

---

## GRC / Audit Perspective

Requirement 2 demonstrates an important GRC principle:

> A security requirement should not only exist on paper; the organization must be able to demonstrate that it is implemented and maintained.

An auditor therefore considers both:

**Documentation + Implementation Evidence**

---

## Key Takeaways

- Secure configurations reduce attack surface.
- Vendor default credentials must not remain insecure.
- Unnecessary services and protocols should be addressed.
- Configuration standards should be documented and maintained.
- Roles and responsibilities should be clearly assigned.
- Evidence is important during a PCI DSS assessment.

---

## Reference

PCI Security Standards Council — PCI DSS

https://www.pcisecuritystandards.org/standards/pci-dss/

Official PCI SSC resources:
https://www.pcisecuritystandards.org/

These notes are for personal learning purposes and contain no confidential company or client information.
