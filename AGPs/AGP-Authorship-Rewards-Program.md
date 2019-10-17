---
AGP: N/A
Title: AGP Authorship Rewards Program
Author: burrrata (@burrrata)
Status: Stage IV
Track: Association
Created: 2019-10-02
---

# AGP-X: AGP Authorship Rewards Program

## Description of desired Association policy change

The Aragon Association ("AA") will reward AGP authors and contributors with ANT at the end of every Aragon Network Vote ("ANV") cycle after ANT votes have been finalized and announced. The ANT rewards will be:
- 300 ANT to be split between any listed authors of an AGP that is approved by the AA for an upcoming ANV.
- 200 ANT to be split between any listed contributors of an AGP that is approved by the AA for an upcoming ANV.
- 300 ANT to be split between any listed authors of an AGP that is approved by ANT voters.
- 200 ANT to be split between any listed contributors of an AGP that is approved by ANT voters.

To receive authorship rewards AGP authors must include an Ethereum address that can receive the ANT ERC-20 token in the proposal. This can be added to the `Author` section in the header of the AGP. Names and addresses listed in the `Author` section of the header should be treated as authors or co-authors in regards to AGP authorship rewards.

To receive contributor rewards AGP authors must also include a list of contributors and their Ethereum addresses. This can be added to the `Author` section in the header of the AGP, however, it must be specified that these are contributors and not main authors. All names and addresses in the `Author` section will be treated as co-authors unless otherwise marked as co-authors. If AGP authors do not list contributors in an AGP, then the contributor rewards will simply not be paid out. The AGP author will not be paid more.

The following example shows what an AGP `Author` section with 2 co-authors and 2 contributors would look like:
- Author: burrrata (@burrrata) 0xa328500Eab14b26C93AA6D1b25698b895F35f5Ee, not-burrrata (@not-burrrata) 0x01b25698b85b26C90Eab14a323AA6D895F35f5Ee, #contributor also-not-burrrata (@also-not-burrrata) 0x00Eab14a321b25698b85b26C93AA6D895F35f5Ee, #contributor definitely-not-burrrata (@definitely-not-burrrata) 0xa321b25698b8500Eab14b26C93AA6D895F35f5Ee

ANT rewards will be split equally between all AGP authors. If a community member has contributed a lot they can be listed as a co-author and the authorship reward can be split between co-authors. Overall, this AGP aims to encourage collaboration by rewarding and recognizing community members who contribute to AGP conversations.

If an AGP author lists contributors, ANT rewards will be split equally between all contributors equally. While this does not account for the fact that some contributors will have done more work than others, it keeps things simple and is a major step forward from the current situation.

In order to receive authorship or contributor rewards, authors and/or contributors must provide an Ethereum address where they wish to receive authorship or contributor ANT rewards.

## Motivation for changing this Association policy

Aragon is a decentralized governance platform. AGPs are the foundation of Aragon's governance process. Engaging in governance is hard. It takes lots of time, emotional energy, and time. There is currently no motivation to engage in AGP discussions or author AGPs other than altruism or personal interest. This greatly reduces the time and effort spent on AGPs.

To address this we need to reward AGP authors. They are doing the Aragon community a service by engaging in discussions, packaging ideas into AGPs, receiving community feedback on those AGPs, modifying AGPs based on that feedback, and then moving AGPs through the various stages of the ANV process. Again, this takes a lot of work and time, but it's important because AGPs are one of the most important aspects of the Aragon community.

Passing the community review and Aragon Association review periods disqualifies any completely spammy proposals. If an AGP makes it through both review periods it could be assumed that it is adding some value to the community. If an AGP Passes in an Aragon Network Vote that clearly shows that ANT holders appreciate the proposal and want the value that it creates. AGP authors and contributors do a lot of work to provide this value to the Aragon network and they should be rewarded accordingly.

## License
Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).
