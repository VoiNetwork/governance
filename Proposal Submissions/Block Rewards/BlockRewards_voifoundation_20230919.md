
# **Token Quantity**

Total: 1,050,000,000

Block Rewards: 500,000,000

Ballast Nodes: 500,000,000

Node Seeds: 50,000,000


# **Abstract**

This proposal aims to distribute Voi tokens for the purposes of incentivizing block proposers, seeding healthy nodes, and ensuring network security through a foundation-managed staking mechanism. We propose a new, more equitable system for distributing tokens, geared towards enhancing the network's overall health and longevity.


# **Team**

Voi Foundation


# **Problem Description**


## Lack of Incentives for Block Proposers

Currently, the Voi network does not offer any token-based rewards for block proposers. While the goal of maintaining and protecting the network is a noble one, it may not provide sufficient motivation for participants to invest resources over the long term. The existing model limits the growth of the network and makes it susceptible to inefficiencies and vulnerabilities, especially in the early stages before reaching a critical mass of participation nodes.


## Node Health and Network Resilience

The network lacks a systematic way to incentivize node operators to maintain healthy nodes, leading to varying levels of network performance and reliability. Without a scoring and reward system, the network is at risk of hosting a plethora of underperforming nodes, which could compromise overall stability and security.


## Foundation's Role in Network Security

The foundation currently plays an undefined role in staking and running nodes. As a result, there's a vacuum in terms of a trusted entity providing a baseline level of security and stability for the network. The absence of a dynamic, automated staking strategy creates uncertainties that could make the network susceptible to attacks or failures.


# **Solution Approach**


## Introducing Daily Rewards for Block Proposers

To incentivize participation and resource investment, we propose introducing daily token rewards for block proposers. This system aims to distribute 500,000,000 tokens over a six-month period. Approximately 2.5 million tokens will be distributed each day. Block proposers will share the daily reward pool, which will be relatively split among the participants based on the number of blocks produced, excluding a blacklisted set of addresses for fairness and to avoid conflicts of interest.

**Key Features:**



* Transition from zero rewards to a daily reward system.
* Rewards distributed as a daily average among block proposers.
* Daily Distribution: Approximately 2.5 million tokens will be distributed among eligible block proposers each day relative to the number of blocks produced.
* Blacklisting mechanism to remove addresses, including those run by the foundation, to ensure fairness and avoid conflicts of interest.


## Seeding Healthy Node Runners Through Performance-Based Rewards

To improve the overall health and performance of nodes, we propose a 50,000,000-token fund to be disbursed to node operators based on their nodes' health scores. These scores will be captured in a snapshot once a week for the entire 6-month (approximately 26-week) testnet phase.

**Key Features:**



* Introduction of a node health scoring system: A score of 5 is considered the threshold for a 'healthy' node.
* Conditional rewards based on weekly snapshots: The total fund will be divided into weekly portions. Only nodes with a health score of 5 or above during the snapshot will receive their allocated bonus for that week.
* Weekly Snapshots: A snapshot of node health scores will be taken once a week to determine the bonus allocation for that week.


## Foundation-Led Staking for Enhanced Network Security

To ensure a base level of network security, we propose that the foundation stakes and runs nodes with a dynamic amount of 500,000,000 tokens. These tokens will be managed by bots that can adjust stakes dynamically, ensuring optimal network security while minimizing the risk of centralization.

**Key Features:**



* Foundation-managed staking to ensure a baseline level of security.
* Dynamic staking: Using bots to continuously adjust the stake, ensuring that the foundation’s nodes have enough stake to secure the network without having too much to risk centralization.
* Foundation-run nodes will be blacklisted from receiving rewards to avoid conflicts of interest.

# **Expected Impact & Outcomes for the Voi Community**



## Incentivized Block Proposing

The introduction of daily token rewards for block proposers is expected to:



* Increase the number of participants willing to act as block proposers.
* Improve the overall security and decentralization of the Voi network as more participants join.
* Encourage long-term commitment from block proposers, thereby increasing network stability.


## Elevated Node Health and Performance

The implementation of performance-based rewards for node runners is designed to:



* Encourage best practices in node maintenance, leading to a more robust and resilient network.
* Enhance the user experience through improved network performance and lower transaction times.
* Improve the average health score of nodes on the Voi network.

## Strengthened Network Security

The Foundation-led staking and blacklisting strategy aims to:



* Provide a stable and secure environment by injecting a substantial amount of staked tokens via foundation-run nodes.
* Mitigate the risk of network attacks or manipulations by dynamically adjusting the stakes.
* Ensure fairness in token distribution by blacklisting foundation-run nodes from rewards, thus avoiding conflicts of interest.

Overall, the proposed changes aim to create a more secure, stable, and equitable network that can sustain long-term growth and community engagement.


# **Technical Approach**


## Block Reward Distribution

For the distribution of daily rewards to block proposers, a JavaScript script will be developed to handle the process efficiently. The script will perform the following actions:



1. Analyze the day's block producers from the Voi blockchain data.
2. Exclude blacklisted addresses, such as foundation-run nodes, to maintain fairness.
3. Distribute the daily reward proportionally among the remaining eligible block producers based off the number of blocks produced.

The script will be open-source and hosted on GitHub for community review and contributions. The repository can be found at Voi Drops GitHub Repository(https://github.com/xarmian/voi_drops).

Tools and Technologies



* Language: JavaScript
* Data Source: Voi blockchain


## Node Health-Based Seeding

To evaluate node health and determine eligibility for seed rewards, telemetry data from nodes with telemetry enabled will be utilized. A snapshot of 7-day data will be taken to evaluate node health using the following website: Voi Proposer Data Health(https://cswenor.github.io/voi-proposer-data/health.html).



1. Capture 7-day node health data from nodes with telemetry enabled.
2. Assign rewards based on the node health scores, distributing tokens according to the criteria outlined in the "Solution Approach" section.

Tools and Technologies



* Data Source: Voi Proposer Health Data
* Analysis: Custom scripts or tools to capture and analyze the 7-day snapshot data.

# **Define Success**


The success of this proposal will be defined by achieving specific targets rather than measuring increases over an existing baseline.


## Block Reward Distribution



1. **Active Participation:** Attract at least 100 active block proposers within the first two months post-implementation.
2. **Security:** Zero major security issues or manipulations involving the new reward distribution within the first six months.
3. **Transparency and Community Engagement: **Positive community feedback and engagement.


## Node Health-Based Seeding



1. **Healthy Nodes:** Achieve at least 70 nodes with health scores of 5 or above within the first two months.
2. **Reliability:** Maintain network stability with no major outages or significant degradation in transaction times.
3. **Community Feedback:** Generate positive reviews and engagement from node operators regarding the new incentive system.


## Foundation-Led Staking for Enhanced Network Security



1. **Stability:** Maintain a network uptime of at least 99.9% post-implementation.
2. **Security:** Record zero successful attacks on the network attributable to staking imbalance or centralization issues.
3. **Fairness:** Adherence to the blacklisting policy for foundation-run nodes, ensuring they do not receive rewards.

In summary, success will be marked by the establishment of a secure, robust, and active Voi network with incentivized participation and a fair distribution system. 


# **Concerns**


## Security Risks Associated with New Reward Mechanisms



1. **Sybil Attacks:** With the introduction of node seeding, the network might be more susceptible to Sybil attacks where an entity creates multiple nodes to monopolize rewards.
2. **Manipulation of Health Scores:** As node health scores become tied to financial incentives, there's a risk of malicious actors finding ways to artificially inflate their scores.


## Centralization Risks



1. **Foundation-Run Nodes:** While foundation-run nodes are blacklisted from rewards to avoid conflicts of interest, their substantial stake in the network could still pose centralization risks if not appropriately managed.
2. **Large Stakeholders:** The introduction of block rewards might encourage accumulation of tokens by large stakeholders, potentially centralizing power and influence.


## Technical Challenges



1. **Bot Efficiency:** The use of bots to dynamically manage the foundation’s staking amount could encounter issues such as inaccuracies, delays, or vulnerabilities.
2. **Data Integrity:** Ensuring the accurate and secure storage of node health scores and other metrics poses a challenge, particularly if malicious actors attempt to tamper with this data.

By addressing these concerns proactively, we aim to implement the proposal in a way that mitigates risks and maximizes the benefit for the Voi community.


# **Project Length**

The implementation of this proposal is intended to coincide with the duration of the Voi testnet. Currently, we anticipate that this phase will span between 3 to 6 months. The key activities will include:



* Finalizing the technical approach for block reward distribution and node health-based seeding.
* Deploying initial versions on the testnet for live trials.
* Monitoring performance metrics and collecting community feedback.
* Making adjustments based on interim assessments and community input.

Should the testnet extend beyond the estimated 6 months, a new proposal will be drafted to address the ongoing needs and adjustments required for extended testing and evaluation.


# **Additional Information**


## Unused Tokens

In the interest of financial prudence and responsible governance, any unused tokens allocated for this project will be returned to the Voi treasury. This ensures that resources are efficiently utilized and can be allocated for future community projects or network improvements.


## Example Calculations

To give a clearer understanding of how the rewards and seed allocations work, example calculations for both are provided below.


### Block Rewards

With a daily distribution of 2.5 million tokens and 1,350 blocks produced in a day, the reward per block would be calculated as follows:



* Reward per Block = (2,500,000 Tokens) / (1,350 Blocks) = approximately 1,851.85 Tokens per Block

If a block proposer is responsible for 10 blocks that day, their reward would be:



* Reward for a Block Proposer = 10 Blocks x 1,851.85 Tokens per Block = 18,518.5 Tokens

In this example, the block proposer would receive approximately 18,518.5 tokens for successfully proposing 10 blocks on that day.

-  Daily Reward Pool: $R$

- Total Blocks Produced In Day $d$ : $B_{dailytotal}$

- Blocks Produced by Proposer in Day $d$: $B_{p}$

- Rewards for Proposer $r_p = R \times \left( \frac{B_p}{B_{dailytotal}} \right)$


### Node Seeding



1. Nodes with a score of 5 or above: 50,000,000 / 26 Weeks / 100 Nodes = ~19,230.77Tokens / Week 

These calculations are intended to serve as examples and actual numbers may vary due to dynamic factors.

- Total Reward for Nodes with a Score of 5 or Above: $R_{total}$

- Duration: $W$

- Number of Eligible Nodes: $N$

- Duration Reward for Each Node: $$R_{W} = \frac{R_{total}}{W \times N}$$


## Disclaimer

All numbers and calculations are subject to change at the discretion of the Voi Foundation. We will re-evaluate the rewards every month to see if they need to be adjusted.
