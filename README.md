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
