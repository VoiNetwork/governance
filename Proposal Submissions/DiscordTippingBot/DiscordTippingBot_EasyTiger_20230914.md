# Token Quantity
3,000,000 VOI

# Abstract
Discord Based Tipping Bot - Algo Leagues Bot is a full-featured tip bot that enables Discord slash commands for users to send assets/NFTs/tokens directly to other Discord users. It can also airdrop assets to Discord roles and “rain” assets on users actively chatting in a Discord channel. User assets are tracked off-chain in a database and are deposited to and withdrawn from the bot easily and reliably. Tipping bots promote engagement and make it easier to onboard new users to Voi across established Discord servers in the Algorand Community and elsewhere.

# Team
**Eddie Pabon** (AlgoLeaguesCreator) - Project Founder and Owner
**Rich Granata** (EasyTiger) - Developer
Developed, Promoted, and Supported Algo Leagues Bot across nearly 100 Discord servers to date.

# Problem Description
Even during testnet stages, chain activity and engagement are needed to promote enthusiasm. The network effects of social engagement should not be underestimated. When a user receives a tip/airdrop through a Discord bot, they will be inclined to discover and research the related project. For many, it may be their first exposure to Voi or the tokens on the network. They will find information on how to claim the tip to their own wallet and use it. The “rain” feature encourages active participation in Discord. It also contributes to distribution and availability of various tokens.

# Solution Approach
Discord bots allow users to engage with a blockchain before they are familiar with all of the nuances of it. Tips can be collected and redistributed in Discord to foster community collaboration. While some bots utilize clawback, Algo Leagues implements an easy-to-use, secure deposit and withdraw system with a shared wallet which enables gameplay and other bot services.

# Expected Impact & Outcomes for the Voi Community 
Many will find that Voi is familiar, active, and well supported in the Algorand Community. NFT collections and token projects need wide distribution to find success. A tipping bot facilitates onboarding and distribution.

# Technical Approach
Algo Leagues Discord bot (currently using Algorand) will be updated to support multiple networks including Voi. It is built using Typescript and runs continuously on AWS Elastic Beanstalk which is their “serverless” offering to deploy and run highly reliable NodeJs applications. The database is NoSQL also on AWS using DynamoDb known for its responsiveness, scalability, and flexibility. Many of the latest features of the Discord API are utilized including slash commands and ephemeral messaging via the latest stable DiscordJs package (v14).

# Define Success
Algo Leagues Bot will have a network selector added to support Voi Testnet (and later Mainnet) and continue to run at 99% uptime. During Testnet, projects competing in the “Token Wars” can utilize the bot to distribute tokens to new users. With about 1,000 active users of the bot on Algorand, expect to see several hundred of them receive a token drop and consequently withdraw it to their personal wallet on Voi (Multiple wallets per user are already supported). Several new users will decide to create their own tokens on Voi and drop them on others in their own Discord servers.

# Concerns
Still under development is the user preferences system that allows users to opt out of rain, @mentions, or certain tokens drops. Some users would prefer not to be “dusted” with unknown tokens so enabling those preferences will be important to maintaining a good user experience, especially when adding a new network into the mix.

# Prerequisite
Wallet support: To begin using an address for deposits and withdrawals, Algo Leagues typically requires that the user confirms that they own the registered address by sending a zero transaction to the bot with note containing a 4 digit PIN. Early in testnet, most transactions are being done via command line or a-wallet connections that can be complicated for regular users to set up. Until a mainstream wallet application is available, we will need to determine if this confirmation step is necessary and if so, the easiest way to complete it. Early on, Algo Leagues may just use NFD verification only.

# Project Longevity
Algo Leagues bot runs at low cost in the cloud and plans to be operational for the distant foreseeable future. Costs are covered by the sales of the Algo Leagues NFT collection. The Algo Leagues Coin (ALC) token is also accepted as payment for bot services such as adding new tokens, adding secondary addresses. More Algo Leagues Coin utility will be introduced as new bot services and game modes are introduced.

# Project Length
Development of support for multiple networks is already underway but once greenlighted, support for Voi should be available within 21 days.

# Additional Information
Email: admin@algoleagues.com
Website: https://www.algoleagues.com
Discord: https://discord.gg/Qxaywxajh4
X (Twitter): https://twitter.com/AlgoLeagues
NFT Primary Market: https://algogems.io/shops/algoLeagues/sales