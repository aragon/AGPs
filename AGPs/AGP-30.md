---
AGP: 30
Title: Futarchy Signaling Markets for AGP Votes
Author: John Kelleher (@jpkcambridge)
Status: Rejected
Track: Finance
Created: 2019-04-06
---

# AGP-30: Futarchy Signaling Markets for AGP Votes

## Address of the transfer recipient

0xB320759d1A0ADbE55360a0a28a221013aA2DA4fC

## Amount of the transfer

30,000 DAI

## Number and frequency of transfers if recurring (enter “1” if only one payment will be made)

1

## Purpose of the transfer

"Aragon is a fight for freedom.  Aragon empowers freedom by creating liberating tools that leverage decentralized technologies." - [AGP-0, The Aragon Manifesto](https://github.com/aragon/AGPs/blob/master/AGPs/AGP-0.md)

[Futarchy](http://mason.gmu.edu/~rhanson/futarchy.html), described as "Vote your Values, Bet Your Beliefs," offers a [collusion resistant](https://www.vitalik.ca/general/2019/04/03/collusion.html) way for organizations to make decisions. By using prediction markets, participants are incentivized to evaluate a decision based on a given metric.  For organizations aligned around given values, futarchy offers the promise of enabling well informed decisions without delegating power to the few.  Futarchy offers the potential to be a liberating tool, and advancements in decentralized technology are allowing it to come to fruition.  We seek to demonstrate and improve upon an implementation of futarchy, better understand futarchy in practice, and to educate the Aragon network and the public at large on the promise of futarchy.

Our team has been developing an [Aragon app for futarchy decision markets](https://github.com/levelkdev/futarchy-app), as part of [this Nest proposal](https://github.com/aragon/nest/issues/93). As the first use case for the futarchy app, we're planning to build "Signaling Markets" for AGP votes using ANT price as the metric.

The AGP Signaling Market will allow users to make bets on the price of ANT at a future date, given the outcome of each AGP decision.

Example: "Team X" requests Flock funding. Two markets will be created - 1) "If Team X receives funding, what will ANT price be 6 months from today?" and 2) "If Team X does not receive funding, what will ANT price be 6 months from today?". Users can take "Long" or "Short" positions in either of these markets. The desired outcome is to predict which decision ("Yes" fund Team X, or "No" do not fund Team X) is best for ANT price.

[The futarchy app](https://github.com/levelkdev/futarchy-app) provides the smart contract infrastructure for setting up these markets, as well as the UI for users to buy and sell positions.

It's important to note that these markets are set up for "signaling" the impact of each decision on ANT price, and will not have an effect on the actual AGP decisions. ANT holders can look to the signaling markets as an input for their voting decisions. Smart contract based voting delegation to market decisions could also be built, although this is not in scope for this proposal.

We are requesting $30,000 funding for:

* Designing and implementing signaling market specific UX/UI, to launch an instance of [the futarchy app](https://github.com/levelkdev/futarchy-app) for AGP's.
* Modify futarchy smart contracts to be signaling markets instead of decision making
* Add Tutorial video(s) and informational material on how to interact with the signaling markets
* Build a script or CLI that allows us to create new markets for each new AGP
* Build an oracle that resolves based on AGP proposal decision vote outcome
* Build an oracle that resolves based on ANT price, leveraging output from the [Oracle Manager](https://github.com/aragon/nest/issues/138)
* Provide some initial liquidity for the markets and cover deployment costs


## Recipient information

Organization:

Name: Level K

Website: https://www.levelk.io/

Fill out the following information for each individual team member who will be managing funds from this transfer:

Name: John Kelleher

PGP key fingerprint: 938228474341ad442ade3986104e7f35bfe55e56

Website:  https://twitter.com/jpkcambridge

Other URL:  https://github.com/jpkcambridge

Name: Emily Williams

PGP key fingerprint: d17cf2aa6dd6954b43047cbf6675f31ab9c5c461

Website: https://twitter.com/crypt0glitter

Other URL: https://github.com/emaG3m

Name: Mike Calvanese

PGP key fingerprint: 38f51ad8fb15ab2f59a873311ee3a764efa68f67

Website: https://twitter.com/MikeCalvanese

Other URL: https://github.com/mikec

## License
Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).
