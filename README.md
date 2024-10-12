# Register Smart Contract

This smart contract is a showcase created for the **Chainlink Certifications - Shenzhen 2024 Event**. It demonstrates a basic storage and retrieval mechanism using Ethereum smart contract technology.

**Event Link:** [Chainlink Certifications - Shenzhen 2024](https://lu.ma/CLL-SZ-Certifications)

## Contract Overview

The `Register` contract allows users to store and retrieve a string of information on the blockchain. It has two main functions:
- `setInfo(string _info)`: Stores a string value.
- `getInfo()`: Retrieves the stored string value.

The contract is deployed on the **Sepolia Testnet** at the following address:

**Contract Address:** `0xD0e295012F3b7891f992A861Ec56228294F898aC`

## Table of Contents
1. [Requirements](#requirements)
2. [Usage](#usage)
3. [Deployment](#deployment)
4. [Testing](#testing)
5. [Security](#security)
6. [License](#license)

## Requirements

To interact with or modify this contract, you need the following tools:
- [Solidity 0.8.19](https://docs.soliditylang.org/en/v0.8.19/)
- [Node.js](https://nodejs.org/)
- [Hardhat](https://hardhat.org/) or [Truffle](https://trufflesuite.com/)
- [Ethers.js](https://docs.ethers.io/v5/) or [Web3.js](https://web3js.readthedocs.io/)
- A wallet like [MetaMask](https://metamask.io/) to interact with the Sepolia network

## Usage

### Interacting with the Contract

Once the contract is deployed on Sepolia, you can interact with it using any Ethereum wallet or dApp development framework (e.g., Hardhat, Ethers.js, or Remix).

#### Setting Information

To set the information, call the `setInfo(string memory _info)` function. This requires sending a transaction with a string parameter.

Example using Ethers.js:
```js
const contract = new ethers.Contract(contractAddress, abi, signer);
await contract.setInfo("Hello, Chainlink Certifications!");