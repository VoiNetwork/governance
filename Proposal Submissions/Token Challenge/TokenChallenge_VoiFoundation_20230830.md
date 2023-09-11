# Proposal Status

Draft

# Token Quantity

300MM (300,000,000) Testnet Tokens

# Abstract
As part of the incentivized testnet the Voi Foundation is going to be running a "Token Challenge" in the DeFi phase. 

This would entail incentivising users to create their own tokens on the testnet and have them try to achieved certain milestones and key metrics which would rank them against each other. 

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

We also believe that this will increase the amount of engagement on social media as people start discussion their tokens and try to increase their own following of said tokens.

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

Proposed Reslutions:
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

Each eligible token will receieve a certain amount of points for the following:
- Activity
- Engagement
- Market Value

Each holder of an eligible token then recieves a share of those points assigned to the eligible token dependent on how many of those tokens they hold.

## Maths

### Variables
- $T$ = Number of unique tokens in the game
- $t_i$ = A specific token, where $i$ ranges from $1$ to $T$
- $P(t_i)$ = Points that token $t_i$ can potentially earn
- $P_{activity}(t_i)$ = Points token $t_i$ gets based on specific activities involving the token
- $P_{engagement}(t_i)$ = Points token $t_i$ gets based on user engagement
- $P_{market}(t_i)$ = Points token $t_i$ gets based on its market value or demand
- $O_{u,t_i}$ = Ownership fraction of user $u$ for token $t_i$
- $R$ = Total rewards available
- $P_u$ = Total points earned by user $u$
- $P_T$ = Total points available in the game

### Formulas
Total points for a specific token:
- $P(t_i) = P_{activity}(t_i) + P_{engagement}(t_i) + P_{market}(t_i)$

User's points from a specific token:
- $p_{u,t_i}$ = $O_{u,t_i}$ $\times$ $P(t_i)$

Total points user earn from all tokens:
- $P_u = \displaystyle\sum_{i=1}^{T} p_{u,t_i}$

Total points available in the game:
- $P_T = \displaystyle\sum_{i=1}^{T} P(t_i)$

User's share of the total rewards:
- $R_u = \left(\frac{P_u}{P_T}\right) \times R$
