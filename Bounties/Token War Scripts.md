# Token War Scripts

Testnet Token Bounty Size: 25MM to 75MM

## Description

For the token war we need a number of scripts developed so that we can calculate how many reward tokens an individual should get based on the rules of the game.

### What

A series of scripts that will query the Voi network among other data sources if necessary to process the necessary data to determine the following:

- Token Points
  -  Each eligible token scores points based on its performance in various KPIs. The better it performs, the more points it gets.
- Holder Points
  -  Holders of tokens are awarded a proportion of the points a token gets based on the number of tokens they possess.
- Rewards
  -  These points then dictate a holder's share of the reward pool.

More information can be found here:
https://github.com/VoiNetwork/governance/blob/TokenChallenge_VoiFoundation_20230830/Proposal%20Submissions/Token%20Challenge/TokenChallenge_VoiFoundation_20230830.md

### Why

These scripts are needed so that we can automate the allocation of points to tokens and users across the different battles and ultimately the war.

From these points we can then proceed to airdrop the appropriate amount of testnet rewards after each battle and after the end of the war.

## Problem Statement - what problem does this bounty solve?

This bounty solves the problem that the Token Wars success will depend on the necessary scripts being written so that we can automatically determine how many rewards each person is eligible for. 

The airdrop scripts are already written and just need to be provided what addresses are to receive what rewards.

## Expected Impact - what is the expected impact for Voi if this bounty is successfully completed? 

This will ensure the technical success of the Token Wars and the impact of that is more clearly outlined in it’s proposal.

## Minimum Requirements - what are the minimum requirements for this bounty? 

- At certain checkpoints (block number) the scripts need to run and query the network and other data sources.
- The scripts must be able to be run successfully for each battle and the entire war itself
- Assign weights to each KPI category and sub-category for each battle and the war for the points
- Retrieve the total circulating supply for tokens
- Retrieve the amount of tokens held by each user
- Retrieve relevant KPI data from chain or other data sources
- Process relevant KPI data for use in determining a tokens share of KPI points
- Determine each tokens share of points assigned to each KPI
- Determine each holder of each tokens share of points from that token
- Determine rewards earned by each holder across the entire battle or war
- Output the necessary input for the airdrop scripts to distribute the rewards to the users

## Stretch Goals - what is desirable, but not required that would enable someone to reach the upper limit of the bounty reward range 

- A war game dashboard

## Definition of Done - what does success look like when completed? 

- The scripts are fully functional and working and can output the correct and necessary input for the airdrop script to then distribute the rewards to the users.
