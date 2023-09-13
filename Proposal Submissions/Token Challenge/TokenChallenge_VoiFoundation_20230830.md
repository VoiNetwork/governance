# Proposal Status

Community Review

# Token Quantity

300MM (300,000,000) Testnet Tokens

# Abstract
As part of the incentivized testnet the Voi Foundation is going to be running a "Token Challenge" in the DeFi phase. 

This would entail incentivising users to create their own tokens on the testnet and have them try to achieve certain milestones and key metrics which would rank them against each other. 

Both the creator and the hodlers would be eligible to receive testnet rewards in conjunction with this challenge.

The Voi Foundation would like to request the deployment of **300MM** testnet tokens for us to then subsequently airdrop as rewards to the participants of the Token Challenge.

# Team

Having worked on and founded Voi network The Voi Foundation has the perfect experience and expertise necessary to utilize the tokens granted to us via this proposal to execute on the Token Challenge.

Here are the teams twitter accounts for reference:
- https://twitter.com/bwhdx
- https://twitter.com/GovVoi
- https://twitter.com/ShanPurushotham
- https://twitter.com/chrisswenor
- https://twitter.com/algoJPEG
- https://twitter.com/JZYeyo

# Problem Description

The problem we are looking to solve is to increase engagement and participation from not only our existing community of Voiagers, but other networks such as Ethereum and Solana. 

We are looking to attract new users to our own community via their participation in the testnet.

# Solution Approach

The Token Challenge we feel will be a fun, engaging and rewarding way for new users to enter the ecosystem and to join our community. 

# Expected Impact & Outcomes for the Voi Community 

We envision this project to greatly benefit the community by creating more cohesion between existing members as well as by increasing the number of new members.

We also believe that this will increase the amount of engagement on social media as people start discussing their tokens and try to increase their own following of said tokens.

# Technical Approach

User created application tokens on the network will be eligible and we will use a number of off-chain scripts to perform chain analysis so that we can rank each token against different metrics and milestones.

Eligible users would then be airdropped their share of the testnet tokens granted by the committee for this proposal via another script.

# Define Success

Success will be ultimately determined by:

1. The increase in the number of unique wallet addresses that are actively participating in the challenge
2. The number of eligible tokens that join the challenge
3. The growth of our community in discord and twitter (X)
4. Increase levels of mentions and engagement of Voi on social media

# **Concerns** 

Concerns:
1. Getting the necessary scripts developed
2. Airdropping the rewards in a timely manner upon the conclusion of the challenge
3. Gaming of the system by actors

Proposed Resolutions:
1. Putting out a bounty for the necessary scripts to perform the chain analysis
2. Utilizing the existing Token Distribution Scripts
3. Designing the system in a way that it can be as sybil resistant as possible and adding applicable filters on the chain analysis scripts to ignore certain accounts that don't meet certain criteria to be deemed eligible.

# **Project Longevity**

This project is a one shot that would not require long term support beyond the conclusion of the challenge epoch and the distribution of the rewards.

# **Additional Information** 


For a token to be eligible it must have fulfilled the following criteria:
- Not be the Voi testnet native token
- Not be a Voi testnet token equivalent
  - For example a VSA distributed by the foundation that is otherwise equivalent in everyway to the native testnet token

## Token Wars: The Battle for Voi

In the vast digital realm of Voi, the newest frontier in decentralized finance, tokens abound with promises of innovation, utility, and growth. As Voi blooms and prospers, a burning question lingers: Amidst this sea of tokens, which will rise as the apex of activity, engagement, and market value? 

Welcome to the Token Wars, an epic 12-week odyssey where tokens clash for dominance and the coveted title of the Voi universe's champion!

### Overview
Spanning a period of 12 weeks, tokens will embark on 6 intense battles, each lasting a fortnight. Each skirmish will see tokens graded based on their key performance indicators (KPIs), earning points based on their activity, engagement, and market stature.

But here's the catch: the heart and soul of Voi – the Voiagers – play a pivotal role in the destiny of these tokens. As a Voiager, not only do you bear witness to these spectacular showdowns, but you also actively shape the outcome. The success of your chosen token is directly linked to the rewards you stand to gain. Rally your fellow Voiagers, partake in spirited activities, and steer your token to unparalleled heights!

### How It Works
Amidst the backdrop of Voi, tokens engage in combat, competing for the upper hand in a series of battles. At the conclusion of each battle, rewards are distributed to the Voiagers based on their token's performance and their stake in it.

The zenith of these clashes is the grand spectacle - The War. Here, tokens are sized up based on their sustained performance over the 12 weeks. The ultimate contest boasts its own reward pool, celebrating the tokens and Voiagers who've displayed unwavering commitment and tenacity.

A word to the wise Voiager: battles may be fleeting, but the war endures. Though points reset post-battle, for the war's spoils, every point secured during each battle is invaluable!

### Your Role as a Voiager
As a Voiager, the destiny of your token rests in your hands! Dive into activities that amplify your token's KPIs; as your token flourishes, so do your fortunes. With each battle and the grand war drawing to a close, bountiful rewards await Voiagers who champion and elevate their tokens.

The cosmos of Voi beckons, and the Token Wars are upon us. Which token will secure its place in the annals of Voi history? Which Voiager community will rally with unmatched fervor? Join this monumental quest and etch your name in the legacy of Voi!

### Summary

The Token Wars will last 12 weeks and consist of 6 battles each lasting 2 weeks.

There will be multiple KPIs used to simulate who is winning the battles and ultimately the war. 

Each eligible token will receive a certain amount of points for the following KPIs:
- Activity
- Engagement
- Market Value

Token points reset after each battle. However, for the final war reward, the token's performance across all battles are taken into consideration.

For each battle, a holder of an eligible token receives a share of that battle's points assigned to the token, based solely on that tokens battle performance and how many of those tokens they hold.

A holder then earns a share of the rewards available for that battle based on the points they have for that battle.

A holder of an eligible token also receives a share of the points assigned to the token over the entire war based on how many of those tokens they hold.

A holder then earns a share of the war rewards based on the points they have for the war.

**These rules, KPIs and point allocations may be updated or changed based on observed behaviors and feedback from the community.**

**The rewards will be awarded at the foundation's discretion.**
 
### Rewards

Rewards are distributed after each battle and at the end of the war to the players.

#### Battles

- Battle 1
  - **REDACTED** of Rewards
- Battle 2
  - **REDACTED** of Rewards
- Battle 3
  - **REDACTED** of Rewards
- Battle 4
  - **REDACTED** of Rewards
- Battle 5
  - **REDACTED** of Rewards
- Battle 6
  - **REDACTED** of Rewards

#### The War

- The War
  - **REDACTED** of Rewards

## Maths

The following would be applied to each battle and then ultimately the entire war.

### Variables
-  $T$ = Number of unique tokens in the round
-  $t_i$ = A specific token, where $i$ ranges from $1$ to $T$
-  $P(t_i)$ = Points that token $t_i$ can potentially earn
-  $P_{activity}(t_i)$ = Points token $t_i$ gets based on specific activities involving the token
-  $P_{engagement}(t_i)$ = Points token $t_i$ gets based on user engagement
-  $P_{market}(t_i)$ = Points token $t_i$ gets based on its market value or demand
-  $O_{u,t_i}$ = Ownership fraction of user $u$ for token $t_i$
-  $R$ = Total rewards available
-  $P_u$ = Total points earned by user $u$
-  $P_T$ = Total points available in the round

### Formulas
Total points for a specific token:
- $P(t_i) = P_{activity}(t_i) + P_{engagement}(t_i) + P_{market}(t_i)$

User's points from a specific token:
- $p_{u,t_i}$ = $O_{u,t_i}$ $\times$ $P(t_i)$

Total points user earn from all tokens:
- $P_u = \displaystyle\sum_{i=1}^{T} p_{u,t_i}$

Total points available in the round:
- $P_T = \displaystyle\sum_{i=1}^{T} P(t_i)$

User's share of the total rewards:
- $R_u = \left(\frac{P_u}{P_T}\right) \times R$

## Token KPIs

Here we will outline how each token is able to earn points. 

For each KPI there is a fixed number of points up for grabs. A token earns a larger share of these points by contributing more to the metric. There would be a cap on how many of the points a single token could earn in a particular sub-category, this will prevent too much dominance by a single token in a given category and encourage holders of such a token to focus on other areas of the game.

For example, if we have 1M points for transaction volume and there are 10000 transactions across all of the tokens, and token 1 consists of 5000 of them then token 1 would get assigned 500,000 points.

**REDACTED**

### Weightings

Each battle and the final war outcome would have 10,000,000,000 points up for grabs and each KPI category and their subcategories will have a weighting to determine their share of the total points of the battle or war that tokens can earn from it.

The weightings will be released ahead of time for the start of a battle and the war itself.

#### Example

Battle 1

- Activity - 4B points
  - **REDACTED**
- Engagement - 3B points
  - **REDACTED**
- Market Value - 3B points
  - **REDACTED**

### Caps

Each KPI subcategory will have a cap on the number of points that a token can earn from it, right now set to be **REDACTED**.

Any points over a KPI subcategory cap will be put aside into an unallocated points pool. 

New distribution percentages for each token not over the cap for each KPI subcategory will be calculated. 

This would be done by taking each token’s original contribution and normalizing it to exclude the contributions of the capped tokens.

The unallocated points will be distributed based on these new percentages for the tokens not over the cap.

This will be repeated until all points are allocated in the event that redistributing the points would cause other tokens to hit their cap.

#### Definitions:

- Let $n$ be the number of tokens in the KPI subcategory.
- $p_{total}$ is the total number of points for a KPI subcategory.
- $p_{i}$ is the proportional point allocation for token $i$ (before any capping considerations).
- $cap$ is the maximum number of points any token can get. 
- $c_{i}$ is the actual point allocation for token $i$ after considering the cap.
- $f_{i}$ is the fraction/proportional representation of token $i$.
- $u$ is the unallocated points after capping some tokens.

#### Steps:

- Calculate Initial Points:
  - $p_{i} = f_{i} \times p_{total}$ for $i = 1$ to $n$
- Apply the Cap
  - If $p_{i}$ > $cap$ then $c_{i} = cap$ else $c_{i} = p_{i}$
- Calculate Unallocated Points 
  - $u = p_{total}$ - sum of all $c_{i}$
- Redistribution
  - $newf_{i} = \frac{f_{i}}{1 - \text{sum of } f \text{ for capped tokens}}$
  - $redist_{i} = newf_{i} \times u$
  - Update $c_{i} = p_{i} + redist_{i}$
  - Check if any of these updated $c_{i}$ now exceed the cap. If they do, cap them and go back to step 3.
  - Each token $i$ gets $c_{i}$ points.

#### Example

Transaction Volume: 1,000,000,000 points
- Token A proportion: 60% (600,000,000 points)
- Token B proportion: 30% (300,000,000 points)
- Token C proportion: 10% (100,000,000 points)
- Cap: 50% (500,000,000 points)
- Token A gets capped at 500,000,000 points, leaving 100,000,000 points unallocated.
- These unallocated points are redistributed between Token B and Token C based on their proportions of the remaining uncapped total.
- New proportions excluding Token A:
  - Token B: 75% (of the uncapped total, i.e. 300,000,000 out of 400,000,000)
  - Token C: 25% 
- Redistribute the 100,000,000 points:
  - Token B gets 75,000,000 points
  - Token C gets 25,000,000 points 

Final points:
-  Token A proportion: 500,000,000 points
-  Token B proportion: 375,000,000 points
-  Token C proportion: 125,000,000 points

