---
AGP: N/A
Title: Common court with Kleros
Author: Clément Lesaege
(@clesaege)
Status: Stage III
Track: Proclamation
Created: 2019-09-20
---

# AGP-XX: Common court with Kleros

## Proclamation text

Aragon will work with Kleros for its court system.

A part of the Kleros native token (PNK) would be minted to be put in an ANT bonded curve (this could use some of the work of Aragon Black on batched bonded curves). To avoid gas wars, there will be some initialization period for this bonded curve where everyone can deposit ANT.

In exchange, Aragon would provide a mix of ETH/DAI/ANT. This can be provided to Kleros cooperative or to the Kleros DAO (using Aragon fund management module). The ETH/DAI would guarantee funding of Kleros improvements and of the ecosystem. The ANT would be there to align incentives between both projects.

The exact amount of tokens to be put in the bonded curve or to be exchanged need to be determined by an agreement of both Aragon and Kleros.

The Aragon Association and the Kleros Cooperative will negotiate an agreement. This agreement and the discussion process will be fully transparent and will be proposed to vote on both Aragon and Kleros governance. This can take the form of multiple deals, each providing funding and additional PNK to the bonded curve. Each will be the subject of a governance proposal in both Kleros and Aragon using the Aragon dapp.


## Motivation for writing this proclamation

### Background

#### Kleros presentation

Kleros is a decentralized autonomous organization (DAO) providing arbitration services. It is useful for Curated Registries, Oracles, and Escrow use cases. It has been live on the mainnet since August 2018 and had its last release in March 2019 allowing specialized courts. It has handled 80 disputes and currently has 3 applications connected to it:

<div style="text-align:center"><img width="115" alt="t2crlogo" src="https://user-images.githubusercontent.com/8873352/63350320-1eed1080-c355-11e9-8b53-e6b20c98814c.png"></div>


The [Token² Curated registry](https://tokens.kleros.io), which is a registry of tokens where Kleros jurors solve disputes about token specifics (Project Name, Logo, Ticker and network address). It is made to prevent scam tokens (tokens impersonating projects and giving wrong addresses) and to provide a way for dapps to access a list of tokens and for people to certify information about token characteristics. It has been used by [Ethfinex](http://ethfinex.com/) (rebranding as DeversiFi) in their listing process and has processed more than 2000 ETH of deposits.


<img width="96" alt="escrow" src="https://user-images.githubusercontent.com/8873352/63358327-c4f34780-c362-11e9-9c11-b3cfa1cea68a.png">


The [Escrow system](https://escrow.kleros.io), allows people to make escrow payments for goods or services. Should the good or service not be provided, the payer can ask for reimbursement as the funds are held in escrow. If the payee does not agree, a dispute can be made that Kleros jurors can arbitrate.


<img width="100" alt="realitio" src="https://user-images.githubusercontent.com/8873352/63358412-e5bb9d00-c362-11e9-8547-9ede57b7d3d4.png"> 


[Realitio](https://realit.io/), is a blockchain Oracle developed by Reality Keys through an [Ethereum Community Fund](https://ecf.network/) grant.

“For smart contracts to produce the correct output, they need a reliable way to verify input. This is the basis of the oracle problem.

The goal of the Realitio project is to provide developers with a flexible tool that can be plugged in today. And that works with any approach, from trusted arbitrators and distributed juries to fully trustless coordination games.”
Kleros can be selected as an arbitrator by Realitio users.

<img width="129" alt="DOT" src="https://user-images.githubusercontent.com/8873352/63358508-0dab0080-c363-11e9-8155-49e1ed7ee0b6.png">

Kleros was also used during the [Doges On Trial](https://dogesontrial.dog) experiment. However this project is not active anymore because most of the Doge images on the internet are already there :p. You can learn more about it at [this ETHCC presentation](https://www.youtube.com/watch?v=DVCzEuEwQGg).

#### Aragon Court State

The [initial Aragon paper](https://github.com/aragon/whitepaper/tree/v1#appendix-a-decentralized-arbitration-system-for-the-aragon-network) mentioned building a decentralized arbitration system as part of network services. This initial paper proposed a model different from Kleros.

Recently Aragon members proposed to create a court based on Kleros with minor modifications (see this [*post*](https://forum.aragon.org/t/aragon-court-v1/691) and [*github*](https://github.com/aragon/whitepaper)). The proposal is similar to Kleros in both its high level functioning and technical nature. It is currently in [Research and Development stage](https://github.com/aragon/aragon-court).


### Arguments

#### Proposal is similar

It's evident that both Kleros and Aragon teams share the same court system vision. At this early stage of the ecosystem it seems more reasonable to pool both teams resources together rather than building/improving two similar systems in parallel.

#### Proposed changes can be implemented in further version or as subcourt specific features

The only significant change would be to charge a subscription fee to organizations using the court even without disputes. The Kleros team believes that this change is likely to hinder adoption. But if governance were to decide so, it could be done without code modification simply by court policies asking jurors to vote “Refuse to arbitrate” on disputes of organizations who have not paid their subscription fees.

#### Kleros community is open to change and experimentations

Creating a new system when the community of a previous system is reluctant to change (as happened with Bitcoin and Ethereum) makes sense as it is the only way to innovate. But Kleros community is not reluctant to change. It is open to cryptoeconomic experiments which can be used to test proposed changes before implementing them at a larger scale. Note that most changes will be consensual and may not require extensive testing (most tweaks proposed by aragon members fit into this category).

#### No benefits from competition to the ecosystem

If the Aragon court were to use different mechanisms, it could benefit the ecosystem if those mechanisms were to perform better than Kleros ones and it would justify a new court creation. Competition is good when different products compete with each other as it gives people more choices and leads to better products more likely to “win” the market. But here, competition of similar products would just distract resources from both teams “fighting” each other for market share on grounds which are not product related.

#### Creating competition with users is dangerous

 Kleros uses Aragon for governance.

Centralized platforms often use an attract-extract strategy.

-   Attract: At the beginning platforms try to offer the best experience to their users, they are often subsidized with VC money. They welcome third parties (intermediate users) integrating and building on their platform.
-   Extract: After reaching a critical mass of users. They now try to extract value from them. This includes competing with their users.

<img width="396" alt="attract-extract" src="https://user-images.githubusercontent.com/8873352/63358602-3d5a0880-c363-11e9-8f13-fdf82840efd3.png">

Decentralization is [*supposed to solve this problem*](https://medium.com/s/story/why-decentralization-matters-5e3f79f7638e). But it won’t if even decentralized platforms try to compete with their users.

For Aragon, network effects among DAOs are not currently strong enough to control the ecosystem, so users are not bound to stay on Aragon. If Aragon were to compete with them, they could migrate their governance to other DAO platforms (DAOstack, MolochDAO forks or even develop their own) in order to avoid reinforcing a competitor. This would also scare would be users, as even if Aragon does not act as a competitor now, it could be in the future if it has a history of doing such things.

#### Good relations and compatibilities

Even if an Aragon team planned to fork Kleros, relations are still good as those plans gave appropriate credit to the Kleros team. Kleros and Aragon teams met at multiple events. Kleros and Aragon communities tends to have similar views and visions (Kleros is composed of legal tech enthusiast and of DAO enthusiasts).

Both teams ask token holders to vote on project direction/updates and aim toward full decentralization of both the network and developing teams.

Both teams have a history of collaborating with others in order to have greater achievements (Kleros was created by members of Crowdjury and of the Decentralized Arbitration Court hackathon project, Aragon onboards new teams).

Both teams are committed to build decentralized, trustless systems to be used as liberating tools (Kleros does not have a formal manifesto, but we did not find any potential point of disagreement reading [*the Aragon manifesto*](https://blog.aragon.org/the-aragon-manifesto-4a21212eac03/)).

Overall, Kleros and Aragon teams/communities are pretty much aligned.

#### Connected dapps potential

There are a multitude of Arbitrable dapps required by the ecosystem (identity DAO, translation dapp, ENS domain curation, see [*a more extensive list there*](https://github.com/kleros/hackathon/blob/master/Arbitrable%20Dapp%20Ideas.pdf)). Most of them also require a governance mechanism. There are a lot of projects which could benefit from both Kleros and Aragon. Those could be created/bootstrapped by both teams.

#### Common work on governance

For now Kleros has mostly been focused on dispute resolution and bootstrapping the ecosystem. It initially planned to build its own governance system (no governance mechanisms were ready at that time) but switched to using Aragon. Kleros roadmap includes governance upgrades [*like liquid voting*](https://forum.kleros.io/t/liquid-voting-complexity/71), which are [*also of interest*](https://forum.aragon.org/t/open-challenges-for-on-chain-liquid-democracy/161) to Aragon. There is a high collaboration potential between Kleros and Aragon on decentralized governance.

## License
Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).
