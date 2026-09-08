# PCI DSS Requirement 8
## Identify Users and Authenticate Access to System Components

### Objective

The objective of Requirement 8 is to ensure that users accessing system components can be uniquely identified and appropriately authenticated.

The basic principle is:

> Every user should be identifiable and authenticated before receiving access.

---

# Why Authentication Matters

Without proper authentication, an attacker could potentially access systems using:

- Stolen credentials
- Shared accounts
- Weak passwords
- Compromised authentication factors

Strong authentication reduces these risks.

---

# 8.1 — Processes and Mechanisms

Organizations should define and understand processes for identifying users and authenticating access.

Responsibilities should be assigned and understood.

---

# 8.2 — User Identification and Account Management

Organizations should manage user accounts appropriately.

Important concepts include:

- Unique user IDs
- Account lifecycle management
- User provisioning
- User modification
- User termination
- Third-party accounts
- Service accounts

---

# Unique User IDs

Each individual should have a unique identifier.

### Bad Example

```text
admin
admin
admin
