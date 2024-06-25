# Quorum1 Governance Change Flows

Each file in this folder defines a governance flow ("flow" for short). Flows define how different parts of the governance repo are changed. Collectively they are our "meta governance process" (the change management process for our governance design).

Each flow has specific scope which is defined here, in this readme file.

## Flows & Scopes

Any time a change is made to the governance repo it must be in compliance with all applicable flows, based on the scopes defined in this section.

Any changes which are later determined to have been made out of compliance with one or more of the in-scope flows as defined at the time of the change will be considered invalid and must be re-processed in accordance with the currently in-scope flows.

### Q-Git Flow

**Scope:** All changes to the governance repo are in-scope for this flow, unless otherwise specified.

The Q-Git Flow (QGF) is our base change flow. For now, all of our other flows inherit from this flow and build on top of it, though that may change in the future.

### Financial Model Change Flow

**Scope:** Only changes to the `/docs/financial-model.md` are in-scope for this flow.

Specifies additional steps required for changing the Financial Model.

