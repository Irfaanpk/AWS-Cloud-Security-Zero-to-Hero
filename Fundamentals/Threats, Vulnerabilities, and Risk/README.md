
# Threats, Vulnerabilities, and Risk

## Overview

Cloud security threats, vulnerabilities, and risks are closely related concepts used to understand and manage security challenges in cloud environments.

A **threat** is a potential cause of harm, a **vulnerability** is a weakness that can be exploited, and a **risk** is the possibility of loss or damage when a threat exploits a vulnerability.

## 1. Security Threats

A security threat is any potential event, activity, or actor that could compromise the confidentiality, integrity, or availability of cloud resources.

Common cloud security threats include:

- **Unauthorized Access:** Accessing cloud resources without proper authorization.
- **Credential Theft:** Stealing passwords, access keys, or session credentials.
- **Malware and Ransomware:** Malicious software used to damage systems, steal information, or deny access to data.
- **Denial-of-Service (DoS) Attacks:** Overwhelming systems with traffic or requests to disrupt service availability.
- **Data Breaches:** Unauthorized exposure or disclosure of sensitive information.
- **Insider Threats:** Security risks caused by individuals with legitimate access, whether intentional or accidental.

## 2. Security Vulnerabilities

A vulnerability is a weakness in a system, configuration, application, or security process that could be exploited by a threat.

Common cloud vulnerabilities include:

- **Misconfigured Resources:** Storage or other services unintentionally exposed to the public.
- **Excessive Permissions:** Users or applications granted more access than necessary.
- **Unpatched Software:** Known vulnerabilities remaining in outdated systems or applications.
- **Weak Authentication:** Insufficient protection for user and administrative accounts.
- **Insecure APIs:** Application interfaces that lack appropriate authentication, authorization, or validation.
- **Insufficient Logging:** Missing security records that make suspicious activity difficult to identify.

## 3. Understanding Security Risk

Security risk represents the potential for a threat to exploit a vulnerability and cause harm to an organization.

Risk assessment commonly considers:

- **Likelihood:** The probability that a security event will occur.
- **Impact:** The potential consequences if the event occurs.

A simplified risk model is:

`Risk = Likelihood × Impact`

Organizations use risk assessments to prioritize security improvements according to the probability and potential consequences of threats.

## 4. Threat vs. Vulnerability vs. Risk

| Concept | Meaning | Example |
|---------|---------|---------|
| Threat | Something that could cause harm | An attacker attempting to access sensitive data |
| Vulnerability | A weakness that could be exploited | A storage resource configured for unintended public access |
| Risk | The potential for loss or damage | Sensitive data being exposed because of the misconfiguration |

## 5. Attack Surface and Attack Vectors

**Attack Surface** refers to the total set of points through which an attacker could potentially access or affect a system.

Examples include publicly accessible services, user accounts, APIs, endpoints, and network interfaces.

**Attack Vector** refers to the method or path used to exploit a weakness or gain unauthorized access.

Examples include phishing, stolen credentials, exploitation of software vulnerabilities, and abuse of insecure APIs.

Reducing the attack surface and securing common attack vectors help reduce the likelihood of successful attacks.

## 6. Risk Mitigation

Risk mitigation involves implementing measures to reduce the likelihood or impact of security incidents.

Common approaches include:

- Applying least-privilege access controls.
- Enabling multi-factor authentication (MFA).
- Encrypting sensitive data.
- Patching systems and applications.
- Restricting unnecessary public access.
- Monitoring security events and suspicious activity.
- Maintaining backups and recovery procedures.

In AWS, services such as AWS Identity and Access Management (IAM), Amazon GuardDuty, AWS Security Hub, and AWS CloudTrail can support different aspects of cloud risk management.

## References

- [AWS Security Documentation](https://docs.aws.amazon.com/security/)
- [AWS Well-Architected Framework — Security Pillar](https://docs.aws.amazon.com/wellarchitected/latest/security-pillar/welcome.html)
- [Amazon GuardDuty](https://docs.aws.amazon.com/guardduty/latest/ug/what-is-guardduty.html)
