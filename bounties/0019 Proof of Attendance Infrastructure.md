---
ID: "0019"
Discussion: https://github.com/XRPLBounties/Proposals/discussions/0019
Category: New Feature
Status: Open
Amount: $7,500
---

# Proof of Attendance Infrastructure

## Overview

Community Event Management Tool: Build a library to provide infrastructure that allows event organizers to mint and distribute Attendance NFTs on the XRP Ledger.

## Details

Create an API library that enables event organizers/developers in the XRPL community to distribute digital badges/collectibles NFTs minted on the XRPL Ledger using XLS-20(https://github.com/XRPLF/XRPL-Standards/discussions/46) for their events.
XLS-20 (native support for NFTs) is implemented in xrpl.js (https://github.com/XRPLF/xrpl.js) and xrpl.py (https://github.com/XRPLF/xrpl-py) and currently live on NFT testnet.

See similar infrastructure built on Ethereum https://poap.xyz/#

Basic requirements:

1. Given a minter - able to mint NFTs for all attendees with the same metadata and artwork (artwork should be hosted somewhere that's not XRPL).
   The NFT minted should include a memo/taxon field that include information about the event (date, location and description) and an artwork that represents the event.
2. Provide a gateway for attendees to collect the NFTs through their wallets or creating new wallets and distributing them securely.

## Milestones

| #   | Description                                        | Details                                                                                                                                        | Proposed Potential Award |
| --- | -------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------ |
| 1   | Create API library for NFT Minting and distrubtion | Complete basic requirements mentioned above with good documentation and tests.                                                                 | $3,000                   |
| 2   | Event attendees lookup                             | Add a way for people to look up wallets with the same event NFTs.                                                                              | $1,000                   |
| 3   | Event NFT ownership verification                   | Add an API for people to verify the event NFT - using their signiture to prove that they are the owner of the account associated with the NFT. | $2,000                   |
| 4  | Deployed no-code tool for non-technical event organizers                   | Add a frontend (preferably a form) with wallet integration (XUMM) for non-technical event organizers to mint and send event NFT's, the website should be deployed publicly | $1,500                   |

