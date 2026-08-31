# PCI DSS Requirement 4
## Protect Cardholder Data with Strong Cryptography During Transmission Over Open, Public Networks

### Objective

The objective of Requirement 4 is to protect cardholder data during transmission over open and public networks.

When cardholder data travels across networks that are not considered trusted, strong cryptography and secure protocols should be used to protect the data.

---

## Key Concept

Data can be exposed while travelling between systems.

Examples:

- Customer browser → Web application
- Payment application → Payment service provider
- Branch network → Data center
- Application → API

Requirement 4 focuses on protecting account data while it is being transmitted.

---

## Open and Public Networks

Examples include:

- The Internet
- Public Wi-Fi
- Other publicly accessible networks

These environments can increase the risk of interception.

---

## Strong Cryptography

Strong cryptography helps protect transmitted account data from unauthorized disclosure or modification.

Examples of technologies/protocols that may provide cryptographic protection include:

- TLS
- HTTPS
- Secure VPN technologies
- Other PCI DSS-approved cryptographic implementations

The exact cryptographic protocols and configurations should follow current PCI DSS requirements and organizational standards.

---

## Example

### Insecure

Customer card data:

Customer Browser → HTTP → Web Server

HTTP does not provide encryption for the transmitted information.

### Secure

Customer Browser → HTTPS/TLS → Web Server

TLS provides cryptographic protection for data transmitted between the endpoints.

---

## Why Requirement 4 Matters

Without appropriate protection, attackers may be able to intercept sensitive information during transmission.

Potential risks include:

- Data interception
- Man-in-the-middle attacks
- Unauthorized disclosure
- Modification of transmitted information

---

## Wireless Networks

Wireless technologies can introduce additional security risks.

Organizations should ensure that wireless networks used to transmit account data are secured using appropriate cryptographic protections.

---

## Secure Protocol Configuration

Using a secure protocol alone is not sufficient.

Organizations should also ensure that:

- Insecure protocols are disabled where required
- Cryptographic configurations are appropriately managed
- Certificates are properly managed
- Strong cryptographic algorithms and protocols are used
- Configuration changes are controlled

---

## GRC / Audit Perspective

During a PCI DSS assessment, an auditor may want to understand:

- Where account data is transmitted
- Which networks are involved
- Which protocols are used
- Whether strong cryptography is implemented
- Whether insecure protocols are disabled
- How cryptographic configurations are maintained

---

## Examples of Audit Evidence

Possible evidence may include:

- Network diagrams
- Data-flow diagrams
- TLS configuration
- SSL/TLS certificate information
- Firewall configurations
- Wireless configuration
- Encryption standards
- System configuration screenshots
- Configuration review records

---

## Example Control

### Control

Cardholder data transmitted over open and public networks must be protected using strong cryptography and secure protocols.

### Possible Evidence

- TLS configuration
- Approved cryptographic standards
- Network diagrams
- Configuration review records
- Certificate management records

---

## Interview Questions

### Q1. What is the purpose of PCI DSS Requirement 4?

To protect cardholder data during transmission over open and public networks using appropriate cryptographic protections.

### Q2. Why is HTTPS important?

HTTPS uses TLS to provide encrypted communication between a client and a server.

### Q3. Is encryption during transmission enough by itself?

No. Organizations also need appropriate secure protocol configurations, certificate management, and supporting security controls.

---

## Key Takeaways

- Protect account data while it is being transmitted.
- Use strong cryptography where required.
- Secure transmissions over open and public networks.
- Avoid insecure protocols and configurations.
- Maintain appropriate cryptographic and certificate management.
- Keep evidence demonstrating that transmission security controls are implemented.

---

## Reference

PCI Security Standards Council — PCI DSS

https://www.pcisecuritystandards.org/standards/pci-dss/

These notes are for personal learning purposes and contain no confidential company or client information.
