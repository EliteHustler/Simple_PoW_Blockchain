# Simple PoW Blockchain 🪙

![GitHub release (latest by date)](https://img.shields.io/github/v/release/EliteHustler/Simple_PoW_Blockchain?style=flat-square)
![GitHub issues](https://img.shields.io/github/issues/EliteHustler/Simple_PoW_Blockchain?style=flat-square)
![GitHub forks](https://img.shields.io/github/forks/EliteHustler/Simple_PoW_Blockchain?style=flat-square)
![GitHub stars](https://img.shields.io/github/stars/EliteHustler/Simple_PoW_Blockchain?style=flat-square)

Welcome to the **Simple PoW Blockchain** repository! This C++ program showcases a basic blockchain implementation using OpenSSL for SHA-256 hashing. Each block in the chain holds transaction data, a timestamp, and a nonce. The program employs proof-of-work to mine blocks with a defined difficulty target.

## Table of Contents 📚

1. [Introduction](#introduction)
2. [Features](#features)
3. [Getting Started](#getting-started)
4. [How It Works](#how-it-works)
5. [Code Structure](#code-structure)
6. [Installation](#installation)
7. [Usage](#usage)
8. [Contributing](#contributing)
9. [License](#license)
10. [Contact](#contact)

## Introduction

Blockchain technology has transformed how we think about data integrity and security. This project demonstrates a simplified version of blockchain mechanics, focusing on proof-of-work mining. With this implementation, you can see how blocks are created, linked, and secured using cryptographic techniques.

## Features

- **Basic Blockchain Structure**: Understand how blocks connect to form a chain.
- **SHA-256 Hashing**: Leverage OpenSSL for secure hashing.
- **Proof-of-Work**: Implement a mining mechanism that requires computational effort.
- **Transaction Data**: Store and manage transaction information.
- **Timestamping**: Record when each block is created.

## Getting Started

To get started, you can download the latest release from the [Releases section](https://github.com/EliteHustler/Simple_PoW_Blockchain/releases). This link will take you to the necessary files for execution.

## How It Works

### Blockchain Basics

A blockchain is a series of blocks that store data. Each block contains:

- **Data**: Transaction details.
- **Timestamp**: When the block was created.
- **Nonce**: A number used in the mining process.
- **Hash**: A unique identifier for the block, created using the SHA-256 algorithm.

### Proof-of-Work

Proof-of-work (PoW) is a consensus mechanism that requires miners to solve complex mathematical problems. This process ensures that creating new blocks requires significant computational resources, making it difficult for malicious actors to alter the blockchain.

### Mining Process

1. **Create a Block**: Initialize a new block with transaction data.
2. **Calculate Hash**: Use SHA-256 to generate a hash.
3. **Adjust Nonce**: Increment the nonce until the hash meets the difficulty target.
4. **Add to Chain**: Once mined, the block is added to the blockchain.

## Code Structure

The project consists of several key files:

- `main.cpp`: The entry point of the program.
- `block.h`: Defines the Block class.
- `block.cpp`: Implements the Block class methods.
- `chain.h`: Defines the Blockchain class.
- `chain.cpp`: Implements the Blockchain class methods.
- `utils.h`: Contains utility functions, including hashing.

## Installation

To install the program, follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/EliteHustler/Simple_PoW_Blockchain.git
   cd Simple_PoW_Blockchain
   ```

2. **Install OpenSSL**:
   Make sure you have OpenSSL installed on your system. You can usually install it via your package manager.

   For Ubuntu:
   ```bash
   sudo apt-get install libssl-dev
   ```

   For macOS:
   ```bash
   brew install openssl
   ```

3. **Compile the Program**:
   Use the following command to compile the code:
   ```bash
   g++ main.cpp block.cpp chain.cpp -o blockchain -lssl -lcrypto
   ```

## Usage

After compiling, you can run the program:

```bash
./blockchain
```

The program will display the blockchain's status, including the mined blocks and their hashes.

## Contributing

We welcome contributions! If you would like to contribute to this project, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Commit your changes.
4. Push to your branch.
5. Open a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For questions or feedback, please reach out to the repository owner. You can also check the [Releases section](https://github.com/EliteHustler/Simple_PoW_Blockchain/releases) for updates and new features.

---

Explore the world of blockchain with this simple implementation. The concepts you learn here can serve as a foundation for more complex systems. Happy coding!