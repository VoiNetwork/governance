# AMM

Testnet Token Bounty Size: **75MM to 125MM**

## Description

Voi needs an AMM Dex such as Tinyman or Humble to enable users to buy/sell fungible assets.

### What

Voi needs an AMM Dex to facilitate the swapping of fungible tokens and to enable users to independently setup the swap pools and provide liquidity to these pools.

### Why

This is crucial to enable DeFi. Users must be able to swap different fungible assets in a decentralized way and be able to provide liquidity to pools to earn fees for providing value to the Dex and it's users.

## Problem Statement

There is currently not enough AMM Dexs on Voi to support our DeFi scene.

## Minimum Requirements

A web app for use on both testnet & mainnet of Voi.

1. Supports appropriate assets
    1. ASAs
    2. [ARC-200](https://github.com/algorandfoundation/ARCs/blob/8fecd9127cfa70b49179a3e4b74212a0186b344b/ARCs/arc-0200.md)
2. Ability for user to connect their wallet via [Browser Extension Wallet](https://github.com/VoiNetwork/governance/blob/main/Bounties/Browser%20Extension%20Wallet.md)
3. Views
    1. Home/Swap
        1. Sign In / Connect Wallet
        2. Statistics
        3. Popular/Trending Swap Pools
        4. Choose Swap Pools
            1. From
            2. To
    2. Pool
        1. Your positions
            1. Add liquidity
            2. Remove liquidity
        2. All Pools
            1. Add liquidity
    3. Rewards/Fees
        1. Collect fees
    4. Network Switch
        1. Testnet
        2. Mainnet
4. AMM facilitated via smart contract for all supported assets
5. Cross standard asset swaps supported (ASA to ARC-200)
6. Link to assets on the [block explorer](https://github.com/VoiNetwork/governance/blob/main/Bounties/Block%20Explorer.md)
7. Deployed and working on
    1. Voi
        1. Testnet
        2. Mainnet 

## Definition of Done

- Successfully implemented the minimum features as per the minimum requirements
- 99.99% uptime for the duration of testnet
- All code open sourced