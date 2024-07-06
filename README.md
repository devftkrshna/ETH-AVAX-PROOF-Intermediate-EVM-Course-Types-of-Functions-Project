# MyToken: A Custom ERC20 Token with Minting and Burning Functionality

## Table of Contents

- [Overview](#overview)
- [Description](#description)
- [Features](#features)
- [Getting Started](#getting-started)
  - [Deploying and Interacting with the Contract](#deploying-and-interacting-with-the-contract)
  - [Minting Tokens](#minting-tokens)
  - [Burning Tokens](#burning-tokens)
- [Help](#help)
  - [Common Issues](#common-issues)
- [Authors](#authors)
- [License](#license)

## Overview

MyToken is a custom ERC20 token with built-in minting and burning functionalities. It leverages the OpenZeppelin library for secure and reliable smart contract development.

## Description

MyToken is designed to provide flexibility for token management on the Ethereum blockchain. It allows the contract owner to mint new tokens and any token holder to burn their own tokens. This functionality is essential for various decentralized applications (dApps), including reward systems, staking mechanisms, and decentralized finance (DeFi) platforms.

## Features

- **ERC20 Compliance**: Implements the standard ERC20 interface for seamless integration with Ethereum-based applications.
- **Minting**: Allows the contract owner to create new tokens and assign them to specific addresses.
- **Burning**: Enables token holders to reduce the total supply of tokens by burning them permanently.
- **Security**: Built using the OpenZeppelin library, ensuring robust security standards and best practices in smart contract development.

## Getting Started

### Deploying and Interacting with the Contract

1. **Compile and Deploy the Contract**:
   - Upload the `MyToken.sol` file to Remix (https://remix.ethereum.org/).
   - Compile the contract using the Solidity compiler provided in Remix.

2. **Deploy the Contract**:
   - Select the appropriate environment (e.g., JavaScript VM for testing, Injected Web3 for deployment).
   - Deploy the contract and note the deployed address.

3. **Interacting with the Contract**:
   - Connect a wallet to Remix (if using Injected Web3).
   - Use the provided UI or console to interact with the deployed contract.

### Minting Tokens

- **Owner can mint tokens**:
  ```solidity
  function mint(address to, uint256 amount) public onlyOwner {
      _mint(to, amount);
  }
  ```

### Burning Tokens

- **Token holders can burn their tokens**:
  ```solidity
  function burn(uint256 amount) public {
      _burn(msg.sender, amount);
  }
  ```

## Help

### Common Issues

- **Deployment Issues**: Ensure you have the correct environment selected in Remix (e.g., JavaScript VM for testing, Injected Web3 for deployment).
- **Minting Permission**: Only the contract owner can mint tokens. Verify the owner's address.
- **Burning Tokens**: Ensure you have enough tokens in your balance to burn.

## Authors

- Dominique Pizzie
  - GitHub: [DomPizzie](https://github.com/DomPizzie)
- Vaibhav Sharma
  - GitHub: [devftkrshna](https://github.com/devftkrshna)

## License

This project is licensed under the MIT License. See the LICENSE.md file for details.
