# PCI DSS Requirement 8
## Identify Users and Authenticate Access to System Components

### Objective

The objective of Requirement 8 is to ensure that users are properly identified and authenticated before accessing systems and data.

Organizations should be able to associate system access with individual users.

---

## Key Concept

Authentication answers:

> "Who are you?"

Authorization answers:

> "What are you allowed to do?"

Requirement 8 primarily focuses on identifying and authenticating users.

---

## User Identification

Each individual user should have a unique identification mechanism where required.

Examples include:

- Unique usernames
- Individual user accounts
- Unique IDs

Shared accounts can make it difficult to determine who performed an activity.

---

## Authentication Factors

Authentication can use different factors.

### Something You Know

Examples:

- Password
- PIN

### Something You Have

Examples:

- Security token
- Authentication application
- Smart card

### Something You Are

Examples:

- Fingerprint
- Facial recognition
- Other biometric characteristics

---

## Multi-Factor Authentication (MFA)

MFA uses multiple authentication factors.

Example:

**Password + Authentication App**

This combines:

- Something you know
- Something you have

MFA provides stronger authentication than relying on a password alone.

---

## Password Security

Organizations should establish appropriate password and authentication requirements.

Controls may include:

- Password length requirements
- Password protection
- Account lockout mechanisms
- Secure authentication procedures
- Protection against unauthorized credential use

---

## Service Accounts

Some applications require non-human or service accounts.

These accounts should be managed securely and should not be treated like ordinary shared user accounts.

Organizations should:

- Assign ownership
- Restrict privileges
- Protect credentials
- Monitor usage
- Review accounts periodically

---

## Example Scenario

### Situation

Five administrators use the same account:

`admin`

### Problem

If a configuration change is made, it may be difficult to determine which individual performed the action.

### Better Approach

Each administrator receives an individual account.

Example:

```text
admin-puspita
admin-user2
admin-user3
