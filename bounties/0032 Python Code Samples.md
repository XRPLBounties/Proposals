---
ID: "0032"
Discussion: https://github.com/XRPLBounties/Proposals/discussions/0032
Category: Technical Documentation
Status: Open
Amount: $7,500
---

# Python Code Samples

## Overview

The XRP Ledger Dev Portal contains many [code samples](https://xrpl.org/code-samples.html), but some of them are not available in Python. Developers would benefit from additional relevant, high quality, well-documented examples in Python.

## Details

To add missing code samples, follow the instructions at the bottom of the page, under **Contribute Code Samples**.

https://xrpl.org/code-samples.html

## Milestones

| # | Description | Details | Proposed Potential Award | Completed? |
| --- | --- | --- | --- | --- |
| 1 | [Address Encoding](https://github.com/XRPLF/xrpl-dev-portal/tree/master/content/_code-samples/address_encoding) | Encode XRP Ledger addresses in base58. This sample can be pulled out of, or perhaps implemented within, an existing client library. | $500 | COMPLETED |
| 2 | [Escrows](https://github.com/XRPLF/xrpl-dev-portal/tree/master/content/_code-samples/escrow) | Create, finish, and cancel [Escrows](https://xrpl.org/escrow.html) using conditional or time-based release. | $1,000 | CLOSED |
| 3 | [Freezes](https://github.com/XRPLF/xrpl-dev-portal/tree/master/content/_code-samples/freeze) | Freeze and unfreeze issued tokens, check freeze status, or give up the ability to freeze tokens. | $1,000 | OPEN |
| 4 | [Monitor Incoming Payments](https://github.com/XRPLF/xrpl-dev-portal/tree/master/content/_code-samples/monitor-payments-websocket) | Watch for incoming payments to an XRP Ledger address, _without_ using a client library. | $1,000 | COMPLETED |
| 5 | [Require Destination Tags](https://github.com/XRPLF/xrpl-dev-portal/tree/master/content/_code-samples/require-destination-tags) | Require incoming payments to specify a [Destination Tag](https://xrpl.org/source-and-destination-tags.html) so you know whom to credit. | $1,000 | COMPLETED |
| 6 | [Submit and Verify](https://github.com/XRPLF/xrpl-dev-portal/tree/master/content/_code-samples/submit-and-verify) | Submit a signed transaction blob and wait until it has a final result. | $1,000 | COMPLETED |
| 7 | [Tickets](https://github.com/XRPLF/xrpl-dev-portal/tree/master/content/_code-samples/use-tickets) | Create a Ticket and use it to send a transaction out of the usual Sequence order. | $1,000 | COMPLETED |
| 8 | [Use Checks](https://github.com/XRPLF/xrpl-dev-portal/tree/master/content/_code-samples/checks) | Create, cash, and cancel Checks for exact or flexible amounts. | $1,000 | OPEN |

When submitting a PR completing one of these milestones, please link to this markdown file for the bounty:
https://github.com/XRPLBounties/Proposals/blob/main/bounties/0032%20Python%20Code%20Samples.md

- A milestone is complete only after the relevant code sample has been approved, merged, and deployed onto XRPL.org.
- All of these code samples must have feature parity with the existing equivalent code samples in other languages. 
- They must also be well-documented to be a useful learning reference, not just working code which performs the task.

**Ripple internal ID:** DGE-93
