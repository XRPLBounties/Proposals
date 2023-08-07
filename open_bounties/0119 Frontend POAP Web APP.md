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
4. **XUMM Integration**: Incorporate XUMM wallet functionality for secure and user-friendly XRPL interactions.

## Benefits

1. **Developer Engagement**: Foster stronger XRPL developer communities through attendance tracking and rewards.
2. **Event Management**: Offer event organizers an efficient way to manage mailing lists and attendance registries.
3. **Talent Identification**: Enable startups/projects in the ecosystem to identify talented XRPL developers more easily.

## Detailed Requirements

In order to make a usable Proof of Attendance Protocol, we need a front end that can be used by event organizers and event attendees with minimal technical knowledge. A backend to handle key features like issuing NFTs, verifying ownership and such has already been completed, so this focuses on how to add a front end to make the tool usable. (Through this process, there may be updates to the backend)

Ultimately, there are three types of users:
1. Event organizers
2. Event attendees
3. The Admin / Tool Operator (needs technical expertise)

### Event organizers need to be able to
1. Create an event
2. Cancel an event
3. Get a link to share with attendees for attendees to redeem the NFT
4. See how many NFTs are minted / claimed
5. See who has claimed the NFTs
   - They also need to be able to search for an account via their wallet address

### Attendees need to be able to
1. Claim an NFT if they have the event link
2. Verify ownership of the NFT (to prove they’re the account holder)

### The Admin needs to be able to:
1. View all events on their platform
   - But shouldn’t have access to the links to redeem NFTs
2. Cancel any event on their platform
   - In order to free up their reserve requirements

**In order to implement these action items we expect to need several pages:**

An “Organizer Home” page where event organizers can log in and manage their events.
An “Organizer Event Details Page” which provides additional info on an event.
An “Attendee Event” page where attendees can go to claim an NFT (optional idea: this could be linked via QR code during the event as a way to distribute the link)
This would also have event-specific information if the organizer is logged in with their wallet.
An “Admin” page for the 3rd party operator (“Admin”) to configure things

### Organizer Home Page before Login

1. A clean and straightforward interface that welcomes users to the platform.
2. Button for "Organizer Login" Leading to XUMM wallet connection.

### Organizer Home Page after Login:
1. A welcoming personalized greeting, including the Organizer's account address.
2. Overview of the Organizer's created events: 
   - This could be a list or cards displaying essential information about each event (name, date, number of attendees, status).
   - The cards should indicate the status of the event
      1. Ongoing
      2. Completed
      3. Canceled
3. A way to “Create a New Event”
4. The "Create New Event" option should lead to a detailed form where the organizer can specify event details 
   - Start Date
   - End Date
   - Description
   - Graphic
   - Event ID
      - Which must be unique across all events to allow for looking up the event after the fact
   - The number of NFTs to create
5. At the bottom of the "Create New Event" form, there should be a live preview of the reserve required (preferrably with UI showing the formula being used to calculate + a link to the docs to avoid confusions around why the reserve is required).
6. Once paid, the NFTs should be created in the background. 
   - If the minting fails for whatever reason, the reserve should be returned to the Event Organizer.
7. After creating the NFTs, the page should automatically redirect to the detailed page for the event (which contains a link that can be shared with attendees for them to claim the NFTs)
8. Clicking an event should lead to a “Event Details Page for Organizers”


### Event Details Page for Organizers
1. A button to cancel the event
2. A record of how many NFTs were created, and how many have been claimed
3. A list of addresses which have claimed the NFTs
4. A link to the “Attendee Event” page which can be shared to attendees to allow them to claim the NFT
5. A record of how much XRP they have deposited with the Admin account to pay reserves

### Event Page for Attendees
1. The page should display event details (recorded from the “Create Event” form)
2. It should include the # of NFTs left to be claimed
3. It should also have a QR code attendees can use to claim the NFT via Xumm
   - Ideally there can be one QR code / website visual that can be put up on a screen, and all attendees can scan it to claim an NFT for themselves.

### Admin Page
1. The admin should have the ability to view all outstanding events, organized by event
2. They should also have the ability to cancel any outstanding events
3. They should also be able to see all organizers that have logged into the platform
4. There should be a live updating account balance
   - Next to that there should be a live updating reserve requirement
   - If they are close to running out of reserve, that should be indicated somewhere
5. They should be able to see a list of reserves provided from Event Organizers


### Additional Details (for specific features)

#### Canceling an event logic
1. Canceled events should have all unclaimed NFTs be burned to free up the reserve. 
2. They should also still appear in the “history” for events created by an event organizer, maintaining their detailed event pages so the event organizer can still look up who claimed NFTs before it was canceled. 
3. Canceled events should have a label saying “Canceled” in the list of events for an event organizer.
4. Events should be cancelable by both Event Organizers and Admins
5. The reserve, once freed, should be returned to the Event Organizer via a payment transaction.

#### Reserve Requirement math

```
Reserve Unit = 2 XRP
Average NFTs per NFTokenPage = 24 (https://xrpl.org/nftokenpage.html#reserve-for-nftokenpage-objects)
Normal # of tickets for event = 100

NFTokenPage Reserve = 2 * (100/24) = 8.33 = 10 XRP (Reserves round up)

Reserve for Tickets = 2 * Max Number of Tickets ~= 10 XRP - 500 XRP (one-time reserve for the admin)
NFTokenOffer Reserve = 2 * NFTokens (worse case) = 200 XRP (worst case)
```

## Milestones

| Milestone | Description | Budget Allocation | Open? |
|-----------|-------------|-------------------|-------|
| 1 | Creating the full front end | $10,000 | [In Review](https://github.com/XRPLBounties/POAP-APP/pull/2) |
