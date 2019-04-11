# Aragon Association Board of Directors AGP Vote Procedure

As detailed in AGP-1, when an AGP moves to Stage IV the Aragon Association Board of Directors will review the final draft AGP and vote to either reject the proposal or approve it and add it to the ballot of AGPs that will be voted on by ANT holders during the next Aragon Network Vote.

## Preparation procedure
This is what the board will do to prepare so that their votes can be verified. This only has to be done once for each Ethereum account that will be used to vote.

1. Each board member will publish a PGP signed statement verifying the Ethereum account they will use to cast their vote approving or rejecting a proposal. This statement will be published in the `ethereum` [sub-directory](signatures/ethereum) of the AGPs repo.

Example:

   `keybase pgp sign -m "I, Firstname Lastname, with Keybase account @examplename, hereby confirm that, as a Board Member of the Aragon Association, I will use the Ethereum account 0xExample to cast my vote approving or rejecting AGPs." -c > AGP_address_verification.sig`

2. Each board member will add their designated Ethereum account to an Aragon organization set up for the board votes.

## Vote procedure
This is the procedure that the board will follow to submit their officially recorded votes. This has to be done for each Aragon Association Board of Directors AGP vote.

1. After AGP Editors move an AGP to Stage IV, the AGP will be added to the agenda for the next Aragon Association Board of Directors AGP vote.

2. During the Stage IV review time, the board members will download the raw version of the AGP as identified by the last commit when the status was changed to Stage IV and review the AGP in full.

Example:

   `wget https://raw.githubusercontent.com/aragon/AGPs/8c945258fc58c842752a49946514815a4fdd971d/AGPs/AGP-1.md`

3. One of the board members will be nominated to submit a proposal for each AGP under consideration to the Aragon organization. The AGP will be referenced by its name, a link to the proposal, and the SHA-256 hash of the raw file. 

Example:

   `Question: Should AGP-1 be approved for the final ballot of ANV-0? (https://raw.githubusercontent.com/aragon/AGPs/8c945258fc58c842752a49946514815a4fdd971d/AGPs/AGP-1.md)(4f0e9d7782fa5c1ca82ada0aba7b80cd64ba372859c5052216fe65daa1b81479)`

3. Each board member will cast their vote in the Aragon organization using their designated Ethereum account.

4. There are two possible outcomes from the board vote:

    - If the board unanimously agrees to put the AGP to a vote, then an AGP Editor will update the AGP status to Stage V and it will be added to the list of AGPs that will be voted on during the next ANT vote cycle, located in the current votes file within the [votes folder](https://github.com/aragon/AGPs/tree/master/votes) in the AGPs repo. 

    - If the board disagrees or unanimously rejects the proposal, then an AGP Editor will update the AGP status to Rejected.
