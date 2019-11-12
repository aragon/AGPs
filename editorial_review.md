# AGP Editorial Review

This document defines the process by which AGP Editors review and shepherd Aragon Governance Proposals (AGPs) through the AGP process. This is not a binding document and there is no strict requirement to follow this process, as long as any deviations remain compliant with the expectations outlined in [AGP-1](https://github.com/aragon/AGPs/blob/master/AGPs/AGP-1.md). Rather this document exists to assist AGP Editors throughout the review process and to help train any contributors who join as a new AGP Editor.

## The AGP Editorial Process

The basic steps in the AGP Editorial Process are:

1. Review
2. Discuss
3. Finalize
4. Update AGP status
5. Record vote outcome
6. (Meta-track only) Merge proposed Amendment PR

A more detailed explanation of each step follows.

### 1. Review

During AGP-1 Stage III and Stage IV, AGP Editors will review proposals submitted as a pull request to the AGPs repo for typos, formatting errors, and compliance with AGP-1, and offer suggestions to fix any issues. A typo or formatting issue does not by itself invalidate a proposal, but AGP Editors should strive to make sure all proposals are clearly legible and subject to as little mis-interpretation as possible. Ensuring AGP-1 compliance is, on the other hand, mandatory per AGP-1 itself.

### 2. Discuss

AGP Editors will respond to comments and questions in response to their review to push progress forward on the proposal toward finalization and Stage V status. Note that the role of AGP Editors is not to comment on the subjective qualities of a proposal (e.g. comments such as: "I don't support this because..." or "I think you should ask for this much money instead...") beyond the question of whether or not a proposal is compliant with AGP-1. If such comments are made by AGP Editors it should be made clear that they are made in the capacity of private commenter and not as an AGP Editor, and ideally in a venue other than the AGPs repo, such as an outside forum thread (again, not a hard requirement here, just a best practices suggestion to keep the discussion clean and compartmentalized).

### 3. Finalize

After a proposal author has signaled their intention to finalize the proposal and move it to Stage V in the AGP process, AGP Editors will give a final review, push any remaining typo and formatting fixes, and, if the proposal is compliant with AGP-1, assign the AGP a number, change the status in the AGP document to Stage V, and update the label on the pull request to "Stage V".

A checklist may be used by AGP Editors and published in their update commit to transparently show that, to the best of their knowledge, an AGP approved to move on to Stage V meets the requirements set forth in AGP-1 and is ready for the Aragon Association review.

```
[] AGP-1 compliant
[] No formatting, grammar, or spelling errors
[] Status updated to Stage V in the AGP file and GitHub label
[] AGP number assigned (see file name AGP-X.md, AGP file header, and AGP title)
```

### 4. Update AGP status

After moving an AGP to Stage V, the status of an AGP will be updated up to two more times:

1. After the Aragon Association review concludes and the Board of Directors has [cast their votes](aa_board_review.md), the status of an AGP is updated as being either `Rejected (Aragon Association)` or `Stage VI`. 
- Proposals are rejected and their pull request closed if they have not been unanimously approved by the board. If the proposal being rejected is a Meta track proposal, then the Amendment PR is also closed at this stage (see section 6 below for more details).
- Proposals that are approved by the board are merged into the AGPs repo and go on to Stage VI of the AGP process, the Aragon Network Vote. These proposals are recorded in a file containing the final ballot in the [votes](votes) folder, the purpose of which is to serve as an easy to read, historical reference regarding information about a vote. If the proposal is Meta track proposal, then only the AGP pull request is merged at this stage (see section 6 below for more details).

2. After the Aragon Network Vote, the status of an AGP is updated as being either `Rejected (ANT Holders)`, `Approved`, or `Superseded by AGP-X`.
- Approval is subject to the requirements defined in AGP-1 and is hard-coded into the Voting app used by ANT holders. Any proposal not approved is considered rejected.
- A proposal has been `Superseded by AGP-X` if an AGP is approved in an Aragon Network Vote that explicitly supersedes an earlier proposal, deprecating the old proposal in favor of the new one. The `X` in `Superceded by AGP-X` should be replaced with the specific number of the AGP that supersedes the AGP in question.

### 5. Record vote outcome
The outcome of the Aragon Network Vote is recorded in the same file created in the [votes](votes) folder to record the final ballot. Links to the Voting apps used are also included in this file. See for example the record for [Aragon Network Vote #1](votes/2019-01-24-AN-Vote-1.md). The blockchain will of course remain the official reference record regarding the outcome of any ANT vote.

- Approved AGPs should also be listed in the [Governance page](https://wiki.aragon.org/network/governance/overview/) of the Aragon wiki.

### 6. (Meta-track only) Merge proposed Amendment PR

Meta-track proposals contain amendments to either AGP-0 or AGP-1, and thus have two pull requests associated with them: one with the text of the AGP itself ("AGP PR") and one that makes the proposed change to the original document ("Amendment PR"). The Meta track AGP [template](https://github.com/aragon/AGPs/blob/master/templates/meta_template.md#instructions) explains the process for AGP authors.

If a Meta-track AGP is approved in the Aragon Network Vote, the Amendment PR is merged by an AGP Editor. If the Meta-track PR is rejected by either the Aragon Association or in the Aragon Network Vote, then the Amendment PR is closed by an AGP Editor.
