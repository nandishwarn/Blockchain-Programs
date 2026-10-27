[README.md](https://github.com/user-attachments/files/34006130/README.md)
# Blockchain Technology Lab Manual — BIC702

A collection of Blockchain Technology laboratory experiments for **Semester VII**, based on the uploaded lab manual from **Yenepoya Institute of Technology (YIT), Moodabidri**.

## Overview

This repository is intended for learning and demonstrating core blockchain concepts through practical exercises involving Python, cryptography, Ethereum smart contracts, wallets, token management, and Hyperledger Fabric.

## Experiments

The manual covers the following practicals:

| No. | Experiment | Main tools / concepts |
|---:|---|---|
| 1 | Generate public and private keys using OpenSSL | OpenSSL, RSA, PEM keys |
| 2 | Develop a basic blockchain | Python, SHA-256, blocks, transactions, proof of work |
| 3 | Develop and test a smart contract on a local blockchain | Solidity, Remix IDE, Ganache, MetaMask |
| 4 | Develop and test a smart contract on an Ethereum test network | Solidity, Remix IDE, MetaMask, Sepolia |
| 5 | Design and develop a multi-user cryptocurrency in Python | Python, transactions, balances, block mining |
| 6 | Set up Hyperledger Fabric and prepare to deploy chaincode | Hyperledger Fabric, Docker, WSL2, Ubuntu |
| 7 | Write a Solidity contract to transfer Ether from a contract to another account | Solidity, Remix IDE, MetaMask |
| 8 | Create and manage a token on Ethereum | Solidity, token balances, transfers, Sepolia |
| 9 | Set up MetaMask and create a wallet using a test network | MetaMask, wallet setup, Sepolia test ETH |
| 10 | Implement a blockchain using Merkle Trees | Python, hashing, Merkle roots |
| 11–12 | Additional practicals listed in the manual | Check the corresponding manual sections for details |

> **Note:** The manual's table of contents lists additional practicals, including setting up a Hyperledger Fabric network with two organizations and one peer each. Refer to the manual for the exact procedure and code for each experiment.

## Requirements

Install only the tools needed for the experiment you want to run. Depending on the practical, you may need:

- Python 3
- OpenSSL
- Visual Studio Code or another code editor
- MetaMask browser extension
- Remix IDE: https://remix.ethereum.org
- Ganache for local Ethereum development
- Docker Desktop
- Windows Subsystem for Linux 2 (WSL2) and Ubuntu for Hyperledger Fabric
- Access to the Ethereum Sepolia test network and a supported test-ETH faucet

Tool versions and network interfaces may change. Check the official documentation if a setup step in the manual no longer matches your installed version.

## Getting Started

1. Clone or download this repository.
2. Open the project folder in your terminal or code editor.
3. Navigate to the experiment you want to run.
4. Install the relevant prerequisite tools.
5. Follow the experiment's code and procedure from the lab manual.
6. Run the program or deploy the contract in the specified local/test environment.
7. Verify the output and record your observations.

### Running Python experiments

For Python files, use Python 3 from a terminal. For example:

```bash
python filename.py
```

On some systems, use:

```bash
python3 filename.py
```

Replace `filename.py` with the actual script name in the repository (for example, `mini_crypto.py` or `merkle_blockchain.py`, if those files are present).

### Generating keys with OpenSSL

If the repository contains the key-generation script from Experiment 1, make it executable on Linux/macOS and run it:

```bash
chmod +x generate_keys.sh
./generate_keys.sh
```

The script may prompt you to protect the private key with a passphrase.

### Smart-contract experiments

For the local-chain and Ethereum testnet exercises:

1. Open the relevant `.sol` file in Remix IDE.
2. Select a Solidity compiler version compatible with the source code.
3. Connect Remix to Ganache for local testing or MetaMask with Sepolia for testnet deployment.
4. Deploy the contract and approve transactions only after checking the selected network and transaction details.
5. Test the contract functions and verify the results.

## Security Notes

- **Never share your MetaMask Secret Recovery Phrase or private keys.**
- Do not commit private keys, wallet passwords, `.env` files containing secrets, or real credentials to GitHub.
- Use **test networks and test ETH** for practice. Do not use real funds for lab experiments.
- Importing a private key from Ganache should be limited to a disposable local development account.
- Smart contracts in this repository are educational examples, not audited production contracts. Review and test code before deployment.
- The Python blockchain and cryptocurrency examples are simplified learning implementations; they are not production-ready financial systems.

## Suggested Repository Structure

Organize your files in a structure like this, adjusting names to match the files you actually upload:

```text
blockchain-technology-lab/
├── README.md
├── experiment-01-openssl-keys/
│   └── generate_keys.sh
├── experiment-02-python-blockchain/
│   └── blockchain.py
├── experiment-03-local-smart-contract/
│   └── Storage.sol
├── experiment-04-sepolia-smart-contract/
│   └── SimpleStorage.sol
├── experiment-05-python-cryptocurrency/
│   └── mini_crypto.py
├── experiment-06-hyperledger-fabric/
├── experiment-07-ether-transfer/
│   └── BalanceTransfer.sol
├── experiment-08-token-management/
│   └── SimpleToken.sol
├── experiment-09-metamask-test-wallet/
└── experiment-10-merkle-tree/
    └── merkle_blockchain.py
```

This is a suggested layout, not a claim about the current repository contents.

## Learning Outcomes

After completing the practicals, students should gain introductory experience with:

- Public-key cryptography and key generation
- Block structure, hashing, and proof of work
- Smart-contract compilation, deployment, and interaction
- Local Ethereum development and testnet transactions
- Basic cryptocurrency transactions and balances
- Token creation and transfer logic
- Merkle Trees and Merkle roots
- The Hyperledger Fabric development environment

## Reference

- **Course:** Blockchain Technology
- **Course Code:** BIC702
- **Semester:** VII
- **Source:** Blockchain Technology Lab Manual, Yenepoya Institute of Technology (YIT), Moodabidri

---

If you use or adapt this material, follow your institution's academic-integrity guidelines and acknowledge the original lab manual where appropriate.
