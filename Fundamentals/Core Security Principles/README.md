
# Core Security Principles

## Overview

Core security principles provide the foundation for designing, implementing, and maintaining secure cloud environments. These principles help organizations protect data, control access, reduce risks, and maintain the confidentiality, integrity, and availability of resources.

## 1. CIA Triad

The CIA triad is a fundamental information security model consisting of three principles.

| Principle | Description | Example |
|-----------|-------------|---------|
| Confidentiality | Ensures information is accessible only to authorized users. | Restricting access to sensitive data using IAM permissions. |
| Integrity | Ensures information remains accurate and is not modified without authorization. | Using cryptographic hashes to verify file integrity. |
| Availability | Ensures systems and data remain accessible when required. | Deploying workloads across multiple Availability Zones. |

## 2. Least Privilege

The principle of least privilege ensures that users, applications, and services receive only the permissions necessary to perform their intended tasks.

- Avoid granting unnecessary administrative permissions.
- Assign permissions based on job responsibilities.
- Review and remove unused permissions.
- Use temporary credentials where appropriate.

In AWS, IAM policies and roles help implement least-privilege access.

## 3. Defense in Depth

Defense in depth uses multiple layers of security controls to protect systems and data. If one control fails, additional controls help reduce the likelihood or impact of a security incident.

Common layers include:

- **Physical Security:** Protects data centers and hardware.
- **Network Security:** Controls traffic between resources.
- **Identity Security:** Restricts access through authentication and authorization.
- **Data Security:** Protects information using encryption and access controls.
- **Monitoring:** Detects suspicious activities and security events.

## 4. Zero Trust

Zero Trust is a security approach based on the principle of not automatically trusting any user, device, or workload based solely on its network location.

Its key principles include:

- Verify explicitly using available identity and contextual information.
- Grant the minimum necessary access.
- Assume that a security breach may occur and limit its potential impact.

Zero Trust emphasizes continuous evaluation of access and security conditions rather than relying only on network boundaries.

## 5. Separation of Duties

Separation of duties divides critical responsibilities among different users or roles to reduce the risk of unauthorized actions, errors, and misuse of privileges.

For example, one user may request a sensitive infrastructure change while another user reviews and approves it.

This principle supports accountability and reduces the risk associated with a single individual controlling an entire critical process.

## 6. Security by Design and Default

**Security by Design** means incorporating security requirements into systems and architectures from the beginning rather than adding them after deployment.

**Security by Default** means configuring systems with secure initial settings, limiting unnecessary exposure, and requiring deliberate action to enable additional access.

Examples include:

- Restricting public access unless it is required.
- Enabling appropriate logging and monitoring.
- Applying secure access permissions.
- Disabling unnecessary services and features.

## References

- [AWS Well-Architected Framework — Security Pillar](https://docs.aws.amazon.com/wellarchitected/latest/security-pillar/welcome.html)
- [AWS Identity and Access Management](https://docs.aws.amazon.com/IAM/latest/UserGuide/introduction.html)
- [AWS Security Documentation](https://docs.aws.amazon.com/security/)
