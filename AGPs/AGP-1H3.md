---
AGP: tbd
Title: Apiary Activity Feed
Author: @lkngtn (@1hive)
Status: Stage IV
Track: Finance
Created: 2019-11-12
---

# **AGP-TBD: Apiary Activity Feeds**

## **Address of the transfer recipient**

 `0x9213737fbb72d8f924fca55d508ae2c004413d64` Vault of the [apiary project organization](https://mainnet.aragon.org/#/apiary)

## **Amount of the transfer**

50,000 DAI Due upon approval
15,000 ANT Due upon successful delivery

## **Number and frequency of transfers if recurring**

2 (One upon approval, one upon successful delivery).
For the purpose of budgeting, the full amount should be debited against this quarter's budget.

## **Purpose of the transfer**

Due to the work on App Mining, Apiary will be indexing all transactions including "internal interactions". This gives us the ability to analyze **Activities** and we think it would be incredibly useful to be able to surface that information as a contextual activity feed. This feed would make it easier to engage and interact with organizations, making them feel much more like a social network than a company.

The activity feed would be displayed in three contexts within Apiary.
* On an Organization Detail page, showing all activities related to that organization
* On a User's profile page, showing all activities involving them across all organizations they participate in.
* In a User's activity feed, showing all activities across the organization's they have subscribed.   

Activities will be categorized into Primary and Secondary events. Primary actions will be things like `Alice created a Vote`, whereas secondary actions will be things like `Bob voted in favor of option A`. Primary actions will exist as parent elements, and secondary actions will be nested as child elements.

Additionally, we will integrate [3box Threads API](https://docs.3box.io/build/web-apps/messaging/about) to provide contextual discussions related to each Primary activity.

In exchange for funding we will deliver the following:
* Add the ability for users to authenticate to Apiary using web3 provider
* Add the ability for users to manage activity feed subscriptions preferences
* Create an Activity Feed component which shows Primary and Secondary activities within the Context of a User, an Organization, or an array of Organizations
* Add an Activity Feed View
* Add an Organization Detail View (if possible this would integrate autark's work on Organization Settings)
* Add a User Profile View (if possible this would integrate Autark's existing work on User Profiles)
* Integrate 3box threads into activity feed enabling contextual discussions in relation to activities.


## **Recipient information**

`0x9213737fbb72d8f924fca55d508ae2c004413d64` Vault of the [apiary project organization](https://mainnet.aragon.org/#/apiary)

## **License**

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).
