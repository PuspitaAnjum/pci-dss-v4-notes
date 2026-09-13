# PCI DSS Requirement 11 — Test Security of Systems and Networks Regularly

## 🎯 Objective

Requirement 11 ensures that security controls are regularly tested to verify that they continue to work effectively.

### Why?

Security controls can become ineffective because of:

- New vulnerabilities
- Configuration changes
- New technologies
- Network changes
- New attack techniques

Therefore, security must be continuously tested.

---

# 11.1 — Testing Processes

Processes and mechanisms for regularly testing security systems and networks must be:

- Defined
- Documented
- Understood

## 11.1.1 — Policies and Procedures

Requirement 11 policies and procedures must be:

- Documented
- Updated
- In use
- Known to affected personnel

## 11.1.2 — Roles and Responsibilities

Roles and responsibilities must be:

- Documented
- Assigned
- Understood

---

# 11.2 — Wireless Access Points

Wireless access points must be:

- Identified
- Monitored
- Controlled

Unauthorized wireless access points must be addressed.

## 11.2.1

The organization must test for wireless access points and detect/identify authorized and unauthorized wireless devices.

Testing, detection, and identification occurs at least once every three months.

### Example

An organization officially has:

20 authorized Wi-Fi access points.

A scan discovers:

20 authorized APs + 1 unknown AP.

The unknown AP must be investigated and addressed.

---

# 11.3 — Vulnerability Management

External and internal vulnerabilities must be:

- Regularly identified
- Prioritized
- Addressed

### Vulnerability Scanning

A vulnerability scan looks for potential weaknesses in:

- Operating systems
- Applications
- Network devices
- Servers
- Other system components

---

# 11.3.1 — Internal Vulnerability Scans

Internal vulnerability scans must be performed according to the applicable PCI DSS frequency and methodology.

Vulnerabilities are prioritized according to the organization's vulnerability risk-ranking process.

---

# 11.3.2 — External Vulnerability Scans

External vulnerability scans are performed by:

- Qualified internal resources
- Or a qualified external third party

The testing should maintain organizational independence.

### Important Term

**ASV = Approved Scanning Vendor**

For applicable PCI DSS external scanning requirements, ASV scanning is an important concept.

---

# 11.4 — Penetration Testing

Penetration testing must be regularly performed to identify:

- Exploitable vulnerabilities
- Security weaknesses

The identified weaknesses must be corrected.

---

# 11.4.1 — Penetration Testing Methodology

The organization must define, document, and implement a penetration-testing methodology.

The methodology should define:

- Scope
- Testing approach
- Vulnerability identification
- Exploitation
- Reporting
- Remediation
- Retesting

---

# 11.4.2 — External Penetration Testing

External penetration testing must evaluate the security of externally accessible systems.

### Example

Internet-facing:

- Web servers
- APIs
- Firewalls
- VPN gateways

may be included depending on scope.

---

# 11.4.3 — Internal Penetration Testing

Internal penetration testing evaluates weaknesses that could be exploited from inside the organization's environment.

### Example

An attacker gains access to an internal workstation.

The test determines whether the attacker could:

Workstation → Internal network → CDE

---

# 11.4.4 — Segmentation Testing

Where network segmentation is used to isolate the CDE, segmentation controls must be tested to verify that they are effective.

### Example

Expected:

Internet
   ↓
DMZ
   ↓
Firewall
   ↓
CDE

The penetration test checks whether the CDE can actually be reached from an out-of-scope network.

---

# 11.4.5 — Penetration Test Remediation

Exploitable vulnerabilities and security weaknesses identified during penetration testing must be corrected.

Retesting should confirm that remediation was effective.

---

# 11.5 — Intrusion and File-Change Detection

Network intrusions and unexpected changes to critical files must be detected and responded to.

### Examples

- IDS/IPS
- File Integrity Monitoring
- Security monitoring tools

---

# 11.6 — Payment Page Security

Unauthorized changes and tampering with payment pages must be detected and responded to.

### Why?

Attackers may compromise a payment page and inject malicious JavaScript to steal payment information.

### Example

E-commerce website:

Customer → Payment Page → Card Details

Attacker injects malicious script.

The malicious script attempts to capture payment information.

Security controls should detect and respond to unauthorized changes.

---

# 🔎 Audit Evidence for Requirement 11

Auditors may request:

- Vulnerability scan reports
- ASV scan reports
- Penetration testing reports
- Penetration-testing methodology
- Remediation tickets
- Retest reports
- Wireless scan results
- Wireless access-point inventory
- Segmentation testing reports
- IDS/IPS configuration
- File Integrity Monitoring reports
- Payment-page monitoring evidence
- Security testing schedules

---

# 🎤 Interview Questions

### Q1. What is the purpose of Requirement 11?

**Answer:**

Requirement 11 ensures that security systems and processes are regularly tested so that vulnerabilities and weaknesses can be identified and corrected.

---

### Q2. What is vulnerability scanning?

**Answer:**

Vulnerability scanning is the process of using tools and methods to identify potential vulnerabilities in systems, applications, servers, and network devices.

---

### Q3. What is penetration testing?

**Answer:**

Penetration testing is an authorized security test where testers attempt to exploit vulnerabilities to determine whether they can actually be used to compromise systems or data.

---

### Q4. Vulnerability scanning vs penetration testing?

**Answer:**

Vulnerability scanning primarily identifies potential vulnerabilities.

Penetration testing goes further by attempting controlled exploitation to determine the real-world impact of vulnerabilities.

---

### Q5. What is ASV?

**Answer:**

ASV stands for Approved Scanning Vendor. PCI SSC recognizes ASVs for performing applicable external vulnerability scans for PCI DSS validation.

---

### Q6. Why is segmentation testing important?

**Answer:**

Segmentation testing verifies that controls separating the CDE from out-of-scope environments actually prevent unauthorized access.

---

### Q7. Why should penetration testing be followed by retesting?

**Answer:**

Retesting verifies that identified vulnerabilities or weaknesses were actually fixed and that the remediation was effective.

---

# ⭐ Key Takeaway

Requirement 11 = **Test Security Regularly**

Think:

**Wireless Testing → Vulnerability Scanning → Penetration Testing → Segmentation Testing → Intrusion/File Monitoring → Payment Page Monitoring**
