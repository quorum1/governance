# Q-Git Governance Change Flow

_**Dependencies:** [Informal Governance Structure Definition & Roles](../docs/igs-roles.md)_

The Q-Git Flow (QGF for short) is our primary governance change flow.


## Guidelines & Base Definitions

- The `main` branch of the repo is considered the current **Live Release**.
- Each **Release** shall follow a sequential naming convention: Release 0, Release 1, Release 2, etc.
- No changes shall ever be made directly to the `main` branch without following the Release Process as defined below.
- In order for changes to the repo to be valid, they must first be made in a **Working Release** branch, then a pull request must be generated into the `main` branch, then the Release Process must be followed.
- When a Working Release is launched, it becomes the new Live Release, and the prior Live Release becomes one of the Legacy Releases.
- All Contributors are allowed to create **Contribution Branches** and submit them for inclusion in a Working Release as outlined in the Development Process.
- All Contributors are also allowed to create **Experimental Branches** for any desired reason or purpose. Though from time to time these may need to be pruned, archived, renamed and/or reorganized.
- During the finalization step of the Release Process, **Resolution Branches** are created by designatees to address key issues.
- No more than one **Working Release** may exist at a time.
- A Live Release may not be changed once it is launched, nor may Legacy Releases be changed. They are considered a permanent part of our audit trail.


## Process Overview

### Release Process

The process through which Working Releases are created and eventually launched.

1. **Creation:** A new Working Release is created.
2. **Development:** The Development Process is followed to gather and approve Contributions to the Working Release.
3. **Finalization:** The Working Release is reviewed, edited, submitted for various levels of feedback & approval, and ultimately either approved or returned for another round of development.
4. **Launch:** After final approval, a Working Release becomes the new Live Release.

### Development Process

The process through which Contributions and drafted and eventually approved for inclusion in a Working Release.

1. **Drafting:** A Contribution is drafted.
2. **Iteration:** A Contribution is submitted for inclusion in a Working Release, and iterated upon with one or more Sponsors.
3. **Merges:** A Contribution may optionally be merged with other Contributions.
4. **Approvals:** A Contribution is either approved or rejected for inclusion in a Working Release.


## Release Process Detail

This process is structured with a higher level of formality because it is our primary safeguard ensuring that only high quality, well-considered changes make it into our governance repo.

### Release Roles

Each Working Release has the following roles associated with it.

- **Release Point (RP):** Coordinates the Release and is responsible for key decisions. Able to delegate authority to others and define the workflow for the Release as long as it doesn't conflict with the definitions in the governance repo. The Release Point must be a Contributor.
- **Stewards:** Play key roles in development and ultimately approve the Release during finalization.
- **Managing Steward (MS):** Helps support the Point, provides architectural guidance, has veto power over approvals, appoints and can change the Point, can overrule decisions made by the Release Point.
- **Designatees:** Designated by the Release Point to develop Resolution Branches as needed during the finalization step.
- **Merge Certifiers:** The final certification step before a Working Release is merged into the `main` branch.

### Step 1 - Creation

A new Working Release can only be created if there is no current Working Release as there can be only one at a time. (If side workspaces are needed, Experimental Branches may be used.)

A new Working Release is created by the MS who also appoints a Release Point.

A new branch is created in the repo with the name `release-#`, where `#` is 1 greater than the current Live Release. The root readme should be updated with a "Work in Progress" section that describes the current status of the release along with any key goals. This section should be kept up to date as work progresses, ideally with checklists, progress meters, or other easy to understand aids.

> \[!NOTE]
> While creating a new release branch, the MS or Release Point are allowed to unilaterally edit any of the `readme.md` files in the gov repo, except for the "Flows & Scopes" section of the flows readme. No approvals are required for this.

### Step 2 - Development

Development progresses with Contribution Branches moving through the Development Process and potentially being approved for inclusion and then being merged into the Working Release branch.

The MS may choose to appoint a new Release Point at any time.

The development step concludes when the Release Point determines that it is ready for finalization.

### Step 3 - Finalization

Upon entering the finalization step, the Release is locked to new Contribution Branches and can only be modified by Resolution Branches.

The finalization process is critical to the overall Release Process. Here are the sub-steps:

- **Step 3a - Steward Review:** Stewards meet on one or more synchronous calls to walk through all changes. These calls must be recorded and preserved indefinitely.
  - All Stewards must be present or must delegate their vote to another Steward.
  - During the calls, potential issues are identified & approved via the following process:
    - Any Steward may flag an issue and they become the first Sponsor of that issue
    - If at least two other Stewards agree to Co-Sponsor the issue, it goes on the list of "Issues to Resolve"
    - If fewer than three Stewards agree to Co-Sponsor the issue, then it goes on the list of "Other Issues" and will not be resolved in the first round of resolutions
    - The MS may veto any issue, but they must do so during a Steward review call and allow for debate. At any point they may choose to retract a prior veto.
    - The Steward review is complete when all changes have been reviewed.
- **Step 3b - First Resolutions:** 
  - The Release Point is responsible for ensuring that the Issues to Resolve are properly documented and assigned to Designatees.
  - The Designatees for each Issue then create a Resolution Branch and work with the Sponsors of the Issue to work it through the Development Process and get it merged back into the Working Release Branch.
  - At any point the Sponsors may agree to retract the Issue and make no changes to the Working Release Branch. In this event, the process continues on, but the Sponsors have another opportunity to voice potential concerns in the following sub-step.
  - This sub-step is finished when all Issues to Resolve are either approved or retracted.
- **Step 3c - Member Review:** 
  - NOTE: This step will be skipped until the governance repo reaches Release 6. The first set of Releases have emerged from prior work and are being fast-tracked.
  - Release 6 should replace the definition of this sub-step.
- **Step 3d - Second Resolutions:** ...
  - NOTE: This step will be skipped until the governance repo reaches Release 6. The first set of Releases have emerged from prior work and are being fast-tracked.
  - Release 6 should replace the definition of this sub-step.
- **Step 3e - Final Review:** NOTE: This sub-step should be redefined in Release 6 to include the Members as well.
  - Stewards meet on one or more synchronous calls to walk through the outcome of all resolutions. These calls must be recorded and preserved indefinitely.
  - All Stewards must be present or must delegate their vote to another Steward.
  - During the call all resolutions are reviewed.
  - Stewards can bring up questions and discuss concerns. They may also share any concerns which would cause them to vote to reject this Release.
  - The final review is complete when all resolutions and open questions have been discussed and when Stewards have agreed on the duration of the approval voting period.
- **Step 3f - Steward Approval:** An asynchronous vote is held.
  - The votes must produce a permanent verifiable audit trail.
  - Stewards may vote to approve or reject the Release:
    - Votes to reject must contain a list of specific Issues to Resolve which would need to be addressed in order for them to approve again in the future.
    - Votes to approve may optionally contain a list of specific Future Issues which the Steward thinks should be addressed in future Releases.
  - All Stewards must either vote or delegate their vote to another Steward. Voting or delegating is mandatory. Any Stewards who will be unavailable during a vote must appoint a delegate beforehand, or a delegate may be appointed on their behalf by the MS.
  - Stewards will have already agreed in the prior sub-step to the duration of the voting period.
  - The MS may unilaterally veto the approval of the Release, but they must hold a synchronous call inviting all Stewards and allowing for debate. The call must be recorded and preserved indefinitely.
  - Once all votes are cast:
    - 75% or greater approval causes the Working Release to be approved and move forward to the launch step.
    - Less than 75% approval (or a veto from the MS) causes the Working Release to be sent back to development step.

### Step 4 - Launch

Once a Working Release is approved for launch, the launch proceeds according to the steps outlined in this section.

A pull request is made from the Working Release branch into the `main` branch. Summaries of all parts of the finalization step must be posted to the pull request, including links to each video recording as well as verifiable evidence of each Steward's vote.

Once all key context is posted to the pull request, the pull request must be reviewed and approved by four Members (referred to as the Merge Certifiers), specifically:
- The MS
- The Release Point
- 2 Stewards (not including the MS & RP), selected by the RP

The Merge Certifiers must not exercise additional editorial review or approval during this step. Their sole responsibility is to ensure that the processes outlined in this flow have been followed and documented appropriately.

If certified, each Merge Certifier approves the pull request in Github. If not certified, a Merge Certifier must communicate the remaining issues to the rest of the Merge Certifiers and work with them to resolve the missing items. This might require rewinding the process, or it might mean simply adding more context to the pull request.

Once the Working Release is merged into the `main` branch, it is considered the new Live Release, and the Release Process may begin again.


## Development Process Detail

This process is structured with less formality and more flexibility because it is intended to support stigmergic contributions and emergent innovation.

Members are encouraged to innovate on top of the basic process outlined below, perhaps experimenting with additional structures and collaboration mechanisms which encourage more creative and thoughtful contributions, generate more work joy, or achieve other desirable outcomes.

### Development Roles

Each Contribution has the following roles associated with it, collectively referred to as the **Contribution Team**.

- **Drafters:** One or more Contributors who help draft and iterate the Contribution.
- **Supporters:** One or more Members who help advise and support the process, but do not directly contribute.
- **Sponsors:** One or more Stewards who guide the Contribution through the approval process.
- **MS:** Able to expedite approvals.

### Step 1 - Drafting

Any group of Drafters may team up to draft a Contribution by creating a Contribution Branch.

Any Contributors who are not confident enough with Github to draft a Contribution themselves are encouraged to team up with other Contributors who are skilled with Github. Non-Contributor Members cannot be Drafters themselves but they are encouraged to be Supporters or to become Contributors.

At any point in the drafting process, Drafters may seek to find one or more Stewards to Sponsor their Contribution. At least one Sponsor is needed to move to the next step.

### Step 2 - Iteration

Once the initial drafting is complete and at least one Sponsor has agreed to support the contribution, the iteration step begins.

This step can proceed however the the Contribution Team desires, but the basic idea is that they should all work together to iterate on the contribution until the Sponsors feel that it's ready to proceed towards approval.

### Step 3 - Merges

This is an optional step which the Sponsors may request (or potentially require) in order to effectively manage Steward bandwidth. Because the approval step requires Steward voting, it may often be desireable to merge many contributions into a single contribution.

The precise process of designing a merge is up to the Contribution Team. The logistics are that multiple Contribution Branches are merged into a single Contribution Branch.

If used, this step will also result in merging the Contribution Teams.

### Step 4 - Approvals

The final step is for the Sponsors to formally submit the Contribution for approval. The approval may proceed via the normal process or the expedited process.

> \[!NOTE]
> The MS or Release Point are allowed to unilaterally approve Contribution Branches which only include changes to `readme.md` files, except for the "Flows & Scopes" section of the flows readme. It may be necessary for other users to approve the pull request for technical reasons, but no video needs to be made and no formal review needs to be recorded. A simple written note in the pull request is sufficient.

The precise method of this submission, and the review process itself is defined by the Release Point as part of their workflow design. But it must meet the following criteria:
- The Sponsors should create a pull request from the Contribution Branch into the Working Release Branch. The pull request should include:
  - All requisite context needed in order for Stewards to render an informed vote.
  - A short video walkthrough which explains the reasoning behind the contribution and walks through the changes.
  - Important Note: Any videos & supporting materials which are stored outside of Github *must* be stored in a place where they can be maintained indefinitely, and in a manner which is aligned with the RP's workflow design for the Release. Cloud-based apps which are not part of Quorum1's long-term systems plan (such as Loom) are not acceptable.
- **Normal Approval Process:** Stewards must be able to vote in a manner aligned with these requirements:
  - Voting is asynchronous (though synchronous sessions can be supported as long as they are optional)
  - Votes must produce a permanent verifiable audit trail
  - Stewards may vote to approve or reject the Contribution
    - Votes to reject must contain a list of specific Issues to Resolve which would need to be addressed in order for them to approve this Contribution in the future.
    - Votes to approve may optionally contain a list of specific Future Issues which the Steward thinks should be addressed in future Contributions.
  - All Stewards must either vote or delegate their vote to another Steward. Voting or delegating is mandatory.
  - The duration of the voting period for Contributions should be made clear to Stewards ahead of time.
  - The MS may unilaterally veto any Contribution, but they must invite asynchronous feedback from any interested Members and must respond to the feedback. They may retract their veto at any point.
  - Once all votes are cast:
    - The full details of the vote must be recorded on the pull request.
    - 75% or greater approval causes the Contribution to be approved.
    - Less than 75% approval (or a veto from the MS) causes the Contribution to be rejected.
- **Expedited Approval Process:** This process may be used when increased speed is desireable.
  - The Sponsors may request that the MS expedite the approval process.
  - If the MS agrees, then the full Steward approval process above is still followed, but with the Sponsors and the MS (and potentially other Stewards as requested by the MS) standing in for all of the Stewards.
  - The approval process must include at least two Stewards, including the MS. This means that if the MS is also the only Sponsor, then at least one additional Steward must be included in the approval process.
  - Note 1: Even during an expedited approval process, a pull request meeting the requirements above must be created.
  - Note 2: The expedited approval process only applies to in the Development Process of specific Contributions. All changes must eventually be reviewed by the full Steward group during Release finalization.
- Rejected Contributions have their pull request closed. They may be tweaked and resubmitted later.
- Approved Contributions have their pull request approved (by both the Release Point and the MS) and are then merged into the Working Release Branch.

