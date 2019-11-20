---
AGP: N/A
Title: Official ANJ and Aragon Network DAO addresses
Author: Facu Spagnuolo (@facuspagnuolo)
Status: Stage IV
Track: Proclamations
Created: 2019-11-13
---

# AGP-X: Official ANJ and Aragon Network DAO addresses

## Proclamation text

The Aragon Network declares the contract deployed at `TBD` to be the official Aragon Network Juror (ANJ) token that must be used by jurors of the canonical Aragon Court to participate in the dispute resolution process.

Along with the official ANJ token address, the Aragon Network declares the Aragon DAO deployed at `TBD` to be the official Aragon Network DAO in charge of governing Aragon Court, which will be deployed in the upcoming weeks as described in its [launch process](https://forum.aragon.org/t/aragon-network-launch-phases-and-target-dates/1263). This DAO will be in full control of Aragon Court as explained in the launch process. The responsibilities of the governor DAO are:

- Controlling the ANJ token until Aragon Court is deployed
- Proposing and verifying Aragon Network governance proposals and voting in favor or against them

The Aragon Network DAO will be managed initially by a council during phases 1 and 2 of the launch process. The initial council will by dissolved  and transfer full control of the Aragon Network DAO to ANT holders as described in the launch process.

The Aragon Network DAO was deployed using the [membership template](https://github.com/aragon/dao-templates/tree/templates-company-v1.0.0/templates/membership) with the following settings:

- Voting settings:
    - Support: 50%
    - Minimum approval: 50%
    - Duration: 1 week
- Token settings:
    - Token: Aragon Network DAO (AND)
    - Members: `TBD`
        - `0xF0a5486944d315e05dD24A3c106B95d12A105650` (Jorge Izquierdo - @izqui)
        - `0xd5931f0a36FE76845a5330f6D0cd7a378401e34d` (Facu Spagnuolo - @facuspagnuolo)
        - `0x...`
        - `0x...`
        - `0x...`
- Agent app at `TBD` installed to be able to trigger calls to Aragon Court

## Motivation for writing this proclamation

Aragon Court will be deployed before the end of the year, kicking off the Aragon Network's launch. Therefore, there is a need for a trusted group of members that will govern the Aragon Network DAO for Aragon Court before it is fully transitioned to ANT holders, which is scheduled to happen during the first half of 2020.

Additionally, Aragon Court requires a native token to be able to participate in its dispute resolution protocol. This token address must be agreed beforehand and set at deploy time for security and trust reasons.

## License

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).

