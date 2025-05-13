# Simple Blockchain in C++ using OpenSSL

This is a basic implementation of a blockchain system written in C++. It uses SHA-256 hashing via OpenSSL to simulate block creation and proof-of-work mining.

---

## Features

- Block structure with:
  - Index
  - Timestamp
  - Previous hash
  - Data (transaction info)
  - Nonce
  - Current hash
- SHA-256 hashing using OpenSSL
- Proof-of-Work mining with adjustable difficulty
- Genesis block creation
- Simple linear blockchain with data immutability

---

## Dependencies

- C++11 or later
- OpenSSL (for SHA-256)

---

##  Compilation

To compile the code, ensure OpenSSL is installed, then use:

```bash
g++ blockchain.cpp -o blockchain -lssl -lcrypto
```

---

## Note

Mining time may vary based on the system and difficulty level.

---
