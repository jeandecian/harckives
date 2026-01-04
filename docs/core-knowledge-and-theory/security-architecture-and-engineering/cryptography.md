# Cryptography

## What is Cryptography?

Cryptography is the science of securing information by transforming it into a format that is unreadable to unauthorized users. It ensures **confidentiality, integrity, authentication, and non-repudiation** of data, both at rest and in transit.

## Core Objectives of Cryptography

1. **Confidentiality:** Ensures only authorized parties can access the information.
2. **Integrity:** Guarantees that data has not been altered or tampered with.
3. **Authentication:** Verifies the identity of users or systems.
4. **Non-repudiation:** Prevents individuals from denying their actions (e.g., sending a message or transaction).

## Key Cryptographic Concepts

### Plaintext vs. Ciphertext

- **Plaintext:** Original, readable data.
- **Ciphertext:** Encrypted data, unreadable without decryption.

### Encryption and Decryption

- **Encryption:** Converts plaintext to ciphertext using an algorithm and a key.
- **Decryption:** Converts ciphertext back to plaintext using the same or a different key.

### Keys

- **Symmetric Key:** The same key is used for both encryption and decryption (e.g., AES, DES).
- **Asymmetric Key:** Uses a public key for encryption and a private key for decryption (e.g., RSA, ECC).

### Hashing

- Converts data into a fixed-length string (hash value) for integrity checks (e.g., SHA-256, MD5).

## Common Cryptographic Algorithms

| Type                  | Algorithm                | Use Case                                |
| --------------------- | ------------------------ | --------------------------------------- |
| Symmetric Encryption  | AES, 3DES, Blowfish      | Encrypting data at rest or in transit   |
| Asymmetric Encryption | RSA, ECC, Diffie-Hellman | Secure key exchange, digital signatures |
| Hashing               | SHA-256, SHA-3, MD5      | Data integrity, password storage        |
