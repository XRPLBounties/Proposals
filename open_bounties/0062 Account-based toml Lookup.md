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

The [xrp-ledger.toml checker on XRPL.org](https://xrpl.org/xrp-ledger-toml-checker.html) is a handy tool for looking up what accounts are claimed by a specific domain ([including domain verification](https://xrpl.org/xrp-ledger-toml.html#domain-verification)), but it could be convenient to be able to do it the other way around and check to see if an account really is claimed by the domain it has set in its Domain field.

So in addition to being able to put in a domain and verify the toml from there, you could put in an account to verify that account's domain: if it has a Domain field, you look up to see if that domain serves a toml file and if that toml claims ownership of the account.


Detailed steps requirement: 
1. Account-based toml Lookup Script:  Write an  Account-based toml lookup tool script similar to the existing domain-based script (https://github.com/XRPLF/xrpl-dev-portal/blob/master/assets/js/xrp-ledger-toml-checker.js), and add appropriate tests.
2. XRPL.org Web Changes : Integrate the script into https://xrpl.org/xrp-ledger-toml-checker.html with an additional input box and button for account-based lookup, make HTML/UI changes necessary to show two input boxes (one domain-based, one account-based) and connect the written script from milestone 1 to the page

Both steps must be completed (reviewed and approved) together in a PR to claim the bounty. 


## Milestones

| # | Description | Proposed Potential Award | Open? |
| --- | --- | --- | --- |
| 1 | Step 1 in the requirements above | $2,000 | OPEN |
| 2 | Step 2 in the requirements above | $500 | OPEN |

## Helpful links/resources

xrpl.org issue ticket: https://github.com/XRPLF/xrpl-dev-portal/issues/576
