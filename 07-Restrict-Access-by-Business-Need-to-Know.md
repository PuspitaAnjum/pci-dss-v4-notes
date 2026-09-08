# PCI DSS Requirement 7
## Restrict Access to System Components and Cardholder Data by Business Need to Know

### Objective

The objective of Requirement 7 is to restrict access to system components and cardholder data based on business need to know.

Users should receive only the access necessary to perform their job responsibilities.

---

## Key Concept

The principle behind Requirement 7 is:

> Users should have access only to the resources and information required for their job.

This is commonly associated with the principle of:

**Least Privilege**

---

## Business Need to Know

Business need to know means that access is granted because a user has a legitimate business requirement to access specific information or systems.

### Example

A database administrator may require access to a database server.

However, the same administrator may not need access to financial reports or unrelated business systems.

Access should therefore be limited according to actual responsibilities.

---

## Access Control

Organizations should define access requirements for:

- Users
- Administrators
- Applications
- System components
- Cardholder data

Access should be authorized before it is granted.

---

## Role-Based Access

Organizations can use roles to simplify access management.

Example:

### Employee

- Email
- Internal applications

### Finance Team

- Financial applications
- Relevant financial records

### Database Administrator

- Database administration systems
- Required database resources

Each role receives only the access required to perform its responsibilities.

---

## Access Reviews

Organizations should periodically review user access.

Reviews can help identify:

- Excessive privileges
- Unnecessary accounts
- Former employees
- Changed job responsibilities
- Inappropriate access

---

## Access Removal

When an employee leaves the organization, unnecessary access should be removed promptly according to the organization's access management procedures and applicable PCI DSS requirements.

---

## Example Scenario

### Situation

An employee moves from the Finance department to Marketing.

The employee still has access to the finance database.

### Risk

The employee may have access to information that is no longer required for their job.

### GRC Response

The organization should:

1. Identify the employee's new role
2. Review current permissions
3. Remove unnecessary access
4. Document the change
5. Maintain evidence

---

## GRC / Audit Perspective

An auditor may evaluate:

- Access control policies
- Role definitions
- User access lists
- Access approval records
- Periodic access reviews
- Terminated-user records
- Privileged access
- Evidence of access removal

The auditor wants to determine whether access is actually restricted according to business need.

---

## Examples of Audit Evidence

- Access control policy
- User access matrix
- Role-based access control configuration
- Access approval tickets
- User access review records
- Termination records
- Privileged access review
- Identity management reports

---

## Example Control

### Control

Access to cardholder data and system components is granted based on documented business need and approved according to organizational procedures.

### Possible Evidence

- Access request
- Manager approval
- Access matrix
- User account configuration
- Periodic access review

---

## Interview Questions

### Q1. What is the principle of least privilege?

Users should receive only the minimum access necessary to perform their assigned responsibilities.

### Q2. What is business need-to-know?

Access is provided only when a user has a legitimate business requirement for specific systems or information.

### Q3. Why are access reviews important?

They help identify excessive, outdated, or inappropriate access.

---

## Key Takeaways

- Restrict access based on business need.
- Apply least privilege.
- Define access based on job responsibilities.
- Review access periodically.
- Remove unnecessary access when roles change.
- Maintain evidence of approvals and reviews.

---

## Reference

PCI Security Standards Council — PCI DSS

https://www.pcisecuritystandards.org/standards/pci-dss/

These notes are for personal learning purposes and contain no confidential company or client information.
