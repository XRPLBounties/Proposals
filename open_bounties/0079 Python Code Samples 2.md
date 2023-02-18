---
ID: 0079
Discussion: https://github.com/XRPLBounties/Proposals/discussions/79
Category: Technical Documentation
Status: Open
Amount: $5,000
---

# Python Code Samples 2

## This will not be merged until we receive budget approval even if we get 3+ technical approvals. Once merged, this bounty is ready to be worked on, please hold off starting work till merging. ##

## Overview

Currently, our Python documentations have [code snippets](https://github.com/XRPLF/xrpl-py/tree/master/snippets) and [code samples](https://github.com/XRPLF/xrpl-dev-portal/tree/master/content/_code-samples) for some common usecases. However, there needs to be more examples to capture common tasks that users would want the library to do. Developers would benefit from additional relevant, high quality, well-documented examples in Python.

## Details

To add missing code samples, follow the instructions at the bottom of the page, under **Contribute Code Samples**.

https://xrpl.org/code-samples.html

## Milestones

| #   | Description              | Details                                                                                                                                                                                                    | Proposed Potential Award | Open? |
| --- | ------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------ | ----- |
| 1   | NFT                      | Mint (or batch mint) and burn an [NFT Token](https://xrpl.org/non-fungible-tokens.html#non-fungible-tokens-overview), assign an authorized minter, transfer NFT tokens (create, cancel, and accept offer). | $1500                    | Closed  |
| 2   | Require Destination Tags | Enable [Require Destionation Tags](https://xrpl.org/require-destination-tags.html#require-destination-tags) for an account. Clarification: This should add a 'Python' tab for each step of the tutorial on xrpl.org.                                                                              | $500                     | Open  |
| 3   | Decentralized Exchange   | Buy and sell tokens in the [decentralized exchange](https://xrpl.org/decentralized-exchange.html). Follow this [guidance](https://xrpl.org/trade-in-the-decentralized-exchange.html) in JavaScript.                     | $500                     | Open  |
| 4   | Tickets                  | List which [Tickets](https://xrpl.org/use-tickets.html) are outstanding against one’s own account and use Tickets to collect signatures for multisign transactions.                                        | $750                     | Closed  |
| 5   | Account Deletion         | Delete (or blackhole) an account.                                                                                                                                                                          | $500                     | Closed  |
| 6   | NFTs                     | List an account’s [NFT pages](https://xrpl.org/nftokenpage.html#nftokenpage) and see token offers for that account’s NFTs.                                                                                 | $750                     | Closed  |
| 7   | Memo                     | Validate and send a [Memo](https://xrpl.org/transaction-common-fields.html#memos-field).                                                                                                                   | $500                     | Closed  |

When submitting a PR completing one of these milestones, please link to this markdown file for the bounty:

- A milestone is complete only after the relevant code sample has been approved, merged, and deployed onto XRPL.org.
- All of these code samples must have feature parity with the existing equivalent code samples in other languages.
- They must also be well-documented to be a useful learning reference, not just working code which performs the task.
