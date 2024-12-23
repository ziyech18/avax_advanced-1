# Avalanche Subnet Creation and Deployment Guide

This guide provides step-by-step instructions on creating an Avalanche Subnet and deploying Solidity code on Remix using MetaMask as the provider.

## Prerequisites

- MetaMask installed in your browser
- Avalanche-CLI installed locally
- Remix IDE (https://remix.ethereum.org/)
- Basic understanding of Solidity and smart contract development

## Installation of Avalanche-CLI

To install the Avalanche-CLI, run the following command in your terminal:

```bash
curl -sSfL https://raw.githubusercontent.com/ava-labs/avalanche-cli/main/scripts/install.sh | sh -s
```

## Creating an Avalanche Subnet

1. **Run the Subnet Creation Wizard:**

   Choose a name for your Subnet (e.g., `mySubnet`) and execute the following command:

   ```bash
   avalanche subnet create mySubnet
   ```

   Follow the wizard to configure your Subnet parameters.

2. **Deploy the Subnet Locally:**

   Deploy your Subnet locally by running:

   ```bash
   avalanche subnet deploy mySubnet
   ```

   Select "Local Network" when prompted.

3. **Interact with Your Subnet:**

   Use the provided connection details to connect to your Subnet:

   - **RPC URL:**   http://127.0.0.1:9650/ext/bc/ctuayjPr34gRM7hK3NzobHVdBo6PCxVCC4CzzXkg6QxLtQmxj/rpc
   - **Funded address:**  0x8db97C7cEcE249c2b98bDC0226Cc4C2A57BF52FC with 1000000 (10^18)
   - **Network name:** mySubnet
   - **Chain ID:** 242003
   - **Currency Symbol:** ETHADVANCED

   Note: Add `--http-host=0.0.0.0` to the config if you want to allow API calls from other machines.

## Running Solidity Code on Remix with MetaMask Provider

1. **Open Remix IDE:**

   Visit [Remix IDE](https://remix.ethereum.org/).

2. **Connect to Avalanche Subnet:**

   In Remix, go to the "Deploy & Run Transactions" tab. Choose "Injected Web3" as the environment. Connect MetaMask to your Avalanche Subnet by selecting the appropriate account.

3. **Compile and Deploy Solidity Code:**

   Copy and paste your Solidity code (e.g., ERC20 and Vault contracts) into Remix. Compile the code, and deploy the contracts to the Avalanche Subnet using MetaMask.

4. **Interact with Deployed Contracts:**

   After deployment, you can interact with your contracts using the provided RPC URL and addresses.

Congratulations! You have successfully created an Avalanche Subnet, deployed Solidity code, and interacted with the deployed contracts using Remix with MetaMask as the provider.
**CODE WITH YAYAADHU
