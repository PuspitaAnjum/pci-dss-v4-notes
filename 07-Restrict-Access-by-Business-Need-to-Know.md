# PCI DSS Requirement 7
## Restrict Access to System Components and Cardholder Data by Business Need to Know

### Objective

The objective of Requirement 7 is to ensure that users receive only the access they need to perform their job responsibilities.

The core principle is:

> Need to Know + Least Privilege

---

# What is Need to Know?

Need to know means a person receives access to information only when that access is necessary for their job.

### Example

A customer-support employee may need to see limited customer information.

They probably do not need:

- Database administrator access
- Firewall administration
- Full PAN access
- Production server administrator privileges

---

# What is Least Privilege?

Least privilege means users receive the minimum level of access required to perform their responsibilities.

### Example

If an employee only needs to read a database:

Give:

**Read access**

Instead of:

**Read + Write + Delete + Administrative access**

---

# 7.1 — Processes and Mechanisms

Organizations should define and understand processes for restricting access to system components and cardholder data.

Roles and responsibilities should be documented and understood.

---

# 7.2 — Access Control Model

An access control model should define how access is granted.

Access should consider:

- Business needs
- Job classification
- Job function
- Least privileges

PCI DSS specifically requires the access-control model to define appropriate access based on business/access needs and the least privileges necessary for the job function. :contentReference[oaicite:5]{index=5}

---

# 7.2.1 — Define Access

The organization should define what access different roles require.

Example:

| Role | Required Access |
|---|---|
| HR | HR systems |
| Developer | Development environment |
| Database Administrator | Database administration |
| SOC Analyst | Security monitoring |
| Finance | Financial systems |

---

# 7.2.2 — Assign Access

Access should be assigned based on:

- Job classification
- Job function
- Least privilege

### Example

A junior developer should not automatically receive production administrator privileges.

---

# 7.2.3 — Approve Access

Required privileges should be approved by authorized personnel.

Example:

Employee requests:

> Production database access

Manager/Security/Owner reviews:

> Is this access actually required?

If justified:

**Approve → Provision**

---

# 7.2.4 — Review User Access

User accounts and access privileges should be reviewed periodically.

The review should determine:

- Whether access is still required
- Whether access matches the user's job
- Whether inappropriate access exists
- Whether management acknowledges the access remains appropriate

---

# 7.2.5 — Application and System Accounts

Application and system accounts also need to be managed.

Examples:

- Database service accounts
- Application accounts
- API accounts
- Automated process accounts

These accounts should have appropriate privileges and ownership.

---

# Role-Based Access Control

A common implementation is:

**RBAC — Role-Based Access Control**

Instead of assigning permissions individually:

User → Role → Permissions

Example:

```text
Puspita
   ↓
GRC Analyst
   ↓
GRC Dashboard
Audit Documents
Risk Register
