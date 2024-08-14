# Org Investment Ledger Design Guidelines

The [Org Investment Ledger](#org-investment-ledger) is the only investment ledger mandated by the Financial Model. The [Core Ledger](#core-ledger) includes a mandatory allocation to the org investment ledger, meaning that a share of all Quorum1 revenue will pass through to this ledger. This ledger is a critical part of Quorum1’s financial infrastructure and key to our long-term sustainability. As such, the design of the org investment ledger must meet our highest standard.

The org investment ledger design itself is officially considered part of the Financial Operations Plan and is thus changed according to the more streamlined [Change Process for Financial Operations Plan](#change-process-for-financial-operations-plan).

However, the Financial Model does impose some guidelines on the org investment ledger design. This section outlines those guidelines. Making changes to any of these guidelines requires modifying this doc in accordance with the [Change Process for Financial Model Definition](#change-process-for-financial-model-definition). 

## Guideline 0 - Launching the Ledger

At the time of writing and approving this Financial Model, the org investment ledger has yet to be launched. The initial launch should align with the guidelines outlined in this section and should follow the [Standard Process for Designing an Investment Ledger](#standard-process-for-designing-an-investment-ledger).

## Guideline 1 - Core Parameters

The core parameters must match the following.

- **Ledger Budget:** $825M Full Value / $55M Face Value (Average Multiple: 15x)
- **Min Multiple:** 1.0x
- **Max Multiple Downgrade:** 90%

**How to Contextualize the Ledger Budget:**

> [!NOTE]
> The ledger budget above is built around the goal of getting to a billion dollars in revenue in 2034 (with at least 5% of gross revenue going to rev token payments).

The precise rev token payment amount in any future year will depend on both the amount of org revenue and the “org rev share allocation” (the net allocation to org investment ledger rev token payments as a portion of overall revenue).

The org rev share allocation percentage in a year will be a factor of (1) the average core ledger allocation percentage across the blend of revenue sources (refer to [Standard Income Allocations](#standard-income-allocations)) in that year and (2) the average percentage allocated by the [Core Ledger](#core-ledger) to the [Org Investment Ledger](#org-investment-ledger) over the year. This means that if the quorum is able to grow higher-margin revenue sources the org rev share allocation will generally increase, but also that the Foundation may impact the the org rev share allocation through the way it manages the core ledger allocation model.

## Guideline 2 - Rev Token Cohorts

Cohorts have a time period (default is a year) and share the same multiple. At a minimum a Cohort is created for each calendar year and sub-cohorts created for each important subdivision there within. 2020 is known as “year 0”, 2021 is known as “year 1”, etc.

The legacy cohorts for years 0 through 3 are listed below and will match these tables exactly, except that the actual face value, which must be under the maximums defined below, will be determined via a participatory process (to be determined by the Foundation) that runs soon after v2 of the Financial Model is initially approved and adopted.

**Legacy Money Rev Tokens:**

| Year | Max Face Value | Multiple | Max Full Value |
| --- | --- | --- | --- |
| Year 0 - 2020 | $0 | 100x | $0 |
| Year 1 - 2021 ² | $70K | 100x | $7M |
| Year 2 - 2022 ² | $20K | 75x | $1.5M |
| Year 3 - 2023 ² | $10K | 50x | $500K |
| **Legacy Total** | **$100K** | **90x (avg)** | **$9M** |

**Legacy Time Rev Tokens:**

| Year | Face Value | Multiple | Full Value |
| --- | --- | --- | --- |
| Year 0 - 2020 ¹ | $100K | 100x | $10M |
| Year 1 - 2021 ² ³ | $230K | 100x | $23M |
| Year 2 - 2022 ² ³ | $580K | 75x | $43.5M |
| Year 3 - 2023 ² | $590K | 50x | $29.5M |
| **Legacy Total** | **$1.5M** | **70.67x (avg)** | **$106M** |
- ***¹ For year 0:** Only time rev tokens are being created for year 0 and will be awarded as rev points to the meta founder as a replacement for the originally planned meta-founder entitlement. Full details outlined in [Changes from Legacy Financial Model](#changes-from-legacy-financial-model).*
- ***² For year 1, 2, and 3:** A pass-through ledger will be created to manage the retroactive issuance of the rev tokens and rev points.*
    - *For money rev tokens: First any money investments will be collected, documented, totaled, and issued as money rev tokens up to the max face value from the table above. These cash investments will specifically include the unpaid legal fees to initial legal counsel less any amounts paid on the Initial Counsel Profit Share to date (full details outlined in [Changes from Legacy Financial Model](#changes-from-legacy-financial-model)). If the final documented amount is under the max face value from the table above, then the remaining amount will not be issued as rev tokens. If the final documented amount is over the max face value from the table above, then the overage amount will be awarded instead as rev points from the time investment pool in the same year cohort.*
    - *For time rev tokens: The rev points will be allocated amongst all individuals who were members during that year via a participatory retroactive valuation process agreed on by at least 60% of the members from that year who remain active members and are engaged enough to participate in the decision-making process.*
- ***³ For year 1 and year 2:** Member Q0005 will be awarded 750K rev points in each year (for a total of 1.5M rev points) as a replacement for the originally planned prime founder entitlement. Full details outlined in [Changes from Legacy Financial Model](#changes-from-legacy-financial-model).*

**The first live cohort will be year 4, defined below (including budget).**

**Year 4 Money Rev Tokens:**

| Year | Max Face Value | Multiple | Max Full Value |
| --- | --- | --- | --- |
| Year 4 - 2024 ¹ | $5M | 40x | $200M |
| **Total from Y0 - Y4** | **$5.1M** | **41.0x (avg)** | **$209M** |

**Year 4 Time Rev Tokens:**

| Year | Max Face Value | Multiple | Max Full Value |
| --- | --- | --- | --- |
| Year 4 - 2024 | $4M | 40x | $160M |
| **Total from Y0 - Y4** | **$5.5M** | **48.4x (avg)** | **$266M** |
- ***¹ For year 4:** Money rev tokens will be allocated to a formal org investment round managed by the meta founder with all critical parameters requiring the 60% agreement of the partner members. The precise amount of Rev Tokens and their Face Value will be determined by the total amount purchased by investors in the formal org investment round, as well as any additional informal investment.*

**The org investment ledger’s governance process will begin determining annual rev token cohorts starting in year 5 (2025).**

## Guideline 3 - Allocation Model

The rev token weighting algorithm for the org investment ledger will stay consistent over time to maximize predictability. 

The rev token payments shall be processed in alignment with the following algorithm:

1. The overall rev token payment is split into two sub-payments, one for each type of rev token: A time rev token payment and a money rev token payment.
    1. The split between these two sub-payments is a key parameter of this algorithm called the “time-vs-money split rate” and is discussed in more detail below.
    2. The intentions of this structure are (1) to provide a tool for creating parity between time and money investors and (2) to ensure that a large amount of investment of one type does not impact the repayment schedule of investors of the other type.
2. Within each sub-payment, each active rev token recipient will receive a percentage of the rev token sub-payment equal to the total full value of their active rev tokens of that type divided by the total full value of all active rev tokens of that type.

**Time-vs-Money Split Rate**

The time-vs-money split rate (TVMSR) is considered part of the Financial Operations Plan and can be changed from payment to payment according to the needs of the quorum. The goal, however, should be to maintain an average TVMSR of 50/50, meaning that 50% goes to time rev tokens and 50% goes to money rev tokens.

Additionally, the percentage allocated to either type may not drop below 30%. This means that the allowed range of TVMSR values is from 30/70 to 70/30.

**Example Scenario**

The overall rev token payment amount is $10,000 and the TVMSR is 50/50.

Therefore $5,000 will go to time rev tokens and $5,000 will go to money rev tokens.

| Rev Token Recipient | Full Value | Type | % of Sub-Payment | Received $ |
| --- | --- | --- | --- | --- |
| Recipient A | $20,000 | Time | 20K/100K = 20% | $1,000 |
| Recipient B | $80,000 | Time | 80K/100K = 80% | $4,000 |
| Recipient C | $15,000 | Money | 15K/20K = 75% | $3,750 |
| Recipient D | $5,000 | Money | 5K/20K = 25% | $1,250 |

## Guideline 4 - Governance Process

The org investment ledger’s governance process will describe the process for determining annual rev token cohorts, with one created for each calendar year and sub-cohorts created for each investment type and rev token pool.

The process should align with the structure outlined below:

- Annual Process: To run every year, though it does not have to follow the calendar year precisely.
    1. Budgeting: Org & Foundation leaders define the investment budget for the year, which is the total face value, multiple, and total full value of the rev tokens in the year’s annual cohort. (This is the main point at which token downgrading might occur.)
    2. Splitting: A participatory process is used to determine the percentage split of the budget between time investment and money investment. Org & Foundation leaders determine the split between formal money investment and informal money investment.
    3. Allocating: A participatory process is used to allocate time investment rev tokens between ledgers which seek them.
    4. Planning: Each ledger receiving investment creates its design. The designs should ideally involve a quarterly cadence of rev tokens allotments.
    5. Operation: The quarterly processes run throughout the year.
    6. Reporting: Each ledger receiving investment reports on results.
- Quarterly Process: To run roughly every quarter, though the governance process can optionally allow greater flexibility. Describes how re-allocation is administered if rev tokens are unissued or rev points are unawarded.

The above process is built around a structure of regular annual investment rounds, with each round striking a balance between time investment and money investment according to the needs of the quorum and based on the market conditions at that time.

## Guideline 5 - Token Downgrade

Token downgrades should happen no more than once per year and should not happen before year 6.

## Guideline 6 - Failsafe Equity Conversion

As outlined in the [Investment Ledger Implementation Details & Risk](#investment-ledger-implementation-details--risk) section, in the case that the entire rev token and rev points structure is ultimately deemed to be fundamentally infeasible to implement, the org investment ledger’s governance process must include details of a failsafe equity conversion process. 

The failsafe process should result in in converting all issued rev tokens and awarded rev options into shares of traditional equity with overall proportions matching each members’ respective full value holdings of rev tokens and rev options. The equity shares should be in Quorum1 or an affiliated legal entity. All equity shares must be in the same legal entity.

## Guideline 7 - Ledger Liquidation Preferences

In the event of the full liquidation of the org investment ledger for any reason, all token holders must convert at the same discount rate, weighting, or liquidation preference.

