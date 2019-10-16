---
AGP: N/A
Title: Comprehensive Aragon Bug Bounty Program
Author: burrrata (@burrrata)
Status: Stage IV
Track: Association
Created: 2019-10-02
---

# AGP-X: Comprehensive Aragon Bug Bounty Program

## Description of desired Association policy change

This proposal is to expand the [Aragon Association Bug Bounty Program](https://wiki.aragon.org/association/security/bug_bounty/) to make all Aragon projects funded by the AA via AGPs, the Nest program, or the Flock program eligible. This definition of "funded by the AA" is left broad enough to cover a range of projects from the Aragon Court to Aragon app developed through the Nest program. This does not automatically include all such project, but makes them eligible for the bug bounty program. Projects will only be accepted into the bug bounty program if they have undergone a security audit, incorporated all major and critical security audit recommendations, and shipped to mainnet. If projects make major changes after incorporating security audits and shipping to mainnet, a new security audit will be required for the projects continued eligibility in the bug bounty program. This ensures that only projects that have been audited and incorporated critical and major security audit recommendations are included. Failure to undergo a security audit or to incorporate a security team's critical and major recommendations will result in projects being dropped from the Aragon Association Bug Bounty Program.

In addition to expanding the scope of the [Aragon Association Bug Bounty Program](https://wiki.aragon.org/association/security/bug_bounty/), the amounts will also be changed.

Currently the Aragon Association Bug Bounty program is as follows:
- Critical (CVSS 9.0 - 10.0): $5,000 - $50,000
- Major (CVSS 7.0 - 8.9): $2,500 - $5,000
- Medium (CVSS 4.0 - 6.0): $1,000 - $2,500
- Low (CVSS 1.0 - 3.9): $500 - $1,000

The Aragon Association Bug Bounty program would change to the following:
- Critical (CVSS 9.0 - 10.0): $50,000 - $150,000
- Major (CVSS 7.0 - 8.9): $25,000 - $50,000
- Medium (CVSS 4.0 - 6.0): $10,000 - $25,000
- Low (CVSS 1.0 - 3.9): $5000 - $10,000

## Motivation for changing this Association policy
Aragon is now shipping more apps through Autark, Aragon Black, and the Nest program. These apps are amazing and could unlock tons of value, but only if people use them…

People are wary of DAOs because of “the DAO” hack. For people to trust (and thus use) Aragon we need to go above and beyond to prove that the Aragon platform, and all major releases of Aragon apps, are secure. This is easier said than done.
- Security audits are not perfect. Even with an audit all you know is what was reported. They might have missed something.
- Security audits are highly technical and the process is opaque to people who are not involved in the Ethereum security community.
- Security audits are expensive. Having strategic and financial help to navigate that negotiation is extremely important!

Aragon is trying to attract talent and users. Having the world's easiest to build on and most secure platform is a huge selling point. If developers see that they will have help shipping professional and production ready applications they are more likely to choose to build on Aragon vs other platforms. If users trust that all major Aragon apps are secure, they’re more likely to use them. To do this we need a multi layered approach to security. This can include audits for all major projects (Nest and Flock), but should also include a comprehensive Bug Bounty program that covers all major apps.

We are spending millions of dollars on Flock teams and hundreds of thousands of dollars on Nest projects. Bug bounties help to secure that investment, but unlike insurance bug bounties are only paid out if there is a problem. Aragon DAOs currently hold hundreds of thousands of dollars in their vaults, and soon more organizations will be using Aragon DAOs to manage millions. Paying out $10,000 for a critical vulnerability is simply an insufficient incentive for anyone who discovers a vulnerability. Increasing bug bounty payouts is a small price to pay for consumer confidence and being able to fix bugs before they are a major issue.

> This proposal is inspired by @stellarmagnet's post on [Upgrading the Bug Bounty program](https://forum.aragon.org/t/upgrading-the-bug-bounty-program-potential-agp/562). Ideas are easy, but shipping a polished, secure, and usable app to production is hard. Thank you for bringing this up and starting the conversation! :)

## License
Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).

