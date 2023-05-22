---
ID: 0119
Discussion: https://github.com/XRPLBounties/Proposals/discussions/119
Category: Community Tools, Events
Status: Open
Amount: $10,000
---

# Proof of Attendance Web App for XRPL Events

## Overview

Develop a user-friendly web app that allows event organizers to distribute attendance NFTs to participants at XRPL events, leveraging the previously developed [Proof of Attendance Infrastructure](https://github.com/XRPLBounties/Proof-of-Attendance) for the XRP Ledger. The web app will specifically utilize the API library provided by the Proof of Attendance Infrastructure for minting and distributing NFTs, as well as handling other related functionalities. Additionally, the web app will integrate with XUMM wallet for seamless XRPL interactions.

## Objective

Provide event organizers with a no-code tool for distributing NFTs for attendance at XRPL events, and track long-term attendance across the XRPL community.

## Core Features

1. **Event Creation**: Enable event organizers to create and manage events within the web app.
2. **NFT Distribution**: Utilize XLS-20 NFTs on XRPL and the backend [Proof of Attendance Infrastructure](https://github.com/XRPLBounties/Proof-of-Attendance) to distribute NFTs to attendees that meet the organizer's criteria for rewards or recognition.
3. **Attendance Tracking**: Allow event organizers to monitor long-term participation records of developers and enthusiasts, rewarding them for loyalty and granting access to additional resources.
4. **Identity Verification**: Collect names and emails to verify user identity and associate a wallet with an identity without requiring full KYC procedures.
5. **XUMM Integration**: Incorporate XUMM wallet functionality for secure and user-friendly XRPL interactions.

## Benefits

1. **Developer Engagement**: Foster stronger XRPL developer communities through attendance tracking and rewards.
2. **Event Management**: Offer event organizers an efficient way to manage mailing lists and attendance registries.
3. **Talent Identification**: Enable startups/projects in the ecosystem to identify talented XRPL developers more easily.

## Detailed Requirements

### Event Organizer Dashboard Features

1. Event organizer XRPL account set up/connection using XUMM Wallet
2. Mint/View/Distribute XLS-20 NFTs on XRPL (using [POAP Infrastructure](https://github.com/XRPLBounties/Proof-of-Attendance))
3. Create a token-gated campaign with properties below:
   - Allow specification of start date, end date, event descriptions, graphics.
   - Selection for NFTs used in the organizer to act as the gate; as the organizer will likely be minting NFTs for other purposes, we want to allow the organizer to select which specific NFTs will be used for this event
4. Distribution of NFTs to attendees
5. Attendee lookup and verification
6. Search module for attendees given their wallet address
7. Verification of NFT ownership using wallet signature.
8. *Stretch Requirement*: Create the ability for event organizers to blast email attendees

### Event Attendee Dashboard Features

1. Event attendee account set up using email address and names
2. Display widget to connect wallet for attendee (XUMM)
3. Claim attendance NFT's via XUMM
4. Apply reward to displayed coupons when NFT conditions are met by the wallet
5. *Stretch Requirement*: RSVP for future events

## Milestones

| Milestone | Description | Budget Allocation |
|-----------|-------------|-------------------|
| 1 | API Integration | $1,000 |
| 2 | UI/UX design wireframes | $1,500 |
| 2 | XUMM and GEM wallet integration | $1,000 |
| 3 | Event Organizer Dashboard Feature (8 detailed requirements above - $500 each) | $4,000 |
| 4 | Event Attendee Dashboard Features (5 detailed requirements above $500 each) | $2,500 |
