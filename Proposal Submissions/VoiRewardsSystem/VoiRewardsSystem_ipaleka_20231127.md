# Token Quantity
42,000,000

# Abstract
This proposal brings a solution for every rewards token allocation inside the Voi Network in a fully transparent way. The creation of the periodical transparency reports should become a much easier task. It will also minimize the possibility of an error during the process, while all the community contributions will be rewarded fairly. Last but not least, it will bring much more involvement and a sense of belonging for the community members.

# Team
@kerr - The most active member in the ASA Stats GitHub issue tracker and the biggest contributor to the ASA Stats rewards system.

@AlgoRhythMatic - One of the creators of the ASA Stats rewards system which he administrates.

@ipaleka - ASA Stats founder and core developer.

@dragmz - The ASA Stats rewards system uses his script for the rewards allocation.

# Problem Description
Every blockchain project has to be 100% transparent. Just an intention and corresponding practice isn't enough to reach such a perfect score of 100% - people have to have insights into everything that is going on inside the project.

There are a lot of transactions from the official Voi Network accounts for various recipients and a variety of reasons. Probably there are people inside the core organization who can get a grasp of almost everything.

Besides periodical reward allocations like those for the node-runners or those for the accepted proposals, there are token allocations as rewards for the community members' exceptional tasks and/or deeds. The majority of the latter are random-based.

It is worth mentioning here that every bit of such information is lost in Discord void after a few minutes or hours.

On top of that, the Voi Network seriously lacks a system for the community members to be more involved and rewarded. Let's just give an example of how community members can contribute and be more involved in the project. This highly important Discord comment has a dead link: https://discord.com/channels/1055863853633785857/1146757961012748339/1146757961012748339. Right now, Voi Network does not have a clear and logical way to trigger fixing, and on top of that, it lacks the motivation for someone to trigger such a fixing.

# Solution Approach

This proposal brings a solution for every rewards token allocation inside the Voi Network in a fully transparent way.

Every rewardable task would be announced in a public space (Discord isn't really a public space) and every related rewards transaction would be that way justified/explained to everybody. For example, every node runner gets an entry for the related rewards allocation without much additional work added. The same goes for the accepted proposals.

In the case of the example from the previous section (fixing a dead link), here's a usual workflow:

a) a community member posts a comment in Discord explaining there's a dead link.  
b) another community member marks the original Discord comment with an emoji that means `noted`, creates an issue in the related Voi Github repo, and links the original comment (or, of course, in some other issue tracker if that fits the Voi Network better). In most cases, this person labels the related type for the issue (probably a `bug` in this case).  
c) a Voi community member with enough administrative privileges in Discord resolves the issue (fixes the dead link), labels the GitHub issue with something that means `addressed`, and sets the level of effort/involvement for the original reporter (an initial, first level for this example), closes the GitHub issue, and marks the original Discord comment with additional emoji that means `addressed`.  
d) once a week (or once or twice a month), a Voi official (let's call it the ceremony master) filters all the closed issues marked as `addressed` and creates the entries in the related Google Docs spreadsheet based on the issue type. In this example, the original reporter gets B1 entry (entry-level bug) and the issue creator gets IC1 (entry issue creation level task). After all of them are filled, a formatted list is created automatically in the spreadsheet. Btw, the Ceremony Master gets their own entry for their task done.  
e) The ceremony master publishes the list for the community members to discuss. A period of a few days is enough to adjust the level of involvement for every contributor if someone emphasizes a mislabeling back in the process (like B2 instead of B1, etc.)  
f) Finally, a core Voi team member saves the list and runs the related script that allocates rewards based on related *values* for the related labels. If some contributors haven't provided their public Voi addresses, the core team member reaches them in a private chat asking for the address (with a link to the cycle's discussion thread). The address is saved (in the private repo accessible only by the core team members) and the script is run against the new addresses/members.

# Expected Impact & Outcomes for the Voi Community
The implementation should completely expose the transparent nature of the Voi Network. Creating the monthly/quarterly transparency reports should become a much easier task. Other people will be able to search for the historical records and get a practical confirmation of the project's transparent nature.

The community members who are not involved in proposals and don't run nodes will be able to earn rewards and be more connected to the project.

The Voi Network will benefit from bigger community members involvement, an involvement that brings focus on exact problems.

People will be rewarded for their help to the project in a consistent and non-random way.

# Technical Approach
This process excels in Discord through the emojis in the comments. People seeing a unique related emoji leaves no doubt of the status of the request/report. A related discussion should outcome of the emojis design and types, and this proposal just defines a need for some of them, like `noted`, `addressed`, `already exists`, `not applicable`, etc.

Platforms like Twitter or Reddit don't have emojis and simple link-based replies should suffice.

A discussion inside the community should define the scope and related labels for the actual GitHub issues. Those include labels like `task`, `bug`, etc.

The same discussion should outcome with the levels and their actual values. For example, in the above example of a dead link, the original reporter just informed of a dead link and that the minimal/initial entry of 1 (marked as B1). The discussion should define that precisely, but maybe if they brought also a solution, the correct link - that spares some time the Discord administrator spent on the issue - then it can be labeled as B2.

Again, the discussion should outcome with the values, but a logical approach is that B2 is worth exactly twice the B1, while B3 can worth triple the B1 or twice the B2.

The GitHub Discussions is quite a suitable space for publishing the rewards cycles' lists.

The script ASA Stats uses for the rewards allocation is Python-based. It should be adjusted for Voi and open-sourced afterward.

# Define Success
Every Voi transaction coming from the official accounts is processed this way - simple as that!

# Concerns
Someone may be concerned that the implementation may overlap with the existing tipping routines (AlgoLeagues), but it rather extends it than replace it.

In a way, this brings more work to the network. That is true, but the work will be spread among many more people and with much less space for error.

# Prerequisite
A dedicated GitHub repository under the Voi Network organization.

An adjustment of the related Python script used for rewards allocation.

# Project Longevity
It is expected that the process will last as long as the Voi Network - forever!

It is expected that the first three members mentioned in the Team sections will administrate the process during the Voi Testnet phase.

# Project Length
3-4 weeks.

# Additional Information
Here's the latest ASA Stats rewards cycle thread in our GitHub for everybody to see in practice how we deal with it: https://github.com/asastats/channel/discussions/847 .