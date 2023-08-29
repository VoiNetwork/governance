# NFT Indexer

Testnet Token Bounty Size: **75MM to 125MM**

## Description

Voi & Algorand both need an NFT indexer for the ARC-72 smart contract based asset standard.

### What

We need an on-chain index with a public method that allows users to provide a wallet address and the indexer to return the ARC-72 assets that the wallet owns. 

### Why

To enable network wide support for the ARC-72 standard by different applications such as marketplaces and wallets.

## Problem Statement

There is currently no way to query the network to retrieve ARC-72 assets. We need to have a smart contract based indexer created that stores the appIds, keeps track of and is queryable for all of the ARC-72 assets that get minted on the network.

## Minimum Requirements

For use on both testnet & mainnet.

1. Supports [ARC-72](https://arc.algorand.foundation/ARCs/arc-0072) assets
2. Keep an up to date smart contract based index of ARC-72 assets & their ownership.
    1. Parse blocks or events in real time as they are created and detect ARC-72 asset transactions that would cause the indexer to need to be updated.
    2. Use [ARC-73](https://arc.algorand.foundation/ARCs/arc-0073) to detect newly created ARC-72 assets that correctly implement the defined interface.
3. Public method where input is a wallet address and output is the appIds of the ARC-72 assets owned by this address.
4. Deployed and working on:
    1. Voi
    2. Algorand 
5. Ensures that the [Public API](https://github.com/VoiNetwork/governance/blob/main/Bounties/Public%20API.md) can implement [ARC-74](https://arc.algorand.foundation/ARCs/arc-0074) ontop of the NFT Indexer.

## Definition of Done

- Successfully implemented the minimum features as per the minimum requirements
- 99.99% uptime for the duration of testnet
- Integrated into the Public API
- All code open sourced

