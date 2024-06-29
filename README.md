# ETH-AVAX-PROOF-Intermediate-EVM-Course-Types-of-Functions-Project

**Introduction**

This Solidity contract implements a basic ERC20 token named `MyToken` using the OpenZeppelin Contracts library. It provides essential functionalities for creating your own custom token on the Ethereum blockchain.

**Description**

* **Standard:** ERC20
* **Functionality:** Ownable (minting and burning controlled by the contract owner)
* **Features:**
    * Minting of new tokens by the contract owner
    * Burning of tokens from the caller's account

**Deployment (Remix)**
* A development environment set up with Solidity and Remix.
**Steps:**
1. **Connect Remix to a Network:**
   * Open Remix ([https://remix.ethereum.org/](https://remix.ethereum.org/)).
   * In the left sidebar, click on the "Deploy & Run Transactions" tab.
   * Under "Environment," select "Injected Web3 Provider."

2. **Compile the Contract:**
   * Go to the "Solidity" compiler tab.
   * Ensure the correct compiler version (at least 0.8.0) is selected.
   * Click the "Compile `myERC20Tokken.sol`" button. If there are no errors, you'll see a green checkmark.

3. **Deploy the Contract:**
   * Go back to the "Deploy & Run Transactions" tab.
   * Select your `myERC20Tokken.sol` contract from the dropdown menu.
   * In the constructor arguments, enter the desired token name and symbol (e.g., "MyToken", "MTK").

4. **Initiate Deployment:**
   * Click the "Deploy" button. Connect your wallet and confirm the transaction.
   * Once successful, you'll see the deployed contract address

**Authors**
Vaibhav Sharma (vaibhavkhandal445@gmail.com)


**License**

MIT License
