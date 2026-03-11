# Secure Information by Quantum Encryption for Sensitive Data

Hybrid Quantum–Classical Encryption Framework using BB84, AES-256, and HMAC Integrity Verification

---

## 📌 Overview

Secure communication remains a fundamental challenge in modern digital systems, particularly when transmitting sensitive information across untrusted networks. Classical cryptographic algorithms such as **AES-256** provide strong computational security, but their effectiveness depends entirely on the secure distribution of cryptographic keys. If the key exchange mechanism is compromised, the entire encryption framework becomes vulnerable.

This project presents a **hybrid quantum–classical encryption framework** that integrates **Quantum Key Distribution (QKD)** with classical encryption techniques to ensure secure data transmission. The system simulates the **BB84 quantum key distribution protocol** to generate a shared secret key between communicating parties. This key is then used within a classical cryptographic pipeline consisting of **AES-256 encryption** and **HMAC based integrity verification**.

By combining quantum secure key generation with classical encryption mechanisms, the framework demonstrates how **quantum communication principles can enhance practical cybersecurity systems**.

---

## ⚛️ Core Concept

The core concept of this project is the use of the **BB84 Quantum Key Distribution protocol** for secure key generation.

In the BB84 protocol, two communicating parties, commonly referred to as **Alice** and **Bob**, exchange quantum states encoded in different measurement bases. Due to the fundamental properties of quantum mechanics, any attempt by an eavesdropper to measure the quantum states introduces detectable disturbances.

This allows Alice and Bob to detect interception attempts and generate a **shared secret key with information theoretic security**.

Once the shared key is established, it is integrated into a classical encryption workflow:

1. **Quantum Key Distribution (BB84)** generates a shared secret key.
2. **AES-256 encryption** uses the generated key to encrypt sensitive data.
3. **HMAC verification** ensures the integrity of transmitted data.

This hybrid approach combines **quantum secure key exchange** with **efficient classical encryption algorithms**.

---

## 🏗 System Architecture

The system consists of three main modules.

### Module 1: Quantum Key Distribution (BB84)

This module simulates the **BB84 quantum key distribution protocol** to generate a shared secret key between Alice and Bob.

Example transmission process:
**Alice Bits**

[1, 1, 1, 1, 1, 0, 0, 1]

**Alice Bases**

[Z, Z, Z, Z, Z, X, X, Z]

**Bob Bases**

[X, Z, Z, X, Z, X, X, X]

**Bob Measurements**

[0, 1, 1, 1, 1, 0, 0, 1]

**Shared Key after Basis Matching**

[1, 1, 1, 0, 0]


After basis reconciliation, only the bits measured in matching bases are retained to form the final shared key.

---

### Module 2: Data Integrity Verification

This module implements **Hash Based Message Authentication Code (HMAC)** to verify the integrity of transmitted data.

If any modification occurs during transmission, the generated HMAC value will not match the original authentication code, allowing immediate detection of tampering.

---

### Module 3: AES-256 Encryption

The shared quantum key generated through BB84 is used to encrypt sensitive data using **AES-256 encryption**.

AES-256 ensures strong encryption while maintaining efficient performance for practical data protection.

---

## 📊 Evaluation Metrics

The performance and security of the system are evaluated using the following metrics.

### 1. Key Entropy
Measures the randomness of the generated quantum key. High entropy indicates strong unpredictability and improved cryptographic security.

### 2. File Size Ratio
Represents the ratio between encrypted file size and original file size, evaluating the overhead introduced by encryption.

### 3. Bit Match Ratio
Measures the agreement between Alice and Bob’s measurement results after basis reconciliation.

---

## 🔐 Security Testing

The system was evaluated under simulated adversarial conditions to assess its robustness.

Test scenarios include:

- Key tampering attempts
- Integrity verification failure
- Encrypted file corruption during transmission

These tests demonstrate that the **HMAC integrity layer successfully detects unauthorized modifications**.

---

## 🖥 Demonstration

A graphical user interface demonstrates the complete secure communication pipeline. The interface allows users to:

- Generate quantum keys using BB84 simulation
- Encrypt files using AES-256
- Verify data integrity using HMAC
- Simulate secure communication between sender and receiver

---

---

## 🚀 Applications

This hybrid quantum encryption framework can be applied in several critical domains including:

- Secure government communications
- Financial transaction protection
- Medical data security
- Critical infrastructure networks

Hybrid quantum–classical cryptographic architectures provide a **practical transition path toward future quantum secure communication systems**.

---

## 👥 Team

- Muhammad Osama
- Huma Sabir  
- Safoora Rana  
- Syed Aamir Abbas  
- Javeria Ashfaq  
- Fatima Afzal
  
## 👥 Mentors
- Dr. Malik Ahmad
- Dr. Shakir ullah
