# Token Quantity
125,000,000

# Abstract
"Voi Observer" - a block explorer that fulfills the published ["Block Explorer" bounty](https://github.com/VoiNetwork/governance/blob/5c4da0252513d5e91daaabd577f5cbe96d40d337/Bounties/Block%20Explorer.md).

Will support networks:

- Voi Testnet
- Voi Mainnet (when launched)
- Algorand Betanet
- Algorand Testnet
- Algorand Mainnet

# Team 

Bit @ D13.co - You can find my [Algorand CV Here](https://docs.google.com/document/d/1XMQ-4RzkK_BCcLlg77kA7Dk_c3JyWgfB2NtnBpN9oH0).

# Problem Description 

We need a good block explorer. Dappflow is nice but falls short in a few areas, notably mobile/responsiveness and level of detail on some views. The open-sourced version that we have access to is also not up to date with the current dAppflow.

# Solution Approach 

Develop my own ideal block explorer that attempts to surface _every available bit of information_ that a node or indexer will provide. And for Algorand: plug the hole that AlgoScan left when they shut down.

I will put heavy emphasis on the user experience:

- things that users copy often should have a copy button
- views should be reasonably easy to navigate even on mobile screens

Examples of advanced features that went away with the sunsetting of AlgoScan:

- Good support for account type identification (logic sig, multisig, rekeyed, etc)
- Reverse lookup from contract escrow account -> application ID
- Working support for multisig signatures on a txn level (e.g. both [AlgoExplorer](https://algoexplorer.io/tx/7AVW5OHN5AJQLAU3NJXVSQDXQMPW5AN7NULDHFVBJPPUB6APDELQ) and [dAppflow](https://app.dappflow.org/explorer/transaction/7AVW5OHN5AJQLAU3NJXVSQDXQMPW5AN7NULDHFVBJPPUB6APDELQ) fail to do this)

# Expected Impact & Outcomes for the Voi Community 

Within Voi, this will deliver a world-class explorer for users and developers to use. On Algorand, a good open-source explorer funded by Voi should garner a lot of "brownie points".

# Technical Approach

To be built in TypeScript utilizing the next.js framework.

I will aim to be able to provide server-side rendering, which is crucial for SEO.

# Define Success

For the most part, as defined in the [Bounty](https://github.com/VoiNetwork/governance/blob/5c4da0252513d5e91daaabd577f5cbe96d40d337/Bounties/Block%20Explorer.md):

1. Overview Dashboard
1. Address View
1. Blocks View
    1. Block View
1. Transactions View
    1. Transaction View
    1. **Transaction Effects View (could be same as above)**
1. Assets View
    1. Asset View
1. Apps View
    1. App View
    1. **Box views**
1. Network Switch
    1. Voi
        1. Testnet
        1. Mainnet
    1. Algorand
        1. Testnet
        1. Mainnet
        1. **Betanet**
1. UI
    1. Reactive design that works on devices of different dimensions
    1. Good UX with intuitive interactivity

Added to the original bounty list:

- Transaction Effects View
    - The transaction effects API is fairly recent, so no explorer currently utilizes it. Among other things, it is the only way to get information about box changes during a transaction call.
- Box Views
    - Boxes on Algorand are largely overlooked by explorers (except for dAppflow)
    - Support them with first-class pages
- Network: Algorand/Betanet

As a general guideline, I will deepen each view (compared to other explorers) to be able to view any kind of information that the node or indexer will provide.

# Stretch Goals

The following section was moved to a stretch goal on the original bounty after [my suggestion](https://github.com/VoiNetwork/governance/pull/6). The reason is that the statistics generation is almost a separate side-project, requiring infrastructure and a pipeline to publish this data periodically.

1. Statistics
    1. Top Accounts
    2. Top Statistics
        1. All
        2. Economics
        3. Accounts
        4. Transactions
        5. Assets

I would recommend that the bounty of 125M be split into 110M for the main explorer and 15M for the statistics stretch goal.

# Concerns

None.

# Project Longevity 

A design goal with the explorer will be to make it work with a vanilla indexer as much as possible.

Modifications to indexers are hard to replicate by third parties (and also can hide performance issues if not done with the utmost care)

Inevitably some data we may need to show (e.g. statistics, escrow account -> app ID reverse lookups) will require a custom data source. For these I will aim to provide the pipeline needed to generate them along with the project, so that anyone can replicate it and publish it elsewhere if needed.

# Project Length

I expect this to be in review-able state by end of Q4 2023, and delivered in Q1 2024.

# Additional Information

The domains that will host the explorer are already purchased - algorand dot observer and voi dot observer.
