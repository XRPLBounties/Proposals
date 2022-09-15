---
ID: 
Discussion: 
Category: Browser Extension
Status: Open
Amount: $100,000
---

# MetaMask Snap for the XRP Ledger

## Overview

[MetaMask](https://metamask.io/) is a gateway to blockchain apps with over 30 million users. With [Snaps](https://metamask.io/snaps/), developers can extend MetaMask to add additional features by leveraging existing APIs, such as the [XRP Ledger API](https://xrpl.org/public-api-methods.html). The Snap may also leverage JavaScript libraries such as [xrpl.js](https://github.com/XRPLF/xrpl.js) for functions like client-side key generation and transaction signing.

## Details

Develop, publish, and support an open source application allowing users to directly manage XRP and XRPL tokens within the MetaMask interface. The Snap should allow users to interact with XRP and XRPL tokens (on the XRP Ledger) without having to wrap tokens on Ethereum or any other blockchain.

Snaps is a system that allows developers to build on the capabilities of MetaMask. It is a program that can customize and modify MetaMask's experience for end users. This Snap must add new APIs to MetaMask and add support for the XRP Ledger blockchain. See the [MetaMask Docs about Snaps for more info](https://docs.metamask.io/guide/snaps.html).

As an example, the Snap would be similar to [BitcoinSnap](https://github.com/KeystoneHQ/btcsnap), but for the XRP Ledger.

## Milestones

| # | Description | Details | Proposed Potential Award |
| - | ----------- | ------- | ------------------------ |
| 1 | Create Account | Implement a Snap that securely generates and stores a new keypair and displays the associated XRPL address to the user. Make it easy for users to copy the address to share or use in other apps. | $1,000 |
| 2 | Send XRP | Enable users to send XRP. The Snap should sign and submit the transaction to a server of the user's choice. For convenience, users can select from one of the [well-known public servers](https://xrpl.org/public-servers.html). | $2,000 |
| 3 | View Transaction History | Show transaction history in a human-readable UI. | $10,000 |
| 4 | Set Trust Line | Enable users to [create or modify a trust line](https://xrpl.org/trustset.html). | $2,000 |
| 5 | Sign Anything | Enable users to sign any transaction or message. | $3,000 |
| 6 | Sign and Submit Transaction | Enable users to sign and submit any transaction. | $3,000 |
| 7 | Dapp Integration | Offer APIs for dapps to interact with the Snap. For an example, see the [API to integrate BitcoinSnap into your dapp](https://github.com/KeystoneHQ/btcsnap/tree/master/packages/snap). | $4,000 |
| 8 | Sample App | Build a sample app to showcase how to interact with the Dapp Integration milestone. | $5,000 |
| 9 | View NFTs | Enable users to see their XLS-20 NFTs directly within MetaMask. | $5,000 |
| 10 | Mint NFTs | Enable users to mint or sell a new NFT. | $7,000 |
| 11 | Ethereum Feature Parity | Add features similar or comparable to those available when using MetaMask with Ethereum. | Up to $50,000 |
| 12 | Xumm Feature Parity | Add features similar or comparable to those offered by [Xumm](https://xumm.app/). | Up to $50,000 |
