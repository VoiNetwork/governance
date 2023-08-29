# Algorand NFT Bridge

Testnet Token Bounty Size: **75MM to 125MM**

## Description

Voi needs an NFT bridge for Algorand.

### What

We need a simple NFT bridge that allows whitelisted NFTs to be transferred between Algorand mainnet and Voi testnet. 

### Why

The transferability of NFTs is going to be used as a way for testnet users to bring value on and off the network during the testnet so that the testnet tokens can be swapped for something of intrinsic value that can then be further swapped for mainnet tokens on destination networks. 

## Problem Statement

There is currently no way to bridge NFTs from existing mainnet networks onto Voi testnet and back again. Ideally done via decentralized bridging, but not necessary.

## Minimum Requirements

This will initially only be for Voi testnet to Algorand mainnet. 

However it should be designed and architected so it can be expanded upon to establish an NFT bridge between Algorand mainnet & Voi mainnet down the line. 

1. Ability to whitelist specified NFTs
    1. Only those on this list can be bridged in either direction.
2. Bi-Directional Bridging
    1. Users are able to bridge a whitelisted NFT from Algorand mainnet to Voi testnet
    2. Users are able to bridge a whitelisted NFT from Voi testnet to Algorand mainnet
3. Support the appropriate standards on either side of the bridge
    1. Algorand
        1. ARC-3
        2. ARC-16
        3. ARC-69
        4. ARC-72
    2. Voi
        1. ARC-72
4. Migration plan
    1. Upon completion of the incentivized testnet the bridge should migrate to be between Algorand Mainnet & Voi Mainnet. As such an executable plan must be put in place to enable this such that no assets are locked up on the Voi testnet in their wrapped form.

## Definition of Done

- Successfully implemented the minimum features as per the minimum requirements
- 99.99% uptime for the duration of testnet
- All code open sourced

