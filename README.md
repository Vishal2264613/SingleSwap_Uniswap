# Single Swap Uniswap

Welcome to the ** Single Swap Uniswap** repository! This project demonstrates how to execute a single token swap on the Uniswap decentralized exchange (DEX) using the Uniswap V3 protocol.

## Overview

Uniswap is a popular decentralized exchange built on the Ethereum blockchain. This project provides a simple example of how to perform a single swap between two tokens using Uniswap's smart contracts. 

## Features

- **Swap Functionality:** Executes a token swap from one token to another.
- **Gas Optimization:** Efficiently handles transactions to minimize gas costs.
- **Error Handling:** Includes basic error handling for common issues.

## Prerequisites

Before you begin, ensure you have the following:

- **Node.js** (v14 or higher)
- **npm** or **yarn** (package managers)
- **Ethereum Wallet** (e.g., MetaMask) with some ETH for gas fees
- **Infura** or **Alchemy** API key (for connecting to the Ethereum network)

## Installation

1. **Clone the repository:**

    ```bash
    git clone https://github.com/yourusername/uniswap-single-swap.git
    cd uniswap-single-swap
    ```

2. **Install dependencies:**

    ```bash
    npm install
    # or
    yarn install
    ```

3. **Configure your environment:**

    Create a `.env` file in the root directory and add the following variables:

    ```env
    INFURA_PROJECT_ID=your_infura_project_id
    WALLET_PRIVATE_KEY=your_wallet_private_key
    ```

    Replace `your_infura_project_id` and `your_wallet_private_key` with your actual Infura project ID and Ethereum wallet private key.

## Usage

To perform a single token swap, run the following command:

```bash
npx hardhat run --network <Network name> scripts/deploySingleSwap.js
```


### Example

To swap LINK for WETH, you might use:

1. Copy & paste code to Remix IDE.
2. Compile and deploy it at Address in remix by using the address of deployed contract on the network.
3. Send some Link token to your contract address on remix.
4. Pass swap exact amount in the first swapExactInputSingle function like (2000000000000000000).
5. then in swapExactOutputSingle function pass amountOut and amountInMaximum to perform the swap.
## Code Overview

- **`deploySingleSwap.js`**: Main script for executing the token swap. Contains logic for interacting with Uniswap's smart contracts.
- **`config.js`**: Configuration file for setting up Web3 and Uniswap contract instances.
- **`.env`**: Environment variables for sensitive information.

## Disclaimer

This project is for educational purposes only. Use it at your own risk. Make sure to test thoroughly and consider security implications when working with real assets.

---
