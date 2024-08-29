# Org Investment Ledger Design

_**Dependencies:** [Informal Governance Model Definition & Roles](./igs-roles.md), [Org Investment Ledger Governance Flow](../flows/org-investment-ledger-governance.md)_

This doc is the formal [Org Investment Ledger Design](./glossary.md#org-investment-ledger-design) in alignment with the requirements of the [Financial Model](./glossary.md#financial-model).

The Org Investment Ledger is the only investment ledger mandated by the Financial Model. The core ledger includes a mandatory allocation to the Org Investment Ledger, meaning that a share of all Quorum1 revenue will pass through to this ledger. This ledger is a critical part of Quorum1’s financial infrastructure and key to our long-term sustainability. As such, the design of the Org Investment Ledger must meet our highest standard.

## Ledger Details

| Property          | Value                 |
| ----------------- | --------------------- |
| **Manager**       | Hank Holiday (Q0001)  |
| **Type**          | Investment Ledger     |
| **Status**        | Active                |
| **Receivable**    | Yes                   |

## Governance Process

In alignment with the Quorum1 Governance Repo meta governance process, changes to this doc are scoped to the Org Investment Ledger Governance Flow, linked to from the dependencies list at the top of this doc.

## Allocation Model

Investment outflows require the approval of the Ledger Manager and at least two additional Partners.

## Core Parameters

| Parameter                     | Value                                                         |
| ----------------------------- | ------------------------------------------------------------- |
| **Ledger Budget**             | $825M Full Value / $55M Face Value (Average Multiple: 15x)    |
| **Min Multiple**              | 1.0x                                                          |
| **Max Multiple Downgrade**    | 90%                                                           |

## Rev Token Cohorts

The rev token cohorts are as defined below. We will generally create one parent cohort for each year with nested sub-cohorts to track important groupings of rev tokens.

For naming purposes: 2020 is known as “year 0”, 2021 is known as “year 1”, etc.

### Top-Level Grouping Cohorts

| Id | Name | Status | Face Value | Multiple | Full Value |
| --- | --- | --- | --- | --- | --- |
| 2020 | Year 0: All | Closed | $100K | 100x | $10M |
| 2021 | Year 1: All | Active | $260K | 100x | $26M |
| 2022 | Year 2: All | Active | $590K | 75x | $44.25M |
| 2023 | Year 3: All | Active | $600K | 50x | $30M |
| 2024 | Year 4: All | Active | $10.1M | ~33.1x | $334M |
| - | **Total** | - | **$11.65M** | **~38.1x** | **$444.25M** |

### Nested Grouping Cohorts

| Id | Name | Status | Face Value | Multiple | Full Value |
| --- | --- | --- | --- | --- | --- |
| 2024.money | Year 4: Money | Active | $6.1M | ~28.5x | $174M |

### Money Cohorts

| Id | Name | Status | Face Value | Multiple | Full Value |
| --- | --- | --- | --- | --- | --- |
| 2021.money | Year 1: Money | Active | $30K | 100x | $3M |
| 2022.money | Year 2: Money | Active | $10K | 75x | $750K |
| 2023.money | Year 3: Money | Active | $10K | 50x | $500K |
| 2024.money.informal | Year 4: Informal | Active | $100K | 40x | $4M |
| 2024.money.seed1 | Year 4: Seed Tranche 1 | Active | $1M | 40x | $40M |
| 2024.money.seed2 | Year 4: Seed Tranche 2 | Planned | $1M | 35x | $35M |
| 2024.money.seed3 | Year 4: Seed Tranche 3 | Planned | $1M | 30x | $30M |
| 2024.money.seed4 | Year 4: Seed Tranche 4 | Planned | $1M | 25x | $25M |
| 2024.money.seed5 | Year 4: Seed Tranche 5 | Planned | $2M | 20x | $40M |
| - | **Total** | - | **$6.15M** | **~29x** | **$178.25M** |

### Time Cohorts

| Id | Name | Status | Face Value | Multiple | Full Value |
| --- | --- | --- | --- | --- | --- |
| 2020.time | Year 0: Time | Closed | $100K | 100x | $10M |
| 2021.time | Year 1: Time | Active | $230K | 100x | $23M |
| 2022.time | Year 2: Time | Active | $580K | 75x | $43.5M |
| 2023.time | Year 3: Time | Active | $590K | 50x | $29.5M |
| 2024.time | Year 4: Time | Active | $4M | 40x | $160M |
| - | **Total** | - | **$5.5M** | **~48.4x** | **$266M** |

## Investment Rounds

### IR1: Legacy Investment Round

**Round Organizers:** All Partners

**Included Cohorts:** 2020, 2021, 2022, 2023

Financial Model v2 was only finalized in late 2023 (year 3). As such, the legacy investment round (IR1) exists to retroactively allocate rev tokens & rev points for year 0 through year 3. All of the money rev tokens in IR1 are for informal investment. 

It's important to note that since Quorum1 doesn't have any traditional stock or other recompense to founders or early members, IR1 represents the only potential financial reward for the many years of foundational work put into Quorum1 by its members in the early years. As such, IR1 is critical to maintaining trust and fairness and is key to our ongoing success.

The actual execution of IR1 will begin soon after IR2 produces enough cash to invest in the work required.

#### IR1: Informal Investment Guidelines

**For year 0:** Only time rev tokens are being created for year, there will be no money rev tokens to allocate.

**For year 1, 2, and 3:** A pass-through ledger will be created to manage the retroactive issuance of the rev tokens. The process used to allocate them should resemble this:

1. First any money investments will be collected, documented, totaled, and issued as money rev tokens up to the max face value from the table above.
2. These cash investments will specifically include the unpaid legal fees to initial legal counsel less any amounts paid on the Initial Counsel Profit Share to date (full details outlined in [Changes from Legacy Financial Model](#changes-from-legacy-financial-model)).
3. If the final documented amount is under the budget established in the rev token cohort definitions, then the remaining amount will not be issued as rev tokens. If the final documented amount is over the max face value from the table above, then the overage amount will be awarded instead as rev points from the time investment pool in the same year cohort.

#### IR1: Rev Point Plan

**For year 0:** Only time rev tokens are being created for year 0 and will be awarded as rev points to the meta founder as a replacement for the originally planned meta-founder entitlement. Full details outlined in [Changes from Legacy Financial Model](#changes-from-legacy-financial-model).

**For year 1, 2, and 3:** A pass-through ledger will be created to manage the retroactive issuance of the rev points. The rev points will be allocated amongst all individuals who were members during that year via a participatory retroactive valuation process agreed on by at least 60% of the members from that year who remain active members and are engaged enough to participate in the decision-making process.

**For year 1 and year 2:** Member Q0005 will be awarded 750K rev points in each year (for a total of 1.5M rev points) as a replacement for the originally planned prime founder entitlement. Full details outlined in [Changes from Legacy Financial Model](#changes-from-legacy-financial-model).*

### IR2: Internal Seed Investment Round

**Round Organizers:** Q001, Q0022, Q0055, Q0175

**Included Cohorts:** 2024.money.informal, 2024.time

#### IR2: Informal Investment Guidelines

Only the rev tokens in the 2024.money.informal cohort are available for informal investment. These are to be allocated for informal cash investments during 2024 and for documented & approved expenses incurred by members directly related to the investment round or critical Quorum1 operations.

#### IR2: Rev Point Plan

Before the 2024.time rev points are allocated, this section will be updated with a detailed plan. The plan should align with the goal of rewarding all members who make material contributions to Quorum1 in 2024.

When possible the rewarding should be based on time tracked in Quorum1's time tracking system and should align with the following rates:
- **Investment Round Related Work:** 6,000 rev points per hour
- **Foundation-Led Work:** 4,000 rev points per hour
- **Other Work:** 2,000 rev points per hour

### IR3: External Seed Investment Round

**Round Organizers:** Q001, Q0022, Q0055, Q0175

**Included Cohorts:** 2024.money.seed1, 2024.money.seed2, 2024.money.seed3, 2024.money.seed4, 2024.money.seed5

#### IR3: Informal Investment Guidelines

This round will not include any informal investment.

#### IR3: Rev Point Plan

This round will not include any time investment.

## Payment Algorithm Parameters

### Time-vs-Money Split Rate (TVMSR) Guidelines

The [TVMSR](./glossary.md#time-vs-money-split-rate) is decided by the Ledger Manager with input from the Partners.

The TVMSR can be changed from payment to payment according to the needs of Quorum1. The goal, however, should be to maintain an average TVMSR of roughly 50/50.

Additionally, the percentage allocated to either type may not drop below 30%. This means that the allowed range of TVMSR values is from 30/70 to 70/30.

### Rev Token Payment Weighting

When processing a money rev token sub-payment, the sub-payment will be split across all active money rev token recipients proportional to their total full values.

### Rev Point Payment Weighting

This section of the design has yet to be defined. The guidance will likely be similar to the rev token payments, but a bit more complex as it needs to allow members to opt-out of payments.

In general, the payments should be proportional to each member's rev point balance but, as specified in the Financial Model, the process should allow members to decide not to receive a payment in a given month.

## Token Downgrades

There have been no token downgrades.

---

# Appendix

## Ledger Liquidation Preferences

In the event of the full liquidation of the Org Investment Ledger for any reason, all token holders must convert at the same discount rate, weighting, or liquidation preference.

## Changes from Legacy Financial Model

The legacy financial model (aka Financial Model v1) is the set of agreements which preceded Financial Model v2. It included a number of “mandatory revenue disbursements”, outlined in Section 7 of the Operating Agreement, which have been retired and replaced as part of this new design.

This section outlines each of the retired structures and what replaces each of them. The replacement structures are all outlined in the [ Rev Token Cohorts](#rev-token-cohorts) section.

- **Meta Founder Revenue Share:**
    - **Financial Model v1:** 1% of gross revenue is paid to the meta founder for 20 years from initial incorporation.
    - **Original Intention:** An exchange for the initial thought work and effort that went into conceiving and founding of Quorum1.
    - **Financial Model v2:** This disbursement is removed and replaced by the 2020 rev point cohort issued to the meta founder, valued at $10M rev points ($100k at a 100x multiple).
- **Prime Founder Profit Share:**
    - **Financial Model v1:** 10% of gross profit is paid to prime founders for 10 years from initial incorporation, who are the first 10 members to earn 500 Q-Credits, with 3% to prime founder 1, 2% to prime founder 2, etc.
    - **Original Intention:** An incentivization program to reward members for early contributions to the founding and growth of Quorum1.
    - **Financial Model v2:** The prime founder program was ended after 12/31/2022 with only two members having achieved prime founder status: Members Q0005 and Q0001. Q0001 agreed to give up their place, thus there was only one prime founder: Q0005.
        - The year 1 and 2 rev point cohorts include a total of 1.5M rev points (split equally between the two years) to Q0005 to replace the legacy entitlement. This amount was arrived at by estimating the value of the legacy entitlement to be 3% of a 20% profit margin against $250M of potential cumulative 10 year revenue, or $1.5M.
        - It’s important to note that a number of other members made significant contributions and were on track to become prime founders before the program was ended. 
        - The 1.5M rev points mentioned above are intended only to compensate Q0005 for winning the game as it was designed. However, all members will be compensated for their contributions via the participatory processes used to allocate the remaining rev options for years 1, 2, and 3. The total available rev points for those years could be as high as 90M, which will leave plenty of space for the ultimate allocation to be fair.
        - This program was ultimately discontinued because the incentivization structure was deemed to have been poorly designed. The fact that only one prime founder was formally recognized is not considered to be a completely fair outcome, but that is how the rules worked out.
- **Initial Counsel Profit Share:**
    - **Financial Model v1:** 6.25% of gross profit is paid to initial legal counsel for 3 years from initial incorporation.
    - **Original Intention:** An exchange for initial legal counsel having graciously offered heavy discounts, and in some cases not passing on incurred expenses, during the initial entity formation and early legal development of Quorum1.
    - **Financial Model v2:** The legacy mechanism is retired and in the rev token cohorts for years 1 through 3, the unpaid legal work is instead converted into rev points, less any amount paid out via the legacy mechanism.
