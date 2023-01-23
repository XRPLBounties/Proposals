<!-- Please update this title -->

# Xrpl-py Event Handler

<!--
Please include this line to ensure that no work is started prior to merging and budget approval
-->

Bounty proposals require 3+ technical approvals _and_ budget approval before they are available to be worked on. A proposal PR with 3+ ✅s is not fully approved if it has not been merged. The bounty is only ready to be worked on after the PR has been merged.

**Category: Client Library Feature**

<!--
Recommend a total value amount for the bounty, in U.S. Dollars. The exact amount will be determined by the approving committee and may be higher or lower than this recommendation.
-->

**Amount:** $2,500

## Overview

<!--
Please provide the context required to complete the bounty.

Questions you should answer here:
1. What is the high level explanation of this bounty? (1-3 sentences)
2. What problem is this solving?
3. What are the requirements for this solution?
-->

Xrpl.js currently allows you to subscribe to ledger updates ([as specified here](https://xrpl.org/subscribe.html)) - it'd be useful to allow that in xrpl-py as well.

This would involve creating an event handler which allows you to subscribe to multiple non-admin subscriptions (So you would NOT have to implement `.on(peer_status)` for example).

[This issue](https://github.com/XRPLF/xrpl-py/issues/290) has a lot of context, including a couple examples of how this could be implemented.

The final submission would have to be well-tested to be production ready.

## Milestones

<!--
Please split the bounty into smaller milestones with individual awards in the following template.
The first milestone should be the core functionality, while the rest can be useful add-ons.

| # | High-Level Description | Details | Proposed Potential Award |
| 1 | ... | ... | $... |

(The proposed amounts from milestones should add up to the amount listed at the top of the bounty proposal)
-->

| # | High-Level Description | Details | Proposed Potential Award |
| 1 | Make & test the event handler | Implement `.on(event_type, callback)`, `.off(callback)` to remove a callback, and `.request(cmd, callback)` as specified in [this issue](https://github.com/XRPLF/xrpl-py/issues/290) | $2500 |

## Helpful links/resources

<!--
Is there anything else that would be helpful for someone picking up this bounty to know about/reference?

Ex.
* Are there existing solutions to this problem which would be helpful to learn from?
* Are there open source projects which can be used as a reference?
* Are there particularly relevant documentation pages?
-->

- Originating issue: https://github.com/XRPLF/xrpl-py/issues/290
- Xrpl.js implementation: https://github.com/XRPLF/xrpl.js/blob/main/packages/xrpl/src/client/index.ts
- Types of subscriptions rippled supports: https://xrpl.org/subscribe.html#subscribe
