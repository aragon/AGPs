---
AGP: N/A
Title: A simple Network Budget
Author: Louis Giraux (@LouisGrx)
Status: Stage IV
Track: Finance
Created: 2019-11-20
---
|-------------------------|------------------------|-----------|------------|


# AGP-Z: A simple Network Budget

## File changed (AGP-0 or AGP-1)
AGP-1

## Link to proposed change

[PR containing changes to AGP-1](https://github.com/aragon/AGPs/pull/149/files?short_path=618aa76#diff-618aa76b7b989ee736b05e779fd24b83)

## Motivation for making this change

Why implement a budget?

- Put a cap on spendings
- Foster discipline in allocating capital

What are qualities to optimize the budget for:

- Legible
- Fair
- Organic
- Low friction
- Not gamable

AGP-103 was voted on and approved during ANV-4. This [AGP](https://github.com/aragon/AGPs/pull/148/files) voices its concerns over the budget as detailed by AGP-103.

Below is a proposal for a new budget, which aims to be simpler and more organic. 

### 1. Determining the budget

Treasury value

It is denominated in DAI. It is defined as the total market value of the Aragon Association multi-sig, net of all existing liabilities. It is snapshotted and calculated at the beginning of each Aragon Network Vote.

The budget

- If the Treasury Value has grown by more than DAI 1M between this ANV and the previous one: the maximum budget spent is 5% of the Aragon Treasury value.
- If the budget has not grow by more than DAI 1M between this ANV and the previous one: the spending is arbitrarily capped to DAI 1M. This is in order to ensure that the treasury doesn't decrease too quickly before Aragon starts growing or appreciating significantly.

### 2.  Allocation process

A simple and elegant way to allocate the budget is to run a dot voting round on proposals that have been approved in a given ANV.

1. All proposals that have been approved in a given ANV as well as all the ongoing recurring proposals go to a Dot Voting round. 
2. The Dot Voting round is ensured by ANT holders, or some other body. This can be changed by ANT holders during a future ANV 
3. The budget -set by the spending cap above- will be split among both the ongoing recurring expenses and the new proposals. 
4. Proposals which do not receive enough funds would *aceept or withdraw* at the end of the DOT voting round. 
5. The unspent capital that is left after withdrawals can go back to the treasury. 

*Buffer rule:*

As initiatives funded through ongoing recurring payments need predictibility, there needs to be a buffer mechanism so these are not out of money from one day to the next. 

This buffer rule can be changed, but it will be initialized as the following: ongoing recurring payments that were decreased by more than 10% in a given Dot voting round takes effect.

1. From the next ANV, for recurring payments > DAI 100K 
2. A month later, for reccurring payments < DAI 100K

Under this mechanism, ANT holders (or the designated body) have the possibility to readjust spendings among different network initatives.

## License

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).
