# Q-Git Governance Change Flow

_**Dependencies:** [Informal Governance Model Definition & Roles](../docs/igm-roles.md)_

The Q-Git Flow (QGF for short) is our primary governance change flow.

---

## Guidelines & Base Definitions

- The `main` branch of the repo is considered the current **Live Release**.
- Each **Release** shall follow a sequential naming convention: Release 0, Release 1, Release 2, etc.
- No changes shall ever be made directly to the `main` branch without following the Release Process as defined below.
- In order for changes to the repo to be valid, they must first be made in a **Working Release** branch, then a pull request must be generated into the `main` branch, then the Release Process must be followed.
- When a Working Release is launched, it becomes the new Live Release, and the prior Live Release becomes one of the Legacy Releases.
- All Contributors are allowed to create **Feature Branches** and submit them for inclusion in a Working Release.
- No more than one **Working Release** may exist at a time.
- A Live Release may not be changed once it is launched, nor may Legacy Releases be changed. They are considered a permanent part of our audit trail.

---

## Process Overview

### Release Process

The process through which Working Releases are created and eventually launched.

1. **Creation**: A new Working Release is created.
2. **Development**: The Development Process is followed to gather and approve contributions to the Working Release.
3. **Finalization**: The Working Release is reviewed, edited, submitted for various levels of feedback & approval, and ultimately either approved or returned for another round of development.
4. **Launch**: After final approval, a Working Release becomes the new Live Release.

### Development Process

The process through which contributions and drafted and eventually approved for inclusion in a Working Release.

1. **Drafting**: A contribution is drafted.
2. **Iteration**: A contribution is submitted for inclusion in a Working Release, and iterated upon with one or more Sponsors.
3. **Merges**: A contribution may optionally be merged with other contributions.
4. **Approvals**: A contribution is either approved or rejected for inclusion in a Working Release.

---

## Release Process Detail

### Release Roles

Each Working Release has the following roles associated with it.

- **Point**: Coordinates the release and is responsible for key decisions.

### Step 1: Creation

...

### Step 2: Development

...

### Step 3: Finalization

...

### Step 4: Launch

...

---

## Development Process Detail

### Development Roles

Each contribution has the following roles associated with it.

- **Drafters**: One or more Contributors who help draft and iterate the contribution.
- **Supporters**: One or more Members who help advice and support the process, but do not directly contribute.
- **Sponsors**: One or more Partners who guide the contribution through the approval process.

## Step 1: Drafting

...

## Step 2: Iteration

...

## Step 3: Merges

...

## Step 4: Approvals

...


