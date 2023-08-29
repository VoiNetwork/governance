# Public API

Testnet Token Bounty Size: **75MM to 125MM**

## Description

Public API for applications to be able to interact with the network without needing to run their own node.

### What

We need a public API that developers and applications can utilize in their code in order to submit transactions to the network or query it. 

A website that users can interact with to sign up to and generate their API keys from.

### Why

This is in order for developers and applications to interact with the Voi network in an easy and accessible way.

## Problem Statement

There is currently no publicly available API that developers and applications can use to interact with the network such as querying it or submitting transactions.

## Minimum Requirements

For use on both testnet & mainnet.


1. Website
    1. Login/Signup
    2. Dashboard
        1. API Key
        2. API Endpoints
        3. Usage data
    3. APIs
        1. Swagger UI Documentation
    4. Code Samples
        1. Example of using the API with the network SDK in different languages
            1. JS
            2. Python
            3. Go
            4. Java
            5. HTML
2. API
    1. Algod
        1. https://developer.algorand.org/docs/rest-apis/algod/ 
    2. Indexer
        1. https://developer.algorand.org/docs/rest-apis/indexer/ 
    3. NFT Index
        1. Support for on-chain [NFT Indexer](https://github.com/VoiNetwork/governance/blob/main/Bounties/NFT%20Indexer.md)


## Definition of Done

- Successfully implemented the minimum features as per the minimum requirements
- 99.99% uptime for the duration of testnet
- Integrated into the Extension Wallet if applicable
- Integrated into the Block Explorer if applicable
- Integrate the NFT Index
- All code open sourced

