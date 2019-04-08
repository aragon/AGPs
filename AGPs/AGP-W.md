---
AGP: N/A
Title: Decentralizing aragonpm.eth
Author: Jorge Izquierdo (@izqui)
Status: Stage III
Track: Association
Created: 2019-04-03
---

## Motivation for changing this Association policy

When Aragon One planned the Aragon 0.6 release, it was internally thought of as a soft-launch. Even though it was the mainnet deployment, the main aragonPM registry (`aragonpm.eth`) in both the rinkeby and mainnet environments was controlled by a cold key that Aragon One held. This has given us the ability to perform releases at any time, and act quick in case an issue were to be found.

It's been more than 5 months after releasing Aragon 0.6. During this time we have published 4 minor releases, all of which were properly scheduled and no emergency releases have been done. We consider that it is now safe and appropriate to transition control of the aragonPM registries from the Aragon One cold key to a more decentralized and future-proof publishing process that won't solely depend on Aragon One.

## Description of desired Association policy change

The following changes are proposed to the `aragonpm.eth` aragonPM DAOs:

- Mainnet and rinkeby environments:
    - Change the root authority of the aragonPM DAOs from the 'Aragon One cold wallet' to the Aragon Association multisig. A Voting app within the DAO will control creating new repos and publishing new versions to all the repos (see Appendix for the proposed DAO structure)
    - Create a new aragonPM registry at `a1.aragonpm.eth` controlled by Aragon One, granting 'Aragon One cold wallet' the `CREATE_REPO_ROLE` permission in the registry and setting this address as the root authority of the DAO. This registry can be used by Aragon One to publish apps before releasing them in `aragonpm.eth`.
- Staging: Aragon One will keep control of the current staging environment, renaming it to `a1-staging` (in both https://aragonpm.com and deployments documentation). The rationale being that other teams can very easily create their own staging environments if they need one (the deployment process is documented in [aragon/deployments](https://github.com/aragon/deployments)) or use the `open.aragonpm.eth` registry that allows anyone to create their own repos.

## Appendix: `aragonpm.eth` DAO structure

### Current state

- [Mainnet permissions](https://github.com/aragon/deployments/blob/master/environments/mainnet/permissions.yml)
- [Rinkeby permissions](https://github.com/aragon/deployments/blob/master/environments/rinkeby/permissions.yml)

### Proposed DAO structure

#### New apps

**Token Manager**:

- Token: APM
- Transferable: No
- Maximum tokens per account: No limit

**Voting**:

- Token: APM
- Support required: 66.666666666666666666% 
- Minimum acceptance quorum: 50%
- Vote duration: 72 hours

#### Permissions

|         App        |        Role        |      Grantee      |     Manager     |
|:------------------:|:------------------:|:-----------------:|:---------------:|
|       Kernel       |     MANAGE_APPS    |  AA multisig (*)  | AA multisig (*) |
|         ACL        | CREATE_PERMISSIONS |    APMRegistry    | AA multisig (*) |
|         ACL        | CREATE_PERMISSIONS |  AA multisig (*)  |   AA multisig   |
|     APMRegistry    |    CREATE_REPOS    |     Voting (*)    | AA multisig (*) |
| All Repo instances |   CREATE_VERSION   |     Voting (*)    | AA multisig (*) |
|       Voting       |    CREATE_VOTES    | Token Manager (*) | AA multisig (*) |
|       Voting       |   MODIFY_SUPPORT   |  AA multisig (*)  | AA multisig (*) |
|       Voting       |    MODIFY_QUORUM   |  AA multisig (*)  | AA multisig (*) |
|    Token Manager   |        MINT        |  AA multisig (*)  | AA multisig (*) |
|    Token Manager   |        BURN        |  AA multisig (*)  | AA multisig (*) |

- Mainnet AA multisig: 0xcafE1A77e84698c83CA8931F54A755176eF75f2C
- Rinkeby AA multisig: TBD by Aragon Association

(*) denotes that this is a permission that will need to be modified or be created

#### Initial token distribution

APM token holders:

- Aragon One: 10 APM
- Aragon Network Security Partner (at the time of deployment): 5 APM

The AA multisig has the ability to change the distribution of token holders by minting and burning tokens. These changes should generally be triggered by an AGP (e.g. a new Flock team that requests APM tokens as part of their proposal) but as per AGP-1, the Aragon Association would still be able to perform these changes unilaterally (e.g. a Flock team is no longer working for the Network).


#### Timeline

These changes should occur no earlier than 1 month after the Aragon 0.7 release and before the ANV3 (scheduled for July 2019).

## License
Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).
