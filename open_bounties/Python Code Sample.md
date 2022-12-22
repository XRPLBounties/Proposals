---
ID:
Discussion:
Category: Technical Documentation
Status: Open
Amount: $5500
---

# Python Code Samples 2

## Overview

Currently, our Python documentations have [code snippets](https://github.com/XRPLF/xrpl-py/tree/master/snippets) and [code samples](https://github.com/XRPLF/xrpl-dev-portal/tree/master/content/_code-samples) for some common usecases. However, there needs to be more examples to capture common tasks that users would want the library to do. Developers would benefit from additional relevant, high quality, well-documented examples in Python.

## Details

To add missing code samples, follow the instructions at the bottom of the page, under **Contribute Code Samples**.

https://xrpl.org/code-samples.html

## Milestones

| #   | Description              | Details                                                                                                                                                                                                    | Proposed Potential Award | Open? |
| --- | ------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------ | ----- |
| 1   | NFT                      | Mint (or batch mint) and burn an [NFT Token](https://xrpl.org/non-fungible-tokens.html#non-fungible-tokens-overview), assign an authorized minter, transfer NFT tokens (create, cancel, and accept offer). | $1000                    | Open  |
| 2   | Require Destination Tags | Enable [Require Destionation Tags](https://xrpl.org/require-destination-tags.html#require-destination-tags) for an account.                                                                                | $500                     | Open  |
| 3   | Use Tickets              | Prepare, sign , and submit [Tickets](https://xrpl.org/tickets.html#tickets) transactions.                                                                                                                  | $500                     | Open  |
| 4   | Decentralized Exchange   | Buy and sell tokens in the [decentralized exchange](https://xrpl.org/decentralized-exchange.html). Follow this [guidance](https://xrpl.org/decentralized-exchange.html) in JavaScript.                     | $500                     | Open  |
| 5   | Escrows History          | List the [Escrows](https://xrpl.org/escrow.html#escrow) on an existing account filtered by source and destination.                                                                                         | $500                     | Open  |
| 6   | Tickets                  | List which [Tickets](https://xrpl.org/use-tickets.html) are outstanding against one’s own account and use Tickets to collect signatures for multisign transactions.                                        | $750                     | Open  |
| 7   | Account Deletion         | Delete (or blackhole) an account.                                                                                                                                                                          | $500                     | Open  |
| 8   | NFTs                     | List an account’s [NFT pages](https://xrpl.org/nftokenpage.html#nftokenpage) and see token offers for that account’s NFTs.                                                                                 | $750                     | Open  |
| 9   | Memo                     | Validate and send a [Memo](https://xrpl.org/transaction-common-fields.html#memos-field).                                                                                                                   | $500                     | Open  |

When submitting a PR completing one of these milestones, please link to this markdown file for the bounty:

- A milestone is complete only after the relevant code sample has been approved, merged, and deployed onto XRPL.org.
- All of these code samples must have feature parity with the existing equivalent code samples in other languages.
- They must also be well-documented to be a useful learning reference, not just working code which performs the task.
