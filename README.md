# Asymmetric Encryption Module

A Python module for asymmetric (public-key) encryption and decryption.

## Overview

This module provides easy-to-use asymmetric encryption capabilities using RSA or similar algorithms.

## Features

- 🔐 **Key Generation** — Create public/private key pairs
- 📤 **Encryption** — Encrypt data with public key
- 📥 **Decryption** — Decrypt data with private key
- 🔒 **Secure** — Uses industry-standard algorithms

## Installation

```bash
pip install -r requirements.txt
```

## Usage

```python
from asymmetric_encryption import AsymmetricEncryption

# Initialize
enc = AsymmetricEncryption()

# Generate key pair
public_key, private_key = enc.generate_keys()

# Encrypt message
message = "Secret message"
encrypted = enc.encrypt(message, public_key)

# Decrypt message
decrypted = enc.decrypt(encrypted, private_key)
```

## How It Works

1. **Key Generation:** Creates mathematically related key pair
2. **Encryption:** Public key encrypts, only private key can decrypt
3. **Security:** Based on difficulty of factoring large primes

## Use Cases

- Secure communication
- Digital signatures
- Key exchange protocols

## License

MIT

---

## CI Status

All PRs are checked for:
- ✅ Syntax (Python, JS, TS, YAML, JSON, Dockerfile, Shell)
- ✅ Secrets (No hardcoded credentials)
- ✅ Security (High-severity vulnerabilities)

