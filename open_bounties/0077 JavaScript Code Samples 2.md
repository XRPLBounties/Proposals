---
ID: "0077"
Discussion: https://github.com/XRPLBounties/Proposals/discussions/77
Category: Technical Documentation
Status: Open
Amount: $8250
---

# JavaScript Code Samples 2

## Overview

Currently, our JavaScript documentations have [code snippets](https://github.com/XRPLF/xrpl.js/tree/main/packages/xrpl/snippets/src) and [code samples](https://github.com/XRPLF/xrpl-dev-portal/tree/master/content/_code-samples) for some common usecases. However, there needs to be more examples to capture common tasks that users would want the library to do, and fixes to outdated or misconfigured snippets. Developers would benefit from additional relevant, high quality, well-documented examples in JavaScript.

## Details

To add missing code samples, follow the instructions at the bottom of the page, under **Contribute Code Samples**.

https://xrpl.org/code-samples.html

## Milestones

| #   | Description                                                                                                                                   | Details                                                                                                                                                                   | Proposed Potential Award | Open? |
| --- | --------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------ | ----- |
| 1   | [Use Checks](https://github.com/XRPLF/xrpl-dev-portal/tree/master/content/_code-samples/checks/js)                                            | Create, cancel, sign, submit, and query Checks are using depreciated RippleAPI. Update them to use current implementation.                                                | $1000                    | Open  |
| 2   | [Escrow](https://github.com/XRPLF/xrpl-dev-portal/tree/master/content/_code-samples/escrow/js)                                                | Create, finish, and cancel [Escrows](https://xrpl.org/escrow.html) are using depreciated RippleAPI. Update them to use current implementation.                            | $1000                    | Open  |
| 3   | Airgapped wallet                                                                                                                              | Folow the same implementation on our Python [code sample](https://github.com/XRPLF/xrpl-dev-portal/tree/master/content/_code-samples/airgapped-wallet/py).                | $1500                    | Open  |
| 4   | Account Tokens                                                                                                                                | Show (issued / fungible) tokens and other objects owned by an account.                                                                                                    | $500                     | Open  |
| 5   | [Build a Wallet](https://github.com/XRPLF/xrpl-dev-portal/tree/ec25f6bbddf182550186406f85913014aa423f44/content/_code-samples/build-a-wallet) | Build a desktop wallet for the XRPL Ledger following this Python [demonstration](https://xrpl.org/build-a-desktop-wallet-in-python.html#6-domain-verification-and-polish) | $1000                    | Open  |
| 6   | Escrows History                                                                                                                               | List the Escrows on an existing account filtered by source and destination.                                                                                               | $750                     | Open  |
| 7   | Tickets                                                                                                                                       | List which [Tickets](https://xrpl.org/use-tickets.html) are outstanding against one’s own account and use Tickets to collect signatures for multisign transactions.       | $750                     | Open  |
| 8   | Account Deletion                                                                                                                              | Delete (or blackhole) an account.                                                                                                                                         | $500                     | Open  |
| 9   | NFTs                                                                                                                                          | List an account’s NFT pages and see token offers for that account’s NFTs.                                                                                                 | $750                     | Open  |
| 10  | Memo                                                                                                                                          | Validate and send a [Memo](https://xrpl.org/transaction-common-fields.html#memos-field).                                                                                  | $500                     | Open  |

When submitting a PR completing one of these milestones, please link to this markdown file for the bounty:

- A milestone is complete only after the relevant code sample has been approved, merged, and deployed onto XRPL.org.
- All of these code samples must have feature parity with the existing equivalent code samples in other languages.
- They must also be well-documented to be a useful learning reference, not just working code which performs the task.
