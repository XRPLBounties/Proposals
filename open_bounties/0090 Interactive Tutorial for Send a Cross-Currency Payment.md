---
ID: "0090"
Discussion: https://github.com/XRPLBounties/Proposals/discussions/0090
Category: Interactive Tutorials 
Status: Open
Amount: $2,000
---


# Interactive Tutorial for Send a Cross-Currency Payment
Bounty proposals require 3+ technical approvals _and_ budget approval before they are available to be worked on. A proposal PR with 3+ ✅s is not fully approved if it has not been merged. The bounty is only ready to be worked on after the PR has been merged.

## Overview

### High Level Description
Build an interactive tutorial for sending a cross-currency payment on xrpl.org, reference issues [here](https://github.com/XRPLF/xrpl-dev-portal/issues/1198)

### requirements
1. Write quality code samples in Javascript that shows steps to send a cross-currency payment, including: 
    - [ ] Pathfinding.
    - [ ] Setting reasonable `SendMax` values
    - [ ] Have to pay for any transfer fees plus the spread on Offers
    - [ ] Choose between multiple source currencies based on cost/liquidity
    - [ ] Troubleshooting (`tecPATH_DRY` / `tecPATH_PARTIAL` in particular)
    - [ ] using `DeliverMin` and partial payments to achieve a "fixed sending amount" cross-currency payment (rather than the default, "fixed receiving amount" payment)
2. Make the code samples interactive, instructions [here](https://github.com/XRPLF/xrpl-dev-portal/blob/master/tool/INTERACTIVE_TUTORIALS_README.md)

* Both requirements need to be completed(reviewed, approved and merged) to claim this bounty.

## Milestones

| # | High-Level Description | Details | Proposed Potential Award |
| 1 | Code Samples | Finish all the bullet points listed in requirement #1 - code samples  | $1000|
| 2 | Interactive tutorials | Make the code samples interactive | $1000|


## Helpful links/resources
Reference Doc: https://xrpl.org/cross-currency-payments.html#cross-currency-payments
Xrpl.org Issue Ticket: https://github.com/XRPLF/xrpl-dev-portal/issues/1198
Interactie Tutorials: https://github.com/XRPLF/xrpl-dev-portal/blob/master/tool/INTERACTIVE_TUTORIALS_README.md