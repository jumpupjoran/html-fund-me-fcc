# Fund Me App

This project is a simple Ethereum-based DApp (Decentralized Application) that allows users to connect their wallet, fund a smart contract with ETH, check the contract's balance, and withdraw funds if they are the contract owner. The application uses MetaMask for wallet connection and the Ethers.js library to interact with the Ethereum blockchain.

## Table of Contents

-   [Fund Me App](#fund-me-app)
    -   [Table of Contents](#table-of-contents)
    -   [Project Structure](#project-structure)
    -   [Features](#features)
    -   [Prerequisites](#prerequisites)
    -   [Installation](#installation)
    -   [Usage](#usage)
    -   [Smart Contract Details](#smart-contract-details)
    -   [License](#license)

## Project Structure

-   **index.html**: Main HTML file with buttons for interacting with the DApp.
-   **index.js**: Contains JavaScript functions for connecting to MetaMask, funding, checking balance, and withdrawing.
-   **constants.js**: Holds the smart contract address and ABI.
-   **package.json**: Project dependencies.
-   **yarn.lock**: Lockfile for Yarn dependencies.

## Features

-   **Connect Wallet**: Connects user's MetaMask wallet.
-   **Fund Contract**: Allows users to send ETH to the contract.
-   **Check Balance**: Displays the current balance of the contract.
-   **Withdraw Funds**: Allows the contract owner to withdraw all funds.

## Prerequisites

-   **Node.js**: Ensure you have [Node.js](https://nodejs.org/) installed.
-   **MetaMask**: This application requires MetaMask for wallet interactions. Install MetaMask as a browser extension if not already done.

## Installation

1. Clone this repository:

    ```bash
    git clone https://github.com/yourusername/fund-me-app.git
    cd fund-me-app

    ```

2. Install dependencies:
    ```bash
    yarn install
    ```
3. Start a local server to serve the `index.html` file

## Usage

1. **Connect MetaMask**: Open `index.html` in a browser with MetaMask installed and click **Connect**.
2. **Fund Contract**: Enter the amount of ETH and click **Fund**.
3. **Check Balance**: Click **getBalance** to view the current contract balance.
4. **Withdraw Funds**: For contract owners, click **withdraw** to withdraw all funds.

## Smart Contract Details

The contract is deployed at the address specified in `constants.js`. Key methods include:

-   **fund()**: Allows anyone to fund the contract with ETH.
-   **withdraw()**: Restricted to the contract owner, enables withdrawing all contract funds.
-   **getBalance()**: Fetches the current contract balance.

## License

This project is licensed under the MIT License.
