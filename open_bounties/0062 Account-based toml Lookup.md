---
ID: "0062"
Discussion: https://github.com/XRPLBounties/Proposals/discussions/0062
Category: XRPL.org tools
Status: Open
Amount: $2,500
---


# Proposal Title

Account-based toml Lookup Tools

**Category:**
XRPL.org tools


**Amount:** 
$2,500

## Overview

We'd like to create a tool to check if an account's Domain field is actually owned by them.

For context, the Domain field points to a website, and was originally intended to help show that a wallet is owned by a specific entity. Ex. Sologenic's wallet links to their website - https://bithomp.com/explorer/SOLO

There is already a tool on xrpl.org to do the reverse look up. It's called the "[xrp-ledger.toml checker on XRPL.org](https://xrpl.org/xrp-ledger-toml-checker.html)" and it verifies that a given website is owned by the same person who has a specific account on ledger.

In order to actually implement this, your tool should take in an account, look up the [Domain](https://xrpl.org/xrp-ledger-toml.html#domain-verification) field, and then see if that domain serves a properly formatted toml file claiming ownership of that account. (A process called Domain Verification)


Detailed steps requirement: 
- [ ] Write an Account-based toml lookup tool script similar to the existing [domain-based script](https://xrpl.org/xrp-ledger-toml-checker.html))
- [ ] Write tests for the script
- [ ] Integrate the script into https://xrpl.org/xrp-ledger-toml-checker.html with an additional input box and button for account-based lookup
- [ ] Make HTML/UI changes necessary to show two input boxes (one domain-based, one account-based) and connect the written script

All steps must be completed (reviewed and approved) together in a PR to claim the bounty. 


## Milestones

| # | Description | Proposed Potential Award | Open? |
| --- | --- | --- | --- |
| 1 | Complete all steps in the detailed requirements| $2,500 | OPEN |

## Helpful links/resources

xrpl.org issue ticket: https://github.com/XRPLF/xrpl-dev-portal/issues/576
