---
AGP: 72
Title: Frame Finance Proposal
Author: Jordan Muir (@floating)
Status: Stage IV
Track: Finance
Created: 2019-07-10
---

# Frame Finance Proposal

[Frame](https://frame.sh) is an open source accounts platform for the web. It lives at the OS-level and isn’t dependent on a browser or extension store. It also works with any type of dapp be it web, desktop or command line. It was built to deliver truly decentralized and unstoppable account and application infrastructure. One of our main goals since starting Frame has been to support the Aragon ecosystem with this platform and to handle the account and provider needs of the Aragon stack.

As a team, we've had great success in the [Aragon Nest](https://github.com/aragon/nest) program delivering on our milestones and releasing mainnet ready account and key management tools along with easy-to-use provider interfaces. We released our mainnet-ready version of Frame earlier this year at Aracon 2019. We're committed to the Aragon ecosystem and we're confident our work can support DAO usability and adoption.

Frame is requesting 232,000 DAI in financing to support work on deep Aragon account integrations and functionality, decentralized application infrastructure, user onboarding and core provider functionality for the Aragon application stack and ecosystem.

**The scope of our work includes:**
- Enabling DAOs to interact with external dapps and protocols via Aragon smart accounts and agent functionality
- Implementing unstoppable decentralized infrastructure for the Aragon stack and ecosystem
- Building solutions for Aragon on-boarding and application launching
- Handling account/key management for the Aragon application stack and ecosystem

Frame will complete, support and iterate on this scope of work in collaboration with Aragon Flock teams and the Aragon community. We hope to be able to continue this work in the future as a Flock team after the next Aragon network vote in October.

## Deliverables
### Aragon Smart Accounts

> **:: The ability to add an Aragon DAO as an account in Frame and interact with external dapps and protocols just like any other account**

Currently DAOs have limited ability to interact with protocols outside of AragonOS. The landscape and availability of dapps and protocols will always move faster than the ability to replicate that functionality inside of AragonOS. Aragon smart accounts are an integration of Aragon DAOs in Frame that allows you to use DAOs like any other account to interact with external protocols, login to dapps and sign transactions. Smart accounts will change the way we use the web and we want Aragon smart accounts to lead the way.

We're very excited to provide this functionality for the Aragon ecosystem and we will continue working to expand the reach, flexibility and usability of Aragon DAOs. Aragon smart accounts open the door to endless possibilities using your DAO with the decentralized web.

View a demo of [Aragon Smart Accounts](https://www.youtube.com/watch?v=24KaOcK38DQ)

### Decentralized Infrastructure

> **:: The ability to easily run local Ethereum light clients and IPFS gateways via a simple interface**
>
> **:: The ability to resolve APM/ENS/IPFS content via this infrastructure and our companion browser extensions in support of true decentralization**
>
> **:: To eliminate the need to maintain a separate Aragon Desktop codebase as this infrastructure will provide the foundation for true decentralization**

We believe Aragon should be truly decentralized and unstoppable. Any user, regardless of technical understanding, should be able to pilot Aragon without relying on centralized services. Frame is the platform to make this a reality. In addition to smart accounts, we're expanding Frame's underlying infrastructure to allow users to run decentralized services locally. Instead of relying on centralized gateways, users can now create their own connections through a simple interface in Frame.

In Frame v0.2, users will be able to run Ethereum light clients and IPFS gateways with the flip of a switch. On top of this we’re making it easy for users to resolve APM/ENS/IPFS content via this infrastructure and our companion browser extensions. This effort will replace the need for Aragon Desktop as we make more of these clients available and easy to use. We will continue to improve this infrastructure and provide unstoppable access to Ethereum, ENS, IPFS and APM within the Aragon stack. We’re really excited about this and think it's an important infrastructure improvement for Aragon.

### User Onboarding and App Launching

> **:: The ability to easily create Aragon smart accounts without having an existing DAO and the ability to launch the Aragon client from these accounts via previously outlined decentralized infrastructure**

We will be working on an integration that gives users the ability to easily create Aragon smart accounts without an existing DAO. We will also be adding the ability to launch the Aragon client from these accounts via the decentralized infrastructure outlined above. This will ensure users always have truly decentralized and unstoppable access to Aragon and their accounts.

We're committed to the mission of making Aragon DAOs more powerful and usable via provider level integrations. We want to make creating and participating in DAOs easier than using the best web services that exist today. We hope to play a large role in the effort to make DAOs accessible everywhere and to everyone.

### Core Provider Functionality

**Hot Signers:** In v0.2 you will have access to non-hardware signers that are stored locally on your machine and can be backed by a mnemonic seed, private key or keystore.json file.

**First-class Hardware Support:** We will continue to work on our first-class hardware integrations, including the addition of BLE signers like the Nano X.

**Persistent Accounts:** In v0.2 accounts are now persistent. This means you can use your accounts even when your signer is asleep or disconnected. You’ll only need your signer to be available when signing a payload. This is also a usability building block that enables smart account UX.

**Activity Monitor:** The initial version of our activity monitor was released in v0.1.2, but that's just the beginning. We plan to push this feature much further to provide users with more insightful and reliable account activity data.

**Gas Controls:** We will add the ability for users to adjust gas before signing a transaction. This control and flexibility is necessary due to fluctuations in the gas market.

**Payload Recognition:** We will add support for `eth_signTypedData` and integrate radspec. We plan to contribute to standalone tooling mentioned in [#58](https://github.com/aragon/nest/issues/58) similar to how we spun off [`eth-provider`](https://github.com/floating/eth-provider) which is now gaining traction from users outside of the Aragon and Frame communities.

**Token Support:** We will add deep understanding and display helpful data when interacting with various token standards.

**ENS/IPFS Resolver:** We will give users the ability to easily resolve ENS/IPFS via Frame + companion extensions and app launching.

## Team

### Jordan Muir - Project Lead

Jordan is the creator of [Frame](https://github.com/floating/frame) and many other projects, most recently [Restore](https://github.com/floating/restore), a predictable and observable state container for React apps. Jordan has extensive full stack experience, including design, with a focus on real-time apps and architectures. He loves discovering new technologies and trying to create impactful experiences that unlock value for users and humanity. He's driven by projects that contribute to the acceleration of human innovation and believes open decentralized networks are an important step. He hopes to contribute to the ecosystem in meaningful ways that increase the use and adoption of these networks. ([GitHub](https://github.com/floating), [Twitter](https://twitter.com/ffloat))

### Philip Prophet - Senior Engineer

Philip is a developer and architect who loves working in small teams to solve big problems. Before joining Frame he worked with Swedish electromobility startup Bzzt to help combat climate change and improve city air quality around the globe. He has been involved in the Swedish crypto/blockchain scene for many years, organizing events, teaching dApp development and working on open source projects. Nothing inspires him more than helping to bring decentralization to tech, finance and politics so when asked to join the Frame team and the wider Aragon family he had absolutely no doubts. ([GitHub](https://github.com/monkybrain), [Twitter](https://twitter.com/monkybrain_))

### Simon Emanuel Schmid - Senior Engineer

Simon has worked for more than 10 years as a Software Engineer where he gained a profound and extensive knowledge on how to develop user interfaces that are fascinating and comprehensible to use. His enthusiasm for programming got him into building several digital products and he co-founded a startup where he gained entrepreneurial experiences on how to design and develop amazing digital products from scratch. He then joined Melonport to build a fully decentralised front-end for digital asset management. During that time he realized that the current main need of the blockchain ecosystem are solid tools that make the technology more accessible for users and developers alike through a great user experience. And that is what Frame is about. ([GitHub](https://github.com/schmidsi), [Twitter](https://twitter.com/schmid_si), [LinkedIn](https://www.linkedin.com/in/schmidsi))

### Matt Holtzman - Operations/Communications/Engineering

Matt brings over 12 years of experience working on technology in capital markets. He previously worked as lead engineer for a startup providing social sentiment metrics for equity trading as well as buy and sell side engagements across the globe, working up and down the tech stack. When he gets some free time he spends it biking or staring opponents down at the poker table. He’s excited to be a part of the Aragon ecosystem and to help build the decentralized organizations of the future. ([GitHub](https://github.com/mholtzman), [LinkedIn](https://www.linkedin.com/in/mattholtzman))

## Finances

We are requesting a total of 232,000 DAI, which covers 6 full-time contributors for 4 months, in addition to ongoing security audits and operational costs. We have subtracted the remaining funding of our Nest grant (62k DAI) from this total.

Total: 232,000 DAI
Payroll: 202,000 DAI
Security Audits/Contractors/Legal: 30,000 DAI

30,000 ANT upon completion of all deliverables

#### Address of Transfer Recipient

0x4df2FA69Ef22D59225521E8C03DF7EfA2b747a1D

#### Frequency of Transfers

1

### Recipient Information

#### Organization
Name: **Frame**
Website: **https://frame.sh**
Other URL: **https://github.com/floating/frame**

#### Members managing funds

Name: **Jordan Muir**
Website: **https://github.com/floating**

## More Resources
**AraCon Presentation:** https://www.youtube.com/watch?v=wlZWLiy2GD0
**Mainnet Release:** https://medium.com/@framehq/frame-mainnet-alpha-update-f0e4a9b89e1e
**Initial Audit:** https://medium.com/@framehq/frame-security-audit-frm-01-7a90975992af
**Nest Grant 1:**  https://github.com/aragon/nest/pull/25
**Nest Grant 2:** https://github.com/aragon/nest/pull/146

The terms of this AGP may be updated by another AGP or Flock membership if we are accepted in the next Aragon network vote in October.
