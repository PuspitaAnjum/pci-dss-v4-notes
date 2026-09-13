# PCI DSS Requirement 10 — Log and Monitor All Access to System Components and Cardholder Data

## 🎯 Objective

Requirement 10 ensures that organizations:

- Record important security events.
- Monitor activity.
- Detect suspicious behavior.
- Protect logs from unauthorized modification.
- Retain logs for investigation.
- Maintain consistent time across systems.

### Simple Example

If an administrator logs into a database containing cardholder data:

The organization should be able to determine:

- Who logged in
- When they logged in
- What system they accessed
- What activity occurred
- Whether the activity was suspicious

---

# 10.1 — Logging and Monitoring Processes

Processes and mechanisms for logging and monitoring access to:

- System components
- Cardholder data

must be defined and understood.

## 10.1.1 — Policies and Procedures

Requirement 10 policies and procedures must be:

- Documented
- Updated
- In use
- Known to affected personnel

## 10.1.2 — Roles and Responsibilities

Roles and responsibilities for logging and monitoring must be:

- Documented
- Assigned
- Understood

---

# 10.2 — Audit Logs

Audit logs must support:

- Detection of anomalies
- Detection of suspicious activity
- Forensic investigation

### Important Events to Log

Examples include:

- User login
- Failed login
- Logout
- Administrator activity
- Changes to accounts
- Changes to privileges
- Access to cardholder data
- Security control changes
- System events

---

# 10.2.1 — User Activity

Logs should allow the organization to determine important user activity.

### Example

Instead of:

"Someone accessed the database."

The log should allow investigators to identify:

"User ABC logged into Server X at 10:32 PM."

---

# 10.2.2 — Administrative Activity

Administrative actions should be logged.

### Example

Administrator changes:

Firewall rule

→ Event is recorded

Database permission

→ Event is recorded

User privilege

→ Event is recorded

---

# 10.2.3 — Invalid Logical Access Attempts

Failed or invalid access attempts must be logged.

### Example

User enters the wrong password five times.

The event should be recorded.

---

# 10.2.4 — Authentication Mechanisms

Changes to authentication mechanisms must be logged.

### Examples

- Password changes
- MFA changes
- Authentication configuration changes
- Account changes

---

# 10.2.5 — Audit Log Initialization / Stopping / Pausing

Actions that affect audit logging must be recorded.

### Why?

An attacker might try to disable logging before performing malicious activity.

---

# 10.2.6 — Creation and Deletion of System-Level Objects

Important system-level object creation/deletion events should be logged.

### Examples

- Creating a database
- Deleting a database
- Creating privileged objects
- Deleting critical system objects

---

# 10.3 — Protect Audit Logs

Audit logs must be protected from:

- Destruction
- Unauthorized modification

### Examples

Use:

- Restricted permissions
- Centralized logging
- SIEM
- Log integrity controls
- Access monitoring

---

# 10.4 — Review Audit Logs

Audit logs must be reviewed to identify:

- Anomalies
- Suspicious activity

## 10.4.1

Logs must be reviewed at a defined frequency based on the applicable PCI DSS requirement and the organization's targeted risk analysis where specified.

## 10.4.1.1

Automated mechanisms are used to perform audit log reviews.

### Example

SIEM automatically analyzes:

- Failed logins
- Multiple authentication failures
- Privilege changes
- Suspicious access
- Unusual activity

---

# 10.4.2 — Review for Other System Components

Certain system components must have logs reviewed according to the applicable PCI DSS frequency and process.

---

# 10.4.3 — Address Exceptions and Anomalies

If a suspicious event is detected, the organization must have a process for addressing it.

### Example

SIEM detects:

50 failed login attempts from one IP.

Security team:

1. Investigates.
2. Determines whether activity is malicious.
3. Takes appropriate action.
4. Documents the investigation.

---

# 10.5 — Retain Audit Log History

Audit log history must be retained and available for analysis.

### Why?

Historical logs may be needed for:

- Incident investigation
- Forensics
- Compliance
- Threat hunting

---

# 10.6 — Time Synchronization

Systems must use time-synchronization mechanisms so that system clocks remain consistent.

### Example

Server A = 10:30:00

Server B = 10:30:02

Server C = 10:29:59

Small differences can make investigations difficult.

Organizations commonly use:

**NTP — Network Time Protocol**

---

# 10.7 — Detect and Respond to Failures

Failures of critical security control systems must be:

- Detected
- Reported
- Responded to promptly

### Examples

- Firewall failure
- IDS/IPS failure
- Logging failure
- SIEM failure
- Authentication-control failure

---

# 🔎 Audit Evidence for Requirement 10

Auditors may request:

- Logging policy
- Log management procedure
- SIEM configuration
- Sample audit logs
- Log review reports
- Security alerts
- Incident tickets
- Log retention configuration
- NTP configuration
- Time synchronization evidence
- Privileged activity logs
- Failed-login logs
- Administrative activity logs

---

# 🎤 Interview Questions

### Q1. Why is logging important?

**Answer:**

Logging provides visibility into system and user activity and helps detect suspicious behavior and perform forensic investigations.

---

### Q2. What is a SIEM?

**Answer:**

SIEM stands for Security Information and Event Management. It collects and analyzes security logs from multiple sources to detect suspicious activity and generate alerts.

---

### Q3. Why do we need centralized logging?

**Answer:**

Centralized logging makes it easier to collect, correlate, monitor, protect, and investigate logs from multiple systems.

---

### Q4. Why is time synchronization important?

**Answer:**

It ensures that events across different systems have consistent timestamps, which is critical for monitoring and forensic investigation.

---

### Q5. What is NTP?

**Answer:**

NTP stands for Network Time Protocol. It is used to synchronize system clocks with a reliable time source.

---

### Q6. What happens if an attacker deletes logs?

**Answer:**

It can make investigation difficult and hide malicious activity. Therefore, audit logs must be protected from unauthorized modification and destruction.

---

### Q7. Give examples of events that should be logged.

**Answer:**

User logins, failed login attempts, administrator activity, changes to privileges, access to cardholder data, authentication changes, and important system/security events.

---

# ⭐ Key Takeaway

Requirement 10 = **Logging + Monitoring + Investigation**

Think:

**Record → Protect → Review → Synchronize → Respond**
