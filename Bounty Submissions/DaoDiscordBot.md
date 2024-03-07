Title:
“DAO Bot - Algo Squirrel and DStain - 20240306”

Proposal Type:
Application

Proposal Category

DeFi
NFTs
Community

Token Quantity
25,000,000

Abstract

Countless AVM NFT communities have attempted to operate as DAOs and failed due to a lack of accessible infrastructure. Current voting mechanisms, such as emojis or Google Forms, are inefficient, inaccurate, and fail to leverage on-chain data. To address this gap, we propose the development of a DAO Discord bot tailored to support AVM NFT communities and specifically, Voi’s ARC-72 standard. 
The proposed DAO Discord bot aims to provide a user-friendly interface for creating and configuring DAOs, enabling sophisticated voting mechanisms such as weighted voting and proposals based on collector holdings. With a focus on pristine user experience, the bot will streamline the process of DAO voting management, making it accessible to all members of the Voi community.

The expected positive impact of this project on the Voi community is significant. By providing accessible DAO infrastructure for MainNet launch, Voi is positioned to leverage its community centric values and develop into a premier blockchain for DAO creation and applications. Project leaders within the Voi ecosystem will have the flexibility to choose a level of decentralization that suits their needs through DAO bot, whether they opt for full DAO integration or prefer to disable holder proposals and solely utilize the weighted voting mechanism. We believe that creativity will be exemplified through building this original and unique project from scratch, serving as inspiration for others to pioneer solutions for the Voi community.

In conclusion, the development of a DAO Discord bot for the Voi community is poised to revolutionize DAO operations within the AVM NFT space. By providing accessible infrastructure and sophisticated voting mechanisms, this project will empower Voi projects to support the decentralized ethos of Web3.

Team
Algo Squirrel (Project Manager) has been active in the Algorand NFT space since 2021, as both a well known collectible NFT project founder ($ACORN) and the #1 Algorand NFT collector by portfolio value, per Asalytic. He has also led a full-stack development team in ideation and creation of an on-chain NFT rental platform. His Web2 background is rooted in business and finance. 

DStain (Technical Developer) has over a year of experience working on Discord bots and utilizing Python to retrieve data directly from the Algorand blockchain. He has developed bots for notable projects, such as AlgoKnitter, that leverage on-chain data in creative ways and require customized UI. Additionally, he has created a proprietary airdrop script which functions automatically for multiple projects. An extensive background in engineering equips him with the technical ability and problem solving skills to code complex products. He is also an active collector in multiple Algorand NFT communities. 

Problem Description
See Abstract.

Solution Approach
See Abstract and Technical Approach.

Expected Impact & Outcomes for the Voi Community
See Abstract.

Technical Approach

1. A 0 VOI transaction is used to verify wallet address ownership with a Discord Account which is recorded in the holder database. This method supports multiple wallet addresses from a single Discord Account.
2. To create a DAO, creators follow instructions to input various fields including the DAO Name, creator addresses, a list of excluded assets within those creator addresses, voting weights corresponding to each creator wallet, and holding requirements for users to propose DAO votes. These fields are saved into the database which can be easily accessed by any user who has ownership in that particular DAO. Utilizing the verification process in Step #1 above, DAO creation is limited to Discord Accounts that verified the relevant creator addresses.
3. After DAO creation, users can check which DAOs they hold membership and voting power in based on their wallet holdings. The wallet holdings are checked in real-time and cross-checked against the creator database, which holds a list of assets minted by creator wallets that are automatically retrieved from on-chain data during Step #2.
4. Users can vote on all member DAO proposals and propose their own votes if the holding requirements set in Step #2 are met. Voting proposal details and results are recorded in the database which is accessible by any member of that DAO.
   
Define Success

We define “success” as DAO bot being fully functional on TestNet with 5+ NFT projects in the #VoiGames Collective Server utilizing DAO bot in a meaningful way as proof of concept, with 2+ instances of a community proposed vote. “Success” also means satisfying the minimum requirements for the “ARC-72 Discord Bots” bounty as outlined below:
All bots that submit proposals to cover this bounty must at minimum:

Be easily installable in a discord server.
Be easily configured for each collection's needs.
Provide a level of value to the collection and its members.
Be easily uninstalled in a discord server.

Achieving “Success” status to us, as described above, means completion of all Proposal related obligations thus earning the proposed Bounty reward in its entirety.

Concerns & Risks

The primary risk we identified is that Discord may not be powerful enough to support all planned project features and that tradeoffs might need to be made between desired features and UX. We will carefully consider all potential tradeoffs throughout product design, development, and all stages of testing.

Prerequisite
No dependencies identified.

Project Longevity

We will continue to service DAO bot to keep it functional and consider additional features based on community feedback to enhance value. Projected overhead costs are insignificant and we do not anticipate any issues in supporting the bot long-term. The code will also be open sourced.

Project Length
We expect DAO bot to be fully functional on Voi TestNet by May 2024 and have begun development in anticipation of proposal acceptance.

Additional Information
N/A

