---
id: overview
title: Overview
---

For some more advanced use cases, it is necessary to use multiple tools in the Uniswap toolchain.

:::info
Already familiar with web3 development and/or the basics of our SDK and want to get right to the code? Start with our first guide, [Getting a Quote](./02-quoting.md)!
:::

## Providers

Communication with the blockchain is typically done through a provider and local models of smart contracts and their [ABIs](./01-background.md#abis).

To achieve this, our examples use the [ethers.js](https://docs.ethers.io/v5/) library. To instantiate a provider you will need a data source. Our examples offer two options:

- **JSON RPC URL**: If you are working directly with the Ethereum mainnet or a local fork, products such as [infura](https://infura.io/) offer JSON RPC URLs for a wide variety of chains and testnets. For our examples, we'll only be using the Ethereum mainnet.

- **Wallet Extension**: If you are connecting to a wallet browser extension, these wallets embed a source directly into the Javascript window object as `window.ethereum`. This object surfaces information about the user's wallets and provides the ability to communicate with the connected chain. Importantly for our examples, it can be used with `ethers.js` to construct a provider.

