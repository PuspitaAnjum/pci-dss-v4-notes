# PCI DSS Requirement 9 — Restrict Physical Access to Cardholder Data

## 🎯 Objective

Requirement 9 focuses on protecting cardholder data and systems from **unauthorized physical access**.

Even if an organization has strong logical security, an attacker or unauthorized person who physically reaches a server, network device, backup, payment terminal, or media may be able to steal or manipulate sensitive information.

### Simple Example

If a company's CDE server room contains systems that process cardholder data:

- Only authorized personnel should enter.
- Entry should be controlled.
- Physical access should be monitored.
- Visitors should be identified and escorted.
- Cardholder-data media should be securely stored and destroyed.
- Payment terminals should be protected from tampering.

---

# 9.1 — Processes and Mechanisms for Restricting Physical Access

The organization must have documented processes and mechanisms for controlling physical access to cardholder data.

## 9.1.1 — Security Policies and Procedures

Policies and operational procedures related to Requirement 9 must be:

- Documented
- Kept up to date
- In use
- Known to affected personnel

### Example

An organization may have a Physical Security Policy describing:

- Who can enter the server room
- How visitor access works
- How access cards are issued
- How CCTV is monitored
- How media is handled

## 9.1.2 — Roles and Responsibilities

Roles and responsibilities for Requirement 9 activities must be:

- Documented
- Assigned
- Understood

### Example

Security Team → monitors physical security

Facilities Team → manages building access

IT Team → manages server-room access

---

# 9.2 — Physical Access Controls

Physical access controls must manage entry into facilities and systems containing cardholder data.

## 9.2.1 — Facility Entry Controls

Appropriate controls must restrict physical access to systems in the CDE.

### Examples

- Access cards
- Badge readers
- Biometric authentication
- Locks
- Security guards
- Mantraps

### Audit Evidence

An assessor may:

- Observe access controls
- Review access lists
- Interview responsible personnel
- Check physical security procedures

---

## 9.2.1.1 — Monitoring Sensitive Areas

Individual physical access to sensitive areas within the CDE must be monitored using:

- Video cameras
- Physical access-control mechanisms
- Or both

The controls must:

1. Monitor entry and exit points.
2. Be protected from tampering or disabling.
3. Have collected data reviewed/correlated with other entries.
4. Store collected data for at least three months, unless otherwise restricted by law.

### Example

Server room:

Employee uses access card → access event is recorded → CCTV captures entry → records are retained.

---

# 9.3 — Physical Access for Personnel and Visitors

Physical access for employees and visitors must be authorized and managed.

## Personnel

Organizations should ensure that employees only receive physical access appropriate to their responsibilities.

## Visitors

Visitors must be appropriately managed.

### Example

A vendor comes to the data center:

1. Visitor is authorized.
2. Identity is verified.
3. Visitor receives identification.
4. Visitor is escorted where required.
5. Visitor access is recorded.
6. Visitor access is removed/ended when they leave.

---

# 9.4 — Media Containing Cardholder Data

Media containing cardholder data must be securely:

- Stored
- Accessed
- Distributed
- Destroyed

### Media Examples

- Backup tapes
- USB drives
- Hard drives
- Printed documents
- Paper receipts
- Archived files

### Secure Destruction Examples

Paper → shredding

Hard drive → secure destruction/wiping according to applicable requirements

Backup media → secure disposal

---

# 9.5 — Protect Point-of-Interaction (POI) Devices

Point-of-interaction devices must be protected against:

- Tampering
- Unauthorized substitution

### Examples

- POS terminals
- Card readers
- Payment terminals

### What should organizations do?

They should maintain an inventory of POI devices and periodically inspect them for:

- Missing components
- Unexpected attachments
- Modified seals
- Changed serial numbers
- Suspicious cables
- Unauthorized replacement

---

# 🔎 Audit Evidence for Requirement 9

An auditor may request:

- Physical security policy
- Data center/server-room access list
- Access-card records
- Visitor logs
- CCTV procedures
- CCTV retention evidence
- Physical access reviews
- Media handling procedures
- Media destruction records
- POI device inventory
- POI inspection records
- Visitor authorization records

---

# 🎤 Interview Questions

### Q1. What is the purpose of Requirement 9?

**Answer:**

Requirement 9 protects cardholder data and systems from unauthorized physical access.

---

### Q2. What is a sensitive area?

**Answer:**

A sensitive area is a physical area within the CDE where systems containing cardholder data are located, such as a server room or data center.

---

### Q3. Why is CCTV important?

**Answer:**

CCTV helps monitor physical access, detect suspicious activity, and provide evidence during investigations.

---

### Q4. How long should physical access monitoring data generally be retained?

**Answer:**

At least three months, unless otherwise restricted by law.

---

### Q5. How should visitors be handled?

**Answer:**

Visitors should be authorized, identified, monitored according to the organization's process, and their access should be properly recorded.

---

### Q6. What is POI?

**Answer:**

POI means Point of Interaction. It refers to devices used to interact with payment cards, such as POS terminals and card readers.

---

### Q7. Why should POI devices be inspected?

**Answer:**

To detect tampering or unauthorized substitution that could compromise payment card data.

---

# ⭐ Key Takeaway

Requirement 9 = **Physical Security**

Think:

**Entry → Monitoring → Visitors → Media → POI Protection**
