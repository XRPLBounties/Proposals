<!-- Please update this title -->

# Code Sample For Airgapped Wallet

<!--
Please add a high level category of work.
Ex. Game Development, Open Source Tooling, Etc.
-->

**Category:** Technical Documentation

<!--
Recommend a total value amount for the bounty, in U.S. Dollars. The exact amount will be determined by the approving committee and may be higher or lower than this recommendation.
-->

**Amount:** $6,000

**Proposed programming language:** Python

## Overview

<!--
Please provide the context required to complete the bounty.

Questions you should answer here:
1. What is the high level explanation of this bounty? (1-3 sentences)
2. What problem is this solving?
3. What are the requirements for this solution?
-->

**Discussion:** https://github.com/XRPLBounties/Proposals/discussions/47 (Must Read for details)

## Milestones

<!--
Please split the bounty into smaller milestones with individual awards in the following template.
The first milestone should be the core functionality, while the rest can be useful add-ons.

| # | High-Level Description | Details | Proposed Potential Award |
| 1 | ... | ... | $ |

(The proposed amounts from milestones should add up to the amount listed at the top of the bounty proposal)
-->


| # | High-Level Description | Details | Proposed Potential Award |
| --- | --- | --- | --- |
| 1 | Keypair/Wallet management system | Generate an XRPL account and store it securely with a password feature built-in using a cryptography algorithm | $1,500 |
| 2 | XRP Payments | Decrypt the previously stored keypair on the filesystem by password and sign a Payment transaction | $1,500 |
| 3 | Transmit & Relay Transaction | **Efficiently** & **Securely** transfer a signed transaction blob from the airgapped machine and relay the Payment to a rippled node and verify Payment's validity  | $1,000 |
| 4 | Tutorial & Descriptions & Diagrams (R&D) | Research and write a proper documentation on the code sample's directory and explain all the components, its purpose and how it all works together to form a reliable & secure way to store a keypair | $2,000 |


The value of the proposal is determined by the amount of research and development put in place, researching & developing the code sample takes a considerable amount of time since the airgapped wallet's effectiveness is not determined by the code itself (to secure the keypair), it's the design and security practices behind the concept which gatekeeps the keypair without any way of compromising it.

Simplifying this to new developers on the ecosystem will give them a sense of why security is prioritized in applications which hold custody to cryptocurrencies & assets. 

All milestones on this Bounty must be fully reached with synchronization  since with one single feature missing (aka. 1 milestone not being accomplished), it won't work as an airgapped wallet requires all the proposed mechanics to work together:
1. Generate wallet and store securely (using cryptography in this case)
2. Sign a transaction and keep the fields complete (i.e. the last ledger sequence is high enough to keep up with ledger progress [+100 advancement])
3. Transmit the signed transaction blob in a secure channel *without* compromising or connecting the airgapped machine to a network (i.e using a QR code)
4. Relay the transaction to a rippled node and display the results

### Milestone 1 Details
>store it securely with a password feature built-in using a cryptography algorithm

Encrypting the keypair on the filesystem should look like this, where the password is used as a key to encrypt/decrypt the wallet creds:
```py
        kdf = PBKDF2HMAC(
            algorithm=hashes.SHA256(),
            length=32,
            iterations=100000,
            salt=salt
        )

        key = base64.urlsafe_b64encode(kdf.derive(bytes(password.encode())))

        crypt = Fernet(key)

        priv = crypt.encrypt(bytes(seed, encoding='utf-8'))
        seed = crypt.encrypt(bytes(seed, encoding='utf-8'))

        with open(get_path("/Wallet/seed.txt"), "w") as f:
            f.write(seed.hex())

        with open(get_path("/Wallet/private.txt"), "w") as f:
            f.write(priv.hex())
```


### Milestone 3 Details
>**Efficiently** & **Securely** transfer a signed transaction blob

By "securely", do not compromise the airgapped machine with any unreliable channels which includes wired, bluetooth, or local network solutions.

It is best to use a QR code solution as it only transfers the necessary information from the airgapped machine to the outside party.

Example:

<img src="https://user-images.githubusercontent.com/87929946/196018292-f210a9f2-c5f8-412e-98c1-361a72286378.png" width=20% height=20%>
(Scan me, it's just a signed_tx blob)

## Helpful links/resources

<!--
Is there anything else that would be helpful for someone picking up this bounty to know about/reference?

Ex.
* Are there existing solutions to this problem which would be helpful to learn from?
* Are there open source projects which can be used as a reference?
* Are there particularly relevant documentation pages?
-->

- https://en.wikipedia.org/wiki/Air_gap_%28networking%29
- https://www.howtogeek.com/687792/the-ultimate-defense-what-is-an-air-gapped-computer/
