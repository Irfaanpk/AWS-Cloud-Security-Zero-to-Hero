
# Cryptography Fundamentals

## Overview

Cryptography is the practice of protecting information using mathematical techniques to prevent unauthorized access, detect modifications, and verify authenticity.

In cloud environments, cryptography is commonly used to protect data at rest, secure data in transit, verify data integrity, and establish trust between communicating systems.

## 1. Encryption

Encryption converts readable data, known as **plaintext**, into an unreadable form called **ciphertext** using a cryptographic algorithm and a key.

Decryption reverses this process to recover the original data using the appropriate key.

Encryption is primarily used to protect the confidentiality of sensitive information.

### Types of Encryption

| Type | Description | Common Use |
|------|-------------|------------|
| Symmetric Encryption | Uses the same secret key for encryption and decryption. | Encrypting files, databases, and stored data |
| Asymmetric Encryption | Uses a mathematically related public and private key pair. | Key exchange, digital signatures, and public-key encryption |

## 2. Hashing

Hashing converts input data into a fixed-length value called a **hash** or **message digest**.

A cryptographic hash function is designed to make it computationally impractical to recover the original input from its hash or to find two different inputs with the same hash.

Common applications include:

- Verifying file integrity.
- Detecting unexpected data modifications.
- Supporting digital signatures.
- Securely storing passwords using dedicated password-hashing algorithms.

Examples of cryptographic hash algorithms include SHA-256 and SHA-384.

**Important:** Hashing is not encryption. It is designed to be a one-way operation and does not use decryption to recover the original data.

## 3. Digital Signatures

A digital signature is a cryptographic mechanism used to verify the authenticity and integrity of digital information.

The sender signs data using a private key, and the recipient verifies the signature using the corresponding public key.

Digital signatures help establish:

- **Authenticity:** Verifies that the signature corresponds to the expected signing key.
- **Integrity:** Detects changes to the signed data.
- **Evidence of Signing:** Supports accountability by linking a signature to a particular key.

Digital signatures do not automatically encrypt the signed data or guarantee the identity of the signer; identity assurance depends on how the signing key is associated with that person or organization.

## 4. Digital Certificates and PKI

A digital certificate is an electronic document that binds an identity to a public key. Certificates commonly use the X.509 format.

A **Public Key Infrastructure (PKI)** is a framework of technologies, policies, and processes used to issue, manage, validate, and revoke digital certificates.

Key components include:

- **Certificate Authority (CA):** Issues and signs digital certificates.
- **Digital Certificate:** Associates an identity with a public key.
- **Public and Private Keys:** Support cryptographic operations such as authentication and digital signatures.
- **Certificate Validation:** Checks certificate trust, validity period, and other relevant conditions.

Certificates are widely used to establish trust in HTTPS connections and other secure communications.

## 5. TLS and Encryption in Transit

Transport Layer Security (TLS) is a cryptographic protocol used to protect communications between systems.

TLS helps provide confidentiality, integrity, and authentication during communication, depending on the configuration and authentication method used.

Common applications include:

- HTTPS connections to websites and APIs.
- Secure communication between applications and services.
- Encrypted connections to supported databases.
- Secure communication between clients and cloud endpoints.

**Encryption in transit** protects information while it travels across a network, reducing the risk of interception or unauthorized modification.

## 6. Encryption at Rest

Encryption at rest protects stored data, including files, database records, storage volumes, and backups.

Cloud services may provide encryption capabilities that use provider-managed keys or customer-managed keys.

Examples in AWS include:

- Amazon S3 server-side encryption.
- Amazon EBS volume encryption.
- Amazon RDS encryption.
- AWS Key Management Service (AWS KMS) for managing supported encryption keys.

Encryption at rest helps protect stored information, but it does not replace access controls, secure configuration, or appropriate key management.

## 7. Key Management

Cryptographic keys must be protected throughout their lifecycle because unauthorized access to a key may compromise the data or operations it protects.

Key management includes:

- Key creation and storage.
- Access control and key usage permissions.
- Rotation and replacement where appropriate.
- Monitoring and auditing key usage.
- Revocation, disabling, and deletion according to security requirements.

AWS Key Management Service (AWS KMS) provides managed capabilities for creating and controlling cryptographic keys used by supported AWS services and applications.

## References

- [AWS Key Management Service Documentation](https://docs.aws.amazon.com/kms/)
- [AWS Encryption SDK](https://docs.aws.amazon.com/encryption-sdk/latest/developer-guide/introduction.html)
- [AWS Certificate Manager](https://docs.aws.amazon.com/acm/latest/userguide/acm-overview.html)
- [AWS Security Documentation](https://docs.aws.amazon.com/security/)
