---
AGP: TBD
Title: Aragon App Mining
Author: lkngtn (@lkngtn)
Status: Draft
Track: Finance
Created: 2019-10-02
---

# AGP-M: Aragon App Mining

## Address of the transfer recipient

0xe0d11d5a1982f64ff1d36cd8c2bd315dea127d66 (Agent of pinion.aragonid.eth)

## Amount of the transfer

100K ANT
50K DAI

## Number and frequency of transfers if recurring (enter “1” if only one payment will be made)

Quarterly transfers of 100K ANT with no expiration date and beginning after ANV 5 and due the week after each ANV.
One time transfer of 50K DAI for initial execution and launch of the App Mining program.

## Purpose of the transfer

To fund an "Aragon App Mining" program which rewards developers for creating and maintaining Aragon applications. The policy is inspired by [Blockstack's App Mining program](https://app.co/mining).

A core value proposition of Aragon is that it is a platform which allows users to pull from a library of modular and composable applications to create and operate an organization on-chain. In order to attract application developers to the platform we need to provide a stable opportunity that encourages entrepreneurial developers to understand user needs, develop applications, ship them to mainnet, and to continue to maintain and improve them over time.

At the moment there is no incentive to do this outside of one-off grants. There has been discussion to create monetization models for the eventual release of the App Center, but currently such a system doesn't yet exist, and even if it did the number of users of Aragon is small enough that such a market may not be attractive enough to bring top talent into the space. Users will come if there are high quality apps, but if there are no users, no high quality apps will be built and maintained.

To remedy this I propose we bootstrap the supply side by allocating funds and distributing them to Aragon Application developers based on agreed upon KPIs. We can combine multiple KPIs into an **Aragon App Score**, which we can use to rank applications and then use the ranking to distribute funding to maintainers on a periodic basic.

**The following weighted KPIs would be used to create the Aragon App Score:**

| KPI | Formula | Weight |
| -------- | -------- | -------- |
| Utility    | Sum of (# of transactions involving an application ) | 30%  |
| Value weighted utility    | Sum of (# of transactions involving an application * DAI value of organization's treasury) | 30%    |
| Popularity    | Sum of (# of installations) | 10%  |
| Value weighted Popularity    | Sum of (# of installations *  DAI value of organization's treasury) | 30% |

To compute the DAI value of an organizations treasury we would use the *default vault* and compute the DAI value of ETH, ANT, and DAI held by the organization.

To compute the # of transactions involving an application we would simply examine the blockchain.   

For each payout cycle, there is a determined “pot” of total earnings that will get paid to apps. The top app gets paid 20% of the total pot. So, for a pot of 100K ANT, the top app receives 20K ANT. The next app gets paid 20% of the remaining pot. The remaining pot is 80K, and 20% of that is 16K ANT. This process continues until every app has been paid or the payout amount is bellow 200 ANT whichever comes first.

**Blacklist**

It's possible that the KPI mechanism can be gamed, for example the popularity metric could be manipulated by creating a bunch of organization and installing a bunch of otherwise unpopular applications. For the purposes of our initial pilot, rather than try an engineer un-gameable metric, we propose that we can rely on the community to report potential abuse and the discretion of Pinion to manage a blacklist for the purpose of excluding recipients that are suspected to be trying to maliciously manipulate payout amounts. In the future, this role could be decentralized by leveraging the Aragon Court.

**Initial and Ongoing Execution**

This proposal includes a one-time 50K DAI budget for Pinion to execute on the development and documentation effort related to surfacing these metrics to the community and preparing the initial launch of the app mining program.

If approved, Pinion would:
    - Work with [Apiary](apiary.1hive.org) to create a dashboard that includes these metrics and make the Aragon App Score publicly and easily accessible to the Aragon community.
    - Provide documentation via PRs to hack.aragon.org for application developers to participate in the program
    - Assist the AA and/or teams responsible for Aragon communications in preparing communications for the launch of Aragon's App Mining program
    - Coordinate with the AA to execute payments each quarter to eligible recipients based on calculated Aragon App Scores
