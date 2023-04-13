---
ID: "0052"
Discussion: https://github.com/XRPLBounties/Proposals/discussions/0052
Category: eCommerce App
Status: Open
Amount: $17,000
---

<!-- Please update this title -->

# Shopify NFT App

## Overview

<!--
Please provide the context required to complete the bounty.

Questions you should answer here:
1. What is the high level explanation of this bounty? (1-3 sentences)
2. What problem is this solving?
3. What are the requirements for this solution?
-->

There are over 2.5 million merchants that use the Shopify platform. All of which use marketing in some form or another to drive sales. 

The goal of this app will be to give merchants a way to increase engagement through the use of NFTs (XLS-20). The actual marketing method is left up to the developer and the only requirement for this bounty is to use NFTs to incentivize customers to make further purchases or to increase engagement with the brand.

Example:
A customer would claim a random NFT via a QR code on their physical receipt or a link on their order confirmation page. Then upon collecting a certain set of NFT's that customer would trade them in for a discount or a free product.

Such an app would allow merchants to use NFTs in their business, strengthen their communities and explore what Web3 has to offer. It would also expose them to  the speed and efficiency of using XRPL.

## Awards Available
This bounty can have up to 3 Shopify apps that help merchants utilize XLS-20.

## Milestones

<!--
Please split the bounty into smaller milestones with individual awards in the following template.
The first milestone should be the core functionality, while the rest can be useful add-ons.

| # | High-Level Description | Details | Proposed Potential Award |
| 1 | ... | ... | $... |

(The proposed amounts from milestones should add up to the amount listed at the top of the bounty proposal)
-->

| # | Description | Details | Proposed Potential Award | Status |
| --- | --- | --- | --- | --- |
|1| Create | Create a Shopify app that uses XLS-20 NFTs on XRPL to drive sales and engagement for a merchant. Detailed requirements are listed below.| $5,000 | In Review |
|2| Launch | Submit and [launch the app on the Shopify app store](https://shopify.dev/apps/store/review) | $5,000 | Open |
|3| Adoption | Get 100+ installs | $5,000 | Open |
|4| Education (optional) | Open source repo for a Shopify app that at a minimum allows creating/viewing/deleting XLS-20 NFTs. This can be a barebones version of your app or an entirely different idea, but should serve as a teaching tool for other Shopify developers. | $2,000 | Open |

**Detailed requirements:**

Merchant dashboard features
- [ ] merchant XRPL account setup
- [ ] create/view/delete XLS-20 NFT on XRPL
  - Create a [token-gated campaign](https://www.shopify.com/ca/retail/token-gating) with properties below:  
  - [ ] allow specification of start date, end date and redemption limits
  - [ ] selection for NFTs used in the campaign to act as the gate; as the merchant will likely be minting NFTs for other purposes, we want to allow the merchant to select which specific NFTs will be used for this campaign
  - [ ] associate reward/promo for NFT(s) such as discount, BOGO and/or free product
  - [ ] selection of included products or collections to which the promo applies, as the merchant will likely have products they don't want discounted

Merchant storefront features
- [ ] display widget via [Shopify app theme extension](https://shopify.dev/apps/online-store/theme-app-extensions) to connect wallet
- [ ] apply promotion to displayed products when NFT conditions are met by the wallet

## Helpful links/resources

<!--
Is there anything else that would be helpful for someone picking up this bounty to know about/reference?

Ex.
* Are there existing solutions to this problem which would be helpful to learn from?
* Are there open source projects which can be used as a reference?
* Are there particularly relevant documentation pages?
-->
 
- https://shopify.dev/apps
- https://help.shopify.com/en/manual/products/digital-service-product/nfts
- https://help.shopify.com/en/manual/products/digital-service-product/nfts/blockchain-app-partners

## Helpful examples
[novel.com](https://www.novel.com/)

![TokenGateExample](https://user-images.githubusercontent.com/20135683/209374864-df336d9b-1582-4519-87fa-7e75297adbef.gif)

[^1]: In review means we have a received a submission for this milestone which is still in consideration, but we are providing feedback to. This does not mean they will necessary be awarded the milestone, but they do have existing work.
