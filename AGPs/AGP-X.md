---
AGP: N/A
Title: Official ANJ and Governor DAO addresses
Author: Facu Spagnuolo (@facuspagnuolo)
Status: Stage II
Track: Proclamations
Created: 2019-11-13
---

# AGP-X: Official ANJ and Governor DAO addresses

## Proclamation text

Aragon Network declares the contract deployed at `TBD` as the official Aragon Network Juror (ANJ) token to be the official ERC20 token that must be used by the jurors of the canonical Aragon Court to participate in the dispute resolution process.

Along with the official ANJ token address, Aragon Network declares the Aragon DAO deployed at `TBD` as the official DAO in charge of governing Aragon Court that will be deployed in the upcoming weeks as described in its [launch process](https://forum.aragon.org/t/aragon-network-launch-phases-and-target-dates/1263). This DAO will be in full control of Aragon Court until the Aragon Network DAO is deployed as explained in the launch process. The responsibilities of the governor DAO are:

- Controlling the ANJ token until Aragon Court is deployed
- Proposing and verifying governance proposals and voting in favor or against them

The Aragon Network governor DAO was deployed using the [company template](https://github.com/aragon/dao-templates/tree/templates-company-v1.0.0/templates/company) with the following settings:

- Voting settings:
    - Support: 50%
    - Minimum approval: 50%
    - Duration: 1 week
- Token settings:
    - Token: Aragon Network Governor (ANG)
    - Members: `TBD`
        - `0xF0a5486944d315e05dD24A3c106B95d12A105650` (Jorge Izquierdo - @izqui)
        - `0xd5931f0a36FE76845a5330f6D0cd7a378401e34d` (Facu Spagnuolo - @facuspagnuolo)
        - `0x...`
        - `0x...`
        - `0x...`
- Agent app installed to be able to trigger calls to Aragon Court

## Motivation for writing this proclamation

Aragon Court will be deployed before the end of the year kicking off Aragon Network's launch. Therefore, there is a need for a trusted entity that will govern Aragon Court before it is transitioned to the Aragon Network DAO which is scheduled to be deployed during the first half of 2020. 

Additionally, Aragon Court requires a native token to be able to participate in its dispute resolution protocol. This token address must be agreed beforehand and set at deploy time for security and trust reasons.

## License

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).

