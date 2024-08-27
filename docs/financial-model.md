# Financial Model v2.2.0

This agreement defines how Quorum1 (also referred to as “the quorum”) handles money as a collective, specifically the money in the accounts held by Quorum1. Our goals are to ensure legal compliance, financial solvency, and operational reliability while making financial flows throughout the network as transparent as possible and supporting emergent innovation by directing significant amounts to participatory budget allocation.

---

# Preamble

## Context

This document is formally referred to as the **Quorum1 Financial Model Definition**, or more casually as the **Financial Model**. 

The **Financial Model** is a living document.

The operational implementation of the Financial Model is referred to as the [Financial Operations Plan](./glossary.md#financial-operations-plan). Any details that are not defined in the Financial Model can be defined in the Financial Operations Plan. The Financial Operations Plan is managed more fluidly than the Financial Model itself and is documented separately.

## Key Dependencies

- [Quorum1 Structure](./structure.md) defines structural terms and their relationships including [Org](./structure.md#the-org), [Foundation](./structure.md#the-org), and [Hosted Entities](./structure.md#hosted-entities).
- The [Gov Repo Glossary](./glossary.md) defines many of the special terms referenced in this doc, particularly parts of the [Financial Operations Plan](./glossary.md#financial-operations-plan).

---

# Ledgers

Ledgers are Quorum1’s financial accounts. Ledgers have inflows of money and rev points, can hold money and rev points, and have outflows of money and rev points. Ledgers can also award rev points.

There are a fixed set of [Standard Ledgers](#standard-ledgers) set out in this document, but the full database of ledgers will evolve organically over time, supporting an emergent financial design for the quorum. 

The ledger management infrastructure is maintained by Team Finance, including the management of the working database of all ledgers and the definition of the [Ledger Management Process](./glossary.md#ledger-management-process). Team Finance is also responsible for maintaining permanent audit trails of all ledgers, changes to ledgers, and ledger activity.

## Required Properties of a Ledger

Below are the main properties of a ledger. Collectively, all of a ledger's properties are referred to as the "ledger design".

- **Ledger Manager:** A single contributor or partner member who is responsible for interfacing with Team Finance and assisting with the management and administration of the ledger.
- **Ledger Type:** The available types and their features are defined in this document.
- **Ledger Allocation Model:** Describes the ledger’s outflows.
- **Ledger Status:** “Proposed”, “Active”, or “Retired”
- **Receivable / Non-Receivable:** Only receivable ledgers are able to receive external income directly. Non-receivable ledgers only receive money through cross-ledger outflows.
- **Rev Point Plan:** Describes how rev points from the rev point pool are awarded. Refer to [Rev Point Pools & Plans](#rev-point-pools--plans) for more detail.
- **Ledger Governance Process:** Describes how changes to the ledger’s design are made. When possible ledgers should use a governance change flow defined in the Quorum1 Governance Repo.
- **Investment Ledger Properties:** Additional required properties for investment ledgers are defined in the [Investment Ledger Design](#investment-ledger-design) section.

### Example Ledger Design

```markdown

# Example Widget LOB Reserve Ledger Design

This is only an example of what a ledger design might look like. The actual format is defined by Team Finance.

## Ledger Details

| Property          | Value             |
| ----------------- | ----------------- |
| **Manager**       | Jane Lee (Q0072)  |
| **Type**          | Reserve Ledger    |
| **Status**        | Active            |
| **Receivable**    | Yes               |

## Governance Process

Changes to this ledger design follow the standard Q-Git flow, with additional approval of the ledger manager required.

## Allocation Model

Outflows require the approval of the ledger manager and one additional approver from the following list:
- Jake Long (Q0123)
- Jai Lu (Q0044)
- John Livingston (Q0202)

## Rev Point Plan

None for now.

```

## Allocation Models

A ledger’s allocation model describes the ledger’s outflows, meaning how money flows out of the ledger. The exact format of the allocation model is defined by the [Allocation Model Templates](./glossary.md#allocation-model-templates) and is standardized for each ledger type. All allocation models, however, are essentially lists of outflows. 

Each outflow has a single allocation target and specifies how much money should flow to that allocation target. The types of valid allocation targets are described in detail in the [Outflows](#outflows) section, but at a high level: internal outflows allow ledgers to pass money on to other ledgers or [Workstream Wallets](./glossary.md#workstream-wallets), while external outflows allow ledgers to send money out of the quorum. 

For receivable ledgers, the allocation model must include certain required allocations based on the type of income they receive. The details of this are outlined in the [Standard Income Allocations](#standard-income-allocations) section.

## Rev Point Pools & Plans

Ledgers are able to receive unawarded rev points and hold them in their ledger rev point pool. The points are intended to be awarded to reward and incentivize contributions. Not all ledgers will have rev points in their rev point pool.

There are two ways to award rev points: (1) By designing a rev point plan and (2) by transferring rev points to [Workstream Wallets](./glossary.md#workstream-wallets) via an allocation model outflow. The rest of this sub-section is focused on the former method.

To award rev points directly to members, a ledger must create a rev point plan outlining how the rev points will be awarded. The rev point plan must clearly define the parameters of how rev points are to be awarded including: who is able to participate, the earning cycle, the specific data that will be delivered, how the point earnings are calculated based on the data, what happens when there’s not enough rev points in the pool to cover all of the earnings in an earning cycle, and all other details required to properly administer the program.

It is allowed for a rev point pool to begin accruing rev points without having a rev point plan defined. It is also allowed to change the design of the rev point plan frequently as long as those changes are communicated to all impacted members and they are given a voice in the decision-making process.

Team Finance is responsible for administering the awarding of rev points as outlined in the rev point plan and based on the data provided by the ledger manager. The ledger manager must work with Team Finance to ensure that the ledger design makes sense and is feasible to administer.

Unawarded rev points may be transferred to another rev point pool by the ledger manager. Unawarded rev points may also be subject to reallocation by the source investment ledger if they remain unawarded for a protracted period of time, according to the investment ledger’s rev point plan.

Rev points and their related processes are outlined in more detail in the [Investment](#investment) section.

## Ledger Types

Each ledger type is designed to provide a specific set of features for managing our money. Taken as a whole, the ledger types are intended to serve as modular building blocks able to be linked together by ledger designers to build the infrastructure needed to support different parts of the quorum’s business.

The standardization of these ledger types is critical for streamlining our financial and technical operations. The modularity of these ledger types is critical for allowing the flexibility we need to grow, evolve, and adapt.

### Pass-Through Ledgers

Pass-through ledgers simply allocate all inflows directly to a list of allocation targets, with a specific percentage flowing to each target.

Pass-through ledgers may optionally also include a set of fixed dollar amount outflows which are taken “off the top” before the rest of the inflowing money is allocated based on percentages.

### Fulfillment Ledgers

Fulfillment ledgers (potentially also called “project fulfillment ledgers” or just “project ledgers”) hold money intended to compensate the fulfillment of a particular project or client engagement. They are necessarily a bit more complex than other ledger types. Fulfillment ledgers are used for all consulting engagements, for internal Quorum1 projects, product development work, and anything else where outflows are linked to work fulfillment. 

Fulfillment ledgers keep track of how much revenue has been fulfilled and produce outflows based only on fulfilled revenue. Fulfillment ledgers also support a refund mechanism for returning the remaining balance to its source if a project is canceled before all of the revenue has been fulfilled.

There are two types of fulfillment ledgers:

- **Hourly** fulfillment ledgers are fulfilled by line item hours being tracked and verified in the [Time Tracking System](./glossary.md#time-tracking-system).
- **Percentage** fulfillment ledgers are fulfilled based on verified completion percentages for each line item. These can also be used to implement recurring payments in fixed amounts.

The allocation model of a fulfillment ledger is also referred to as a “project cost model”. The project cost model defines two lists of allocation targets: 

- The **line item allocations** produce the fulfilled revenue. Each line item includes a bill rate and a cost rate. The bill rate yields the amount of revenue fulfilled. The cost rate, which must be equal to or lower than the bill rate, yields the amount received by the allocation target. The difference between the bill rate and cost rate yields the margin.
- The **margin allocations** each receive a fixed percentage of the fulfilled revenue. Note: The project cost model must be designed so that the smallest line item margin percentage is equal to or greater than the sum of all margin allocation percentages, to prevent cost overruns.

### Expense Ledgers

Expense ledgers hold money intended to pay for vendor expenses. Expense ledgers may have one or more virtual or physical debit cards linked to them, according to the [Debit Card Management Process](./glossary.md#debit-card-management-process).

Expense ledgers may only be used to pay for the following types of outflows:

- One-time payments to registered vendors, requiring a corresponding invoice
- Recurring payments to registered vendors, via the [Recurring Expense Management Process](./glossary.md#recurring-expense-management-process)
- Reimbursement requests from members, via the [Expense Reimbursement Process](./glossary.md#expense-reimbursement-process)

The ledger manager is expected to maintain a viable level for the expense ledger to ensure a reasonable runway to cover recurring expenses. Team Finance is responsible for providing ledger managers with the tools and visibility needed to manage the levels in the ledger. Overdrafts or shortfalls in an expense ledger may result in Team Finance retiring the ledger or requiring a different ledger manager.

### Reserve Ledgers

Reserve ledgers hold money in reserve to provide financial security and help us manage risk. Reserve ledgers do not have any pre-defined outflows. Instead, each transfer of money out of a reserve ledger must be approved according to an approval process defined in the allocation model for the reserve ledger.

### Collaborative Ledgers

Collaborative ledgers hold money intended to be assigned to projects and initiatives as determined through collaborative processes open to the participation of some or all quorum members.

The allocation model of a collaborative ledger defines the specific set of quorum members who should be included in the collaborative process and any guidelines or limitations that the collaborative process itself must meet, as well as how often the process should be run.

Before the running of a collaborative funding process, the process itself must be clearly defined. An appropriate audit trail must also be recorded as part of the collaborative funding process log.

### Bonus Ledgers

Bonus ledgers hold money used to award bonuses for certain activities which are part of a well-defined incentivization program. This includes sales & marketing commissions, client referral fees, new member recruiting bonuses, and other similar programs. 

Note that, like all ledgers, bonus ledgers may only direct outflows to valid ledger outflows & allocation targets. This means that community members are not able to receive bonus payouts directly.

Team Finance is responsible for administering the calculation and disbursement of bonuses based on data provided by the ledger manager. The ledger manager must work with Team Finance to ensure that the bonus ledger design makes sense and is feasible to administer.

The allocation model of a bonus ledger must clearly define the parameters of the incentivization program including: who is able to participate, the earning cycle, the specific data that will be delivered, how the bonuses are calculated based on the data, what happens when there’s not enough money in the ledger to cover all of the bonuses in an earning cycle, and all other details required to properly administer the program.

It is allowed for a bonus ledger to begin accruing money without having an incentivization program defined. It is also allowed to change the design of the incentivization program frequently as long as those changes are communicated to all impacted members and they are given a voice in the decision-making process.

### Investment Ledgers

An investment ledger is a special type of ledger which can receive investment inflows, create rev tokens, create rev points, and share revenue passed from other ledgers back with active rev token recipients and rev point holders.

For more information on investment ledgers refer to the [Investment Ledger Design](#investment-ledger-design) section. The full details on the quorum’s investment mechanisms are outlined in the [Investment](#investment) section.

## Standard Ledgers

This section lists the set of standard ledgers that are mandatory and exist to serve key functions for operating and supporting Quorum1 holistically. These ledgers must always exist and are administered directly by Team Finance and managed either by the Managing Partners or by a foundation team appointed by Managing Partners. The ledger manager of each standard ledger is appointed by the team responsible for managing the ledger.

The allocation models of each standard ledger are part of the Financial Operations Plan.

### Core Ledger

The core ledger is a pass-through ledger. The core ledger is used to pay for Quorum1’s operating expenses and core programs. All Quorum1 income must allocate a certain percentage to the core ledger, based on the type of income. 

The core ledger must allocate a percentage to each of the other standard ledgers listed in this section. The core ledger may not directly allocate to any non-standard ledgers. The precise allocation percentages are defined by the core ledger allocation model.

### Org Expense Ledger

The org expense ledger is an expense ledger used to pay for all core vendor expenses. This includes things like operating costs, insurance, business systems, service providers, taxes, and fees. Over time many non-standard expense ledgers will exist and are by definition allowed to manage vendor expenses on their own. However, ledger managers of non-standard expense ledgers are encouraged (but not required) to allocate particular vendor expenses to the standard org expense ledger instead when it makes sense to do so (such as in order to negotiate a lower cost).

### Org Reserve Ledger

The org reserve ledger is Quorum1’s primary reserve ledger. This ledger can be used to pay for unexpected expenses or anything related to supporting the continued operation of the quorum. However, this ledger’s balance should be kept at a sufficient level at all times.

Ideally this ledger should target a balance sufficient to cover 2 to 3 months of foundation operations and org expenses. If the ledger’s balance exceeds 12 months of foundation operations and org expenses, then the quorum should consider re-allocating some of the reserve to other uses.

### Foundation Operations Ledger

The foundation operations ledger is a pass-through ledger intended to pay for everything required to keep the Foundation Team running and to provide operating capital for ongoing maintenance and investment in continued innovation of the quorum platform. This ledger should be used to pay for Foundation Team salaries and contracts, and to allocate money to [Workstream Wallets](./glossary.md#workstream-wallets) to support maintenance and innovation of the systems managed by the Foundation Team. This ledger may also be used to fund any other efforts that are related to the support, maintenance, improvement, promotion, and improvement of Quorum1.

### Org Investment Ledger

The org investment ledger is our primary investment ledger and is maintained by Quorum1 for the org as a whole. Rev tokens in the org investment ledger are exchanged with investors of both time and money. Prioritization, allocation, and other decision-making processes around the org investment ledger must always be participatory and democratic in accordance with Quorum1’s established best practices as they evolve.

This ledger and the linked rev tokens and rev points are a critical part of Quorum1’s financial infrastructure. More details are outlined in the [Investment](#investment) section.

The org investment ledger design is maintained in the Quorum1 governance repo, alongside the Financial Model and many other docs. For more information refer to: [Org Investment Ledger Design](./glossary.md#org-investment-ledger-design).

In the event of the full liquidation of the org investment ledger for any reason, all token holders must convert at the same discount rate, weighting, or liquidation preference.

### Org Bonus Ledger

The org bonus ledger is a bonus ledger intended to fund Quorum1’s org incentivization program.  Quorum1’s org incentivization program should focus primarily on rewarding the sales, biz dev, marketing, and demand generation work needed to drive new paid project work. But the program may also reward efforts on critical initiatives that impact the entire quorum.

### Org Collaborative Ledger

The org collaborative ledger is a collaborative ledger intended to fund internal Quorum1 projects and new product development projects that are selected via periodic participatory budgeting processes involving all community, contributor, and partner members.

---

# Inflows

Inflows are money or rev points that flow into a ledger.

There are technically two types of inflows: internal inflows (from other ledgers) and external inflows (aka income). However, since internal inflows are very simple, the bulk of this section is dedicated to discussing income.

## Internal Inflows

Internal inflows are money that flows into a ledger from another ledger, through a cross-ledger outflow. These are described in more detail in the [Cross-Ledger Outflows](#cross-ledger-outflows) section.

## Income (External Inflows)

External inflows are our income. Income is money that flows into Quorum1 from external sources. Each incoming payment is associated with a specific receivable ledger and the money flows according to the ledger’s allocation model.

Income may only flow into ledgers which are designated as being “receivable”. In order to be receivable, a ledger must comply with the [Receivable Ledger Requirements](./glossary.md#receivable-ledger-requirements). For example, a receivable fulfillment ledger for a client project may require a signed SOW.

### Income Types

The income type impacts many different things, including which types of ledgers may be targeted, the standard income allocations, and the required documentation checklist used during income reconciliation. 

All income must be categorized as a single income type. Payments which contain multiple types of income are split during the bookkeeping process so they can be processed separately.

- **Service** income comes from professional services work performed for clients.
- **Product** income comes from fees charged for physical or virtual products, including “Software-as-a-Service” fees and other product subscription fees. For now we are far more likely to sell software products rather than hardware products.
- **Investment** income (which is not considered “income” in the traditional sense, but which is an external inflow and thus “income” as defined in this document) comes from purchases of rev tokens as outlined in the [Investment](#investment)  section.
- **Marketplace** income comes from money loaded into a quorum-operated marketplace. This income type is still experimental and, for now, will only come from payments between [Workstream Wallets](./glossary.md#workstream-wallets). Revenue may not be recognized until the money loaded into a wallet is actually transacted via the workstream.
- **Other Income** which does not fit the above categories is processed and allocated ad hoc by Team Finance.

### Standard Income Allocations

All receivable ledgers must include the following standard income allocations, as relevant:

1. All income must allocate a required percentage to the **core ledger.** The required percentage is defined by the [Standard Income Allocation Table](./glossary.md#standard-income-allocation-table), part of the Financial Operations Plan.
2. Income linked to a hosted entity must allocate a required percentage to its corresponding **hosted entity ledger**. The required percentage is defined by the hosted entity in accordance to its governance process.

**Standard Income Allocation Table Format and Default Values:**

The [Standard Income Allocation Table](./glossary.md#standard-income-allocation-table) is part of the Financial Operations Plan, not the Financial Model and may be changed without updating this doc. 

The standard income allocation table defines the required percentage of recognized income that must be allocated to the core ledger for each type of income based on various parameters, including whether the income is associated with a hosted entity and whether it uses the Quorum1 brand. 

The standard income allocation table should match the basic format outlined here. The actual values may differ, however. And the actual format may also differ slightly as long as it aligns with the spirit of this design.

In the interim period before an official standard income allocation table is finalized, the values in the table below will serve as defaults.

| Income Type | Hosted Entity? | Brand Type | Core Ledger % |
| --- | --- | --- | --- |
| Service | No | Q1-Branded | 20% / 15% ¹ |
|  | Yes | Q1-Branded | 15% |
|  | Yes | Alt-Branded | 10% |
| Product | No | Q1-Branded | 50% |
|  | Yes | Q1-Branded | 40% |
|  | Yes | Alt-Branded | 30% |
| Investment | No | Q1-Branded | 0% |
|  | Yes | Q1-Branded | 0% |
|  | Yes | Alt-Branded | 5% |
| Marketplace | N/A ² | N/A ² | 2% |

¹ Projects operated under the Quorum1 brand and not associated with a hosted entity have a default core ledger allocation of 20%. But when led by partner members, they may optionally allocation a lower amount, as low as 15%.

² Marketplace income is experimental for now and only pertains to transaction fees related to [Workstream Wallets](./glossary.md#workstream-wallets).

### Available Ledger Types by Income Type

Each type of income may only be received by certain types of receivable ledgers.

| Income Type | Core Ledger? | Hosted Entity Ledger? | Generic Pass-Through Ledger? | Project Fulfillment Ledger? | Investment Ledger? |
| --- | --- | --- | --- | --- | --- |
| Membership | ✅ | ✅ | ❌ | ❌ | ❌ |
| Service | ❌ | ❌ | ❌ | ✅ | ❌ |
| Product | ❌ | ✅ | ✅ | ❌ | ❌ |
| Investment | ❌ | ❌ | ❌ | ❌ | ✅ |
| Marketplace | ✅ | ✅ | ✅ | ❌ | ❌ |

### Income Reconciliation

Team Finance is responsible for reconciling each incoming payment. Only after a payment is reconciled does it become income. Any payments which cannot be reconciled may need to be refunded or held in escrow until they can be reconciled.

The income reconciliation process involves matching an incoming payment with a specific ledger and verifying that the required documentation is complete. The [Required Income Documentation Checklist](./glossary.md#required-income-documentation-checklist) is part of the Financial Operations Plan.

### Fulfillment, Recognition, & Refunds

Most quorum income is recognized as revenue immediately upon receipt. But receivable fulfillment ledgers are unique in that they do not recognize revenue until it is fulfilled as defined by the ledger’s project cost model. (More details on this ledger type: [Fulfillment Ledgers](#fulfillment-ledgers))

Unfulfilled (and therefore unrecognized) revenue in a fulfillment ledger may be refunded in accordance to the [Refund Process](./glossary.md#refund-process).

---

# Outflows

Outflows are money or rev points that flow out of a ledger as defined by the ledger’s allocation model. Each outflow has a single allocation target (where the money goes to).

There are two basic types of outflows: internal outflows and external outflows.

## Internal Outflows

Internal outflows are money that flows to allocation targets which are inside of the quorum.

### Cross-Ledger Outflows

Cross-ledger outflows are money or rev points that flow from one ledger to another ledger. Any ledger is able to be an allocation target of any other ledger.

Cross-ledger outflows may optionally include usage requests that specify how the money or rev points should be used (such as paying for a specific expense). These usage requests are not strictly binding but the ledger managers should make a good faith effort to respect them.

### Workstream Wallet Outflows

Workstream wallet outflows allow ledgers to move money or rev points into specific [Workstream Wallets](./glossary.md#workstream-wallets). This in turn enables more agile work structures and gives the wallet managers the ability to source help from the full quorum membership.

## External Outflows

External outflows are money that flows to allocation targets which are outside of the quorum.

### Member Outflows

Contributor and partner members are valid allocation targets based on their eligibility according to the [Member Payment Eligibility Process](./glossary.md#member-payment-eligibility-process). If members have joined the quorum via a corporate entity, then their payments are directed to their registered corporate entity.

### Vendor Company Outflows

Vendor company outflows send money to vendors that have been registered according to the [Vendor Registration Process](./glossary.md#vendor-registration-process). These types of outflows may be subject to additional requirements, such as needing copies of invoices or receipts.

### Rev Token Outflows

Rev token outflows are only available to investment ledgers. These outflows send money to the ledger’s active rev token recipients. This process is outline in the [Investment](#investment) section. 

---

# Investment

We believe that Quorum1 has the potential to generate tremendous wealth over the coming years. If achieved, it is critical to our mission that this wealth be both re-invested in nurturing future success *and* shared equitably with the individuals and organizations that helped build the wealth engine. This is our dual investment mission: To balance our support of future innovation with our returns to our ever-growing community of investors.

The former goal of re-investment is achieved via the [Org Collaborative Ledger](#org-collaborative-ledger), and the other [Collaborative Ledgers](#collaborative-ledgers) which will emerge over time, as well as through the emergent properties intrinsic to our unique organizing model.

The latter goal of equitably sharing wealth with our investors—of both time and money—is addressed in this section.

In creating our design for a Quorum1 investment mechanism, we require that it be aligned with our goals, mission, and values. We also require that our investment mechanism function within the logistical and operational environment of our emergent org structure.

## Investment Model Orientation

### Investment Model Key Concept Overview

These concepts are outlined in greater detail in later sections, but below is a brief summary of some of the key concepts which make up our investment model.

- **Investment Ledger:** Special type of ledger which can receive investment inflows, create rev tokens and rev points, and share revenue passed from other ledgers back with active rev token recipients and rev point holders.
- **Types of Investment:**
    - **Time Investment:** The contribution of work, effort, or support to the quorum.
    - **Formal Money Investment:** Money invested in an investment round via formal investment
    - **Informal Money Investment:** Ad-hoc investments in an investment round that are managed more fluidly
- **Rev Token Concepts:**
    - **Rev Token:** An owned asset which entitles the owner to receive rev token payments. Each rev token is linked to an investment ledger. Each rev token has a face value, a multiple, and a full value equal to the face value times the multiple.
    - **Rev Token Payments:** Revenue share income flows into an investment ledger and is passed through to active rev token recipients via regular rev token payments.
    - **Rev Token Cohort:** Groups of rev tokens within an investment ledger. There are two types: *Issuing* cohorts issue rev tokens and can be nested inside of *grouping* cohorts.
- **Time Investment Concepts:**
    - **Time Investment Pool:** For investment ledgers only. A pool of issued rev tokens held by Quorum1 with the received payments powering the ledger’s rev point program.
    - **Rev Point:** A reward mechanism for time investors which allows members to benefit financially in the future success of the quorum without the legal and tax implications of owning an asset.
    - **Rev Point Payments:** Rev token payments received by the rev tokens held in the ledger’s time investment pool are passed through to rev point holders via regular rev point payments.
    - **Rev Point Pool:** Each ledger (including non-investment ledgers) has a rev point pool which can hold unawarded rev points which are awarded to members who make contributions according to the ledger’s rev point plan.

### How Investment Ledgers Work

All investment in the quorum is managed through investment ledgers (one of our [Ledger Types](#ledger-types)). An investment ledger is a special type of ledger which can receive investment inflows, create rev tokens and rev points, and share revenue passed from other ledgers back with active rev token recipients and rev point holders.

The [Org Investment Ledger](#org-investment-ledger) is our standard investment ledger and must maintain ongoing continuity, but other investment ledgers may be created and changed over time according to the [Investment Ledger Management Process](./glossary.md#investment-ledger-management-process). Investment ledgers are necessarily complex, involving special legal contracts and, in some cases, custom technology to facilitate their ongoing operations. Each investment ledger may also present unique regulatory and compliance challenges. This means that rev share ledgers require the support and alignment of Team Finance, Team Legal, Team Ops, Team Build, and the Managing Partners.

The org investment ledger may be used to reward and incentivize investment in any part of Quorum1 or in areas deemed important by the quorum. Other investment ledgers will have their own design, limitations, and participation, defined by the members and leaders of each ledger.

#### Investment Ledger Inflows & Outflows

Investment ledgers have the following inflows:

- **Investment inflows¹** flows in from money investors and is exchanged for rev tokens. The received cash is held in the ledger and available for investment outflows.
- **Rev share inflows** flow in from other ledgers and are used to pay back investors. The received cash automatically flows to rev token payments and rev point payments.

Investment ledgers have the following outflows:

- **Investment outflows** allocate investment inflows to target ledgers, with each outflow approved according to the ledger’s allocation model.
- **Rev token payments²** allocate rev share inflows to rev token recipients according to the [Investment Ledger Payment Algorithm](#investment-ledger-payment-algorithm).
- **Rev point payments³** allocate the rev token payments from the time investment pool to rev point holders according to the [Investment Ledger Payment Algorithm](#investment-ledger-payment-algorithm).

***¹ Investment inflows:** Each investor must be onboarded as defined by the [Investor Management Process](./glossary.md#investor-management-process). Formal money investment is associated with an investment round, informal money investment is not associated with an investment round.*

***² Rev token payments:** Rev share inflows are passed through to the active rev token recipients as outlined in the [Rev Token Payments](#rev-token-payments) section.*

*³ **Rev token payments:** Time investment pool rev token payments are passed through to the rev point holders as outlined in the [Rev Point Payments](#rev-point-payments) section.*

### Investment Ledger Implementation Details & Risk

At the time of writing and approving this version of the Financial Model, some of the technical, operational, legal, and financial implementation details around rev tokens and rev points have not been finalized. This means that key details around contract structure, legal design, tax treatment, and ongoing operations are still being developed. This further means that there is some amount of risk that parts of this design will not be able to be implemented as intended. 

In order for us to fund and incentivize this development work (and to formally recognize the years of work already put into the quorum), however, it is necessary for Quorum1 to begin issuing rev tokens and awarding rev points before the development work is complete. We acknowledge that this approach creates the risk that these initial rev tokens and rev points will need to be modified in the future once the implementation details have been finalized. 

We believe, however, that the implementation of this model will ultimately succeed and that whatever further Financial Model iteration is required will produce minimal changes to the structure of the initial rev tokens and rev points. We further believe that it would be difficult or impossible to implement a model as novel as the rev token and rev point structure without an immediately real world use case.

It is important to note, though, that in the most severe case it is possible that the entire rev token and rev points structure may prove fundamentally infeasible. For that reason, every investment ledger created before the finalization of the implementation details should include a “failsafe equity conversion” governance process. This process outlines the steps to be followed only in the case that rev token and rev point structures are considered to be fundamentally infeasible to implement.

This is outlined in more detail in this section: [Failsafe Equity Conversion Governance](#failsafe-equity-conversion-governance).

## Investment Types

We recognize two broad categories of investment: the **investment of time** through contributions to quorum-related work and the **investment of money**. We recognize that both types of investment are critical to the quorum’s long-term success and they must be recognized and incentivized using the same core mechanism. For us that mechanism is the rev token system outlined later in this section.

We also recognize that the legal, tax, and compliance implications are different for time investors and money investors. This means that there must be some inevitable differences in the way the mechanisms are implemented for these two different investor types. Our solution is rev points, which are a non-asset-based member benefit awarded to time investors and ultimately funded by the same rev tokens issued to money investors.

A balance must be struck between the incentivizing of time investment and money investment. Our investment model aspires to provide tools for this balance to be clearly defined while also allowing it to change as the quorum’s needs evolve.

Managing the investment outflows equitably will require careful prioritization, but the prioritization must always align with the principle that time and money (work and capital) are both important and are equally worthy of remuneration.

### Time Investment

Time investment is a general term to describe the contribution of work, effort, or support to the quorum. Time investment can be made by Quorum1 members or by collaborating organizations.

Rev points are awarded to time investors. In general the number of rev points awarded should be equal to the face value of the time investment multiplied by the rev token cohort’s multiple, but this math may differ when needed.

We recognize that, when rev points are awarded for time investment, the face value of the investment may be challenging or, in some cases, impossible to determine precisely. And even in cases where the value is able to be determined, due to budget limitations it may not always be possible to fully recompense the true value. This is acceptable as long as the broader allocation of rev points is equitable.

In general, the valuation of time investments should follow these key principles:

- **Time Valuation Principle 1:** The fair market value (FMV) of either the impact of the effort or of the time itself should be the primary guide when establishing a valuation. The FMV of the impact is preferred over the FMV of the time, though both are acceptable. And other methods are acceptable when they are more appropriate than valuing impact or time.
- **Time Valuation Principle 2:** Establishing the value of a time investment prior to the investment being made (preceding valuation) is strongly preferred to retroactive valuation, when possible.

It’s worth noting that it’s not always possible to comply with time valuation principle 2 (preceding valuation). This is evidenced within this doc by the retroactive valuation of the time investments made prior to the establishing of the current version of the Financial Model. Retroactive valuation is acceptable as long as it is done equitably, but it should be avoided whenever possible to do so without making overall allocation less equitable.

> \[!IMPORTANT]
> **Rev points are intended to be a form of supplementary or bonus income (analogous to stock options in a startup), not the primary form of compensation.** The primary form of compensation for time investors should be cash. In cash-lean periods it may be necessary for rev points to largely (or fully) take the place of cash compensation, but the practice should be avoided when possible.

### Money Investment

Money investment in Quorum1 is the process of issuing rev tokens to investors in exchange for money. Each investor must be onboarded as defined by the [Investor Management Process](./glossary.md#investor-management-process). The face value of money investment rev tokens is always equal to the amount paid by the investor.

All money investment is associated with a specific investment round.

Money investment takes two forms:

- **Formal investment** is money investment associated with a signed investment contract and subject to traditional diligence processes.
- **Informal investment** is ad-hoc money investment which is managed more fluidly and does not involve formal diligence processes. Informal investment is restricted to partner members or highly trusted contributor members who meet the criteria established by Team Finance and Team Legal. Informal investment can be used for “cash calls” to cover expenses or other purposes.

## Investment Ledger Design

This section describes the design of an investment ledger, describing the interpretation of required ledger properties and highlighting additional required properties specific to this ledger type.

### Meaning of Common Ledger Properties for Investment Ledgers

Below are the [Required Properties of a Ledger](#required-properties-of-a-ledger) and how each differs for an investment ledger.

- **Ledger Manager:** No differences.
- **Ledger Type:** No differences.
- **Ledger Allocation Model:** The allocation model of an investment ledger functions similarly to that of a reserve ledger.
    - Investment ledgers have automatic rev token & rev pool payment outflows, but they do not have any pre-defined investment outflows.
    - Instead, each transfer of cash out of an investment ledger must be approved according to an approval process defined in the allocation model. 
    - Note: The allocation model of an investment ledger only defines how outflows from the cash holdings are approved, it *does not* define how rev share inflows are allocated--that is defined by the [Investment Ledger Payment Algorithm](#investment-ledger-payment-algorithm).
- **Ledger Status:**
    - Only "Active" investment ledgers can receive investment inflows.
    - Both "Active" and "Retired" ledgers generate rev token payments and rev point payments.
    - Before being "Retired" any remaining cash must be transferred out of the investment ledger.
- **Receivable / Non-Receivable:** Investment ledgers are always receivable.
- **Rev Point Plan:** Rather than having a single rev point plan, an investment ledger has a separate rev point plan for each investment round.
- **Ledger Governance Process:** Is recommended to include specific guidance on the following.
    - **Token Downgrade Guidelines:** Describes any restrictions on when a token downgrade can be executed and any additions to the change management processes when token downgrades are being added to the investment ledger design. (More detail: [Token Downgrade Governance](#token-downgrade-governance))
    - **Failsafe Equity Conversion Guidelines:** Describes the process through which investors are issued traditional equity in the unlikely eventuality that the rev token structure is deemed fundamentally infeasible to fully implement. (More detail: [Failsafe Equity Conversion Governance](#failsafe-equity-conversion-governance))

### Additional Required Properties for Investment Ledgers

These properties must also be specified in the investment ledger design.

- **Core Parameters:** Every investment ledger has a set of core parameters which impose limits on its operations. Changes to these parameters have their own part of the ledger’s governance process.
    - **Ledger Budget:** The upper limits for (1) the total full value and (2) the total face value of all outstanding rev tokens in the ledger, including unissued rev tokens. Once either of these limits are reached, no new rev tokens can be created.
    - **Min Multiple:** The lower limit for the multiple property of all rev tokens in the ledger. During a token downgrade, no token multiples will be decreased below this limit.
    - **Max Multiple Downgrade:** A percentage between 0% and 100% used during a token downgrade to prevent the multiple of any rev token from decreasing more than this amount from its originally issued multiple.

- **Rev Token Cohorts:** Each rev token in an investment ledger belongs to an issuing rev token cohort. Each issuing rev token cohort takes a chunk of the ledger budget and turns it into rev tokens. Issuing rev token cohorts may be nested within parent grouping cohorts in order to formally track important groupings of rev tokens.
    - **Cohort Id:** A unique machine-parsable identifier to use for this cohort. Must be unique across all cohorts in this investment ledger.
    - **Cohort Name:** A unique human-readable name to use for this cohort. Must be unique across all cohorts in this investment ledger.
    - **Cohort Type:** The type can be one of the following values.
        - "Grouping" cohorts are only for grouping. They only contain other cohorts and can be nested to an arbitrary depth.
        - "Time" cohorts are for issuing time rev tokens. They cannot contain other cohorts and can issue only time rev tokens.
        - "Money" cohorts are for issuing money rev tokens. They cannot contain other cohorts and can issue only money rev tokens.
    - **Cohort Status:** The status can be one of the following values.
        - "Planned" cohorts have not yet had any rev tokens issued from them and are subject to change.
        - "Active" cohorts are actively being issued or subscribed and are less likely to change, though they are still subject to change.
        - "Closed" cohorts have been fully subscribed.
    - Required for issuing cohorts, optional for grouping cohorts:
        - **Multiple:** Specifies the multiple of all rev tokens in the cohort.
        - **Face Value:** The total face value of all rev tokens in the cohort.
        - **Full Value:** The total full value of all rev tokens in the cohort.

- **Investment Rounds:** A list of investment rounds, including for each:
    - **Round Organizers:** A list of at least two partners who serve as the approvers for the round's design and the overall managers of the round. The organizers must come to full consensus in their decisions unless otherwise specified.
    - **Included Cohorts:** Which rev token cohorts are available for sale in the round.
    - **Informal Investment Guidelines:** If applicable, any guidelines around how informal investments should be managed and approved. By default, the round organizers are responsible for approving informal investments.
    - **Rev Point Plan:** Defines how the rev points are to be allocated, in alignment with the [Rev Point Pools & Plans](#rev-point-pools--plans) section.

- **Payment Algorithm Parameters:** Defines the math used to calculate rev token & rev point payments from rev share inflows. This is described in detail in the next subsection ([Investment Ledger Payment Algorithm](#investment-ledger-payment-algorithm)). The investment ledger design must include the following required parameter definitions:
    - **TVMSR Guidelines:** Guidelines around the TVMSR value.
    - **Rev Token Payment Weighting:** How the money rev token sub-payment is split across the active money rev token recipients.
    - **Rev Point Payment Weighting:** How the time rev token sub-payment is split across rev point holders.

- **Token Downgrades:** Contains a list of token downgrades if applicable, or language indicating that this investment ledger has not had any token downgrades. Token downgrades should be formally approved through the process of adding them to this list, though the actual process is defined in the [Token Downgrade Governance](#token-downgrade-governance). Each downgrade in the list must include the date, downgrade factor, and the sum total of full value across all rev token cohorts before and after the downgrade.

### Investment Ledger Payment Algorithm

This section defines the standard investment ledger payment algorithm that is used to calculate rev token payments and rev point payments based on rev share inflows into an investment ledger. This section also defines the key parameters that must be provided by the investment ledger design.

The rev token payments are processed in alignment with the following algorithm / process:

1. Before processing a round of rev token and rev point payments, the [TVMSR](#time-vs-money-split-rate) is defined in alignment with the **TVMSR Guidelines**. It is recommended is that the ledger manager determines the TVMSR and that they seek input from all relevant stakeholders, but the ledger design may define different guidelines.
2. The overall rev token payment is then split, based on the TVMSR, into two sub-payments: one for time rev tokens and another for money rev tokens.
3. Within each sub-payment, a list of member payments is generated:
    1. The time rev token sub-payment is split across rev point holders based on the **Rev Point Payment Weighting**. Note that since all time rev tokens are held by Quorum1 on behalf of the members, the recipient for all time rev tokens is technically the same: Quorum1.
    2. The money rev token sub-payment is split across all active money rev token recipients based on the **Rev Token Payment Weighting**.
4. The payments are then executed to the rev point holders and rev token recipients as outlined in the prior step.

This algorithm requires the following key parameters, defined in the investment ledger design:
- **TVMSR Guidelines:** Provides guidance around step 1 above.
- **Rev Point Payment Weighting:** Implements step 3A above. More details in [Rev Point Payments](#rev-point-payments) section.
- **Rev Token Payment Weighting:** Implements step 3B above. More details in [Rev Token Payments](#rev-token-payments) section.

#### Time-vs-Money Split Rate

The time-vs-money split rate (TVMSR) for an investment ledger may change from payment to payment as needed. The updates must comply with the time-vs-money split rate guidelines defined in the investment ledger design.

The TVMSR process exists to (1) provide a tool for creating parity between time and money investors and (2) ensure that a large amount of investment of one type does not impact the repayment schedule of investors of the other type.

When communicating the value of a TVMSR the following format is used: `X/Y`, where:
- `X` is the % going to time rev tokens
- `Y` is the % going to money rev tokens
- `X + Y` is equal to 100

For example: A TVMSR of 60/40 means that 60% goes to time rev tokens and 40% goes to money rev tokens.

### Investment Ledger Governance Notes

This section outlines provides guidance towards governance processes which are unique to investment ledgers and should be included in their designs.

#### Token Downgrade Governance

> \[!WARNING]
> Token downgrades are disruptive. They should be used rarely and must be used in good faith and with full transparency.

It may become necessary to decrease the return multiple of all outstanding rev tokens in a ledger. This process is called a [Rev Token Downgrade](#rev-token-downgrades). For example: A token downgrade might be needed when the revenue growth of the ledger inflows has proven to be too slow to reach the ledger budget, or when more room for investment is needed without raising the ledger budget.

A token downgrade involves selecting a downgrade factor (a decimal number between zero and one) and changing the multiple property of **all outstanding rev tokens** by multiplying their originally issued multiple by that downgrade factor. During this process the min multiple and max multiple downgrade core parameters must be respected, meaning that all rev tokens may not end up decreasing by the exact same factor.

As part of a token downgrade governance sub-section, the ledger governance process should describe:
- **Restrictions:** Whether there are any restrictions on when a token downgrade can be executed.
- **Process:** The process through which a rev token downgrade is executed (documented and approved). Recommendations:
    - The process should ideally consist of adding the token downgrade to the list of token downgrades in the investment ledger design.
    - The investment ledger design should ideally be stored as a doc in a repo governed by a change flow defined in the Quorum1 Governance Repo.
    - The process should ideally also highlight the fact that all impacted numbers in the investment ledger design must be updated with the new post-downgrade values.
- **Special Review Requirements:** Any additional requirements associated with the review process, beyond those required when other parts of the investment ledger design are changed. Specific recommendation: A longer time available for review.

##### Rev Token Downgrade Example

1. Let's say that a token downgrade applies a `0.6` downgrade factor to an investment ledger. This is the only token downgrade to this investment leger to date.
2. Let's assume that before the downgrade a particular rev token (Rev Token A) had $10K face value, 40x multiple, and $400K full value
3. After the downgrade Rev Token A would have a $10K face value, 24x multiple, and $240K full value. 
4. Let's further assume that in the core parameters of the investment ledger the max multiple downgrade is 90% and the min multiple is 1x.
5. That would mean that no token downgrade or series of token downgrades could result in the multiple of Rev Token A decreasing below 4x (which is a 90% decrease of 40x). In this case the min multiple would not come into play since it is lower than 4x.
6. Now let's assume that before the downgrade another rev token (Rev Token B) had $10K face value, 7x multiple, and $70K full value.
7. That would mean that no token downgrade or series of token downgrades could result in the multiple of Rev Token B decreasing below 1x. In this case the min multiple would apply instead of the max multiple downgrade since it is higher.

##### Token Upgrades Disallowed

**Token upgrades** (increasing the multiples of all outstanding rev tokens in a ledger) **are specifically disallowed**.

The rationale is that constraining multiples to a single direction of movement:
1. Makes it easier for investors to predict how rev token values might change.
2. Encourages more accurate initial valuation of effort at the outset.

This restriction is further justified by the fact that new rev tokens may easily be issued to recognize an increased valuation of past efforts, without requiring the disruption of modifying all multiples.

#### Failsafe Equity Conversion Governance

> \[!NOTE]
> At this point, significant work has been done to validate the rev token & rev point structure. Executing a failsafe equity conversion is highly unlikely. But it's still an important backup process to have available.

As outlined in the [Investment Ledger Implementation Details & Risk](#investment-ledger-implementation-details--risk) section, in the unlikely event that the entire rev token and rev points structure is ultimately deemed to be fundamentally infeasible to implement, each investment ledger created before the finalization of all implementation details should include a governance process outlining a “failsafe equity conversion” process.

This process should outline steps that will result in issuing traditional equity in Quorum1 or an affiliated legal entity, proportionally based on rev tokens and rev points.

### Example Investment Ledger Design

Investment ledger designs can be quite long and complex.

For an example to use as a starting point, refer to the [Org Investment Ledger Design](./glossary.md#org-investment-ledger-design).

## Rev Tokens

Rev tokens are a type of debt instrument linked to a particular investment ledger, similar to a corporate bond with a fixed return multiple but a variable payback rate (and therefore a variable interest rate) and the additional risk of the multiple being downgraded in the future. 

Rev tokens are an owned asset entitling the owner to a portion of the rev share inflows of the linked investment ledger until the total payments received reach a certain value. Quorum1 facilitates investment by issuing rev tokens to our investors. 

For money investors, rev tokens are issued in exchange for money. For time investors, rev tokens are instead issued to and held by Quorum1 and used to power a [Rev Points](#rev-points) program.

Rev tokens may be owned by individuals or by other legal entities.

### Rev Token Properties

Below are some of the most important properties of a rev token.

- **Face Value:** The value of the money or time exchanged for the token at time of issuance.
- **Multiple:** The factor applied to the face value to calculate the full value.
- **Full Value:** Equal to the face value times the multiple.
- **Received Value:** The sum total of all payments received by the token to date.
- **Remaining Value:** The amount remaining to be received. Equal to the full value minus the received value.
- **Type:** There are two types of rev tokens, corresponding to the two [Investment Types](#investment-types): money rev tokens and time rev tokens.
- **Cliff:** The period of time, post-issuance, before the token begins receiving payments.
- **Status:** Where the token is at in its lifecycle (Unissued, Inactive, Active, Retired).
- **Owner:** The individual or entity which owns the token.
- **Recipient:** The individual or entity which receives payments (usually the owner).

### Rev Token Lifecycle

**Unissued** tokens belong to a specific rev token pool until they are issued. Though we may discuss “how many” unissued tokens exist in a rev token pool, that is just a shorthand for talking about the size of the rev token pool itself. Tokens are not actually individuated at this stage and exist only as a pool of potential tokens with a total max full value. Once a token is issued, it becomes individuated, gains all of the rev token properties outlined above, and then proceeds through the lifecycle outlined below.

An **Inactive** token is still in its cliff period and is not yet receiving payments. Tokens which are issued with no cliff will skip this status and become active immediately upon issuance.

Once a token passes its cliff it becomes **Active** and begins receiving payments.

When a token’s received value reaches its full value it becomes **Retired.** Retired tokens no longer receive payments and may never become active again. A token may also be prematurely retired, only by its owner, as outlined in the [Rev Token Ownership Processes](./glossary.md#rev-token-ownership-processes).

### Rev Token Transfers

The owner of a rev token may sell it or otherwise transfer it to a new owner as outlined in the [Rev Token Ownership Processes](./glossary.md#rev-token-ownership-processes). The transfer process is permanent.

### Rev Token Payments

Rev token payments are received by the rev token recipient on a regular basis. 

Rev token payments pass the rev share inflows which flow into the investment ledger through to the rev token recipients of all active rev tokens linked to the ledger. Team Finance administers these payments and should seek to increase their frequency over time until they are able to go out on a monthly basis, but it may take some time to reach that frequency. 

Once revenue is flowing into the rev share inflow source ledgers, at least one rev token payment should be made each year. The goal should be regular payments throughout the year.

Each active rev token receives a payment according to the rev token weighting algorithm defined in the investment ledger’s allocation model. The algorithm must not use the rev token owner or recipient as a parameter and must allocate at least some revenue to each active rev token.

The ledger managers may optionally decide to deduct an administration percentage from the gross rev share inflows, but the full amount must go directly to helping pay for the administration of the ledger and the amount must be no more than 2%.

### Rev Token Implementation & Compliance

The implementation of the rev token system must be legally compliant, technically reliable, auditable, secure, and transparent to members. 

The initial implementation will utilize traditional business systems and tools and the manual effort of the Foundation team.

The v1 implementation will be a key priority for the Foundation and should be a primary focus of investment. The v1 implementation should utilize blockchain technology to streamline the technical operations, improve auditability, and provide greater liquidity.

### Rev Token Downgrades

It is possible for the multiples of rev tokens to decrease (but not increase) over time if there is a token downgrade on the linked investment ledger. This should be a rare event, but a possibility of which all investors should be aware. The precise governance process surrounding token downgrades is defined by the ledger’s governance process. For more details refer to [Token Downgrade Governance](#token-downgrade-governance).

In the event of a token downgrade, all rev token multiples are decreased by the same factor (a decimal number between zero and one) while respecting the core parameters of the investment ledger, specifically the min multiple and max multiple downgrade. This may mean that there are slight variances in the effective downgrade factor across rev tokens to protect them from over-downgrading.

## Rev Points

Rev points are a reward mechanism for time investors which allows members to benefit financially from the future success of the quorum without the legal and tax implications of owning an asset. 

Rev points are not assets, but a member entitlement implemented as a simple set of properties associated with each Quorum1 membership. 

Rev points are awarded to time investors for their contributions. In general the number of rev points awarded should be equal to the face value of the time investment multiplied by the rev token cohort’s multiple, but this math may differ when needed.

Things to cover in this section:

### Rev Point Structure

Rev points are linked to an investment ledger and are backed by the rev tokens in the ledger’s time investment pool. **One rev point is equal to $1 USD of full value of the rev tokens in the time investment pool.** The total number of rev points linked to an investment ledger will always equal the total full value of all the rev tokens in the investment ledger’s time investment pool.

Each Quorum1 member has a **rev point balance** for each investment ledger. The rev point balance is an integer value indicating the number of rev points held by the member within that investment ledger. Each member also has a **transaction history** of all changes made to their rev point balance.

In most cases, a member’s rev point balance goes up when they are awarded new rev points and goes down each time they receive a rev token payment. A full list of possible balance changing events is defined below.

### Rev Point Balance Changes

It is critical to the long-term success of Quorum1 that the rev point structure be safe and reliable. **Rev point balances cannot be changed arbitrarily.**

All new members start with a balance of zero rev points for all investment ledgers. Each change to a member’s rev point balance is considered a transaction and must be logged in their transaction history.

**Valid Transaction Types:**

Changes in rev point balances are only allowed for the transaction types listed in this sub-section. No other types of rev point balance changes are allowed.

- **Award:** Rev points are awarded to members from the rev point pools of ledgers according to the ledgers’ rev point plans.
- **Retraction:** Rev points awarded in error due to administrative errors or data quality problems may be retracted at a later date. Rev points may never be retracted for other reasons.
- **Transfer:** A member may transfer some of their rev points to another member.
- **Payment:** Each rev point payment received by a member reduces their balance, with each $1 USD received reducing the balance by 1 rev point.
- **Downgrade:** In the case of [Rev Point Downgrades](#rev-point-downgrades), all member rev point balances are decreased by the same factor.

### Rev Point Payments

Rev point payments are offered to each rev point holder on a regular basis.

Rev point payments pass the rev token payments received by the rev tokens in the investment ledger’s time investment pool through to all holders of rev points linked to the ledger. Team Finance administers these payments and should seek to increase their frequency over time until they are able to go out on a monthly basis, but it may take some time to reach that frequency.

Each active and eligible rev point holder is offered a payment according to the rev point weighting algorithm defined in the investment ledger’s allocation model. The algorithm must not use the rev point holder’s identity as a parameter and must offer at least some revenue to each active and eligible rev point holder. (Eligibility is defined by the [Member Rev Point Payment Requirements](./glossary.md#member-rev-point-payment-requirements) in the Financial Operations Plan.)

The rev point payment process and rev point weighting algorithm should be designed to allow each rev point holder to opt-in or opt-out of each rev point payment. If a rev point holder opts-out of a particular payment, their rev point balance does not decrease and they should be offered a benefit as a reward for not exercising their liquidity. Some or all of their non-exercised payment should then be made available to increase the rev point payments of other members.

The ledger managers may optionally decide to deduct an administration percentage from the gross time investment pool rev token payments powering the rev point program, but the full amount must go directly to helping pay for the administration of the ledger and the amount must be no more than 2%.

Aside from the administration percentage, all of the rev token payments received from the time investment pool must eventually go to rev point holders. It is acceptable, however, for portions to be held in reserve in order to support the non-exercising rewards or other programs deemed to benefit the health and sustainability of the overall rev point program.

### Rev Point Rights & Restrictions

Only Quorum1 members may receive rev point payments and members must meet the [Member Rev Point Payment Requirements](./glossary.md#member-rev-point-payment-requirements) defined in the Financial Operations Plan in order to receive payments. 

The member rev point payment requirements and all other aspects of the rev point program implementation must align with the rights & restrictions outlined in this sub-section.

- **Payment eligibility:**
    - All levels of membership are able to receive rev point payments.
    - There must always be a tier of membership which allows members to receive payments without requiring a particular level of activity or engagement from them. This means that it is not acceptable to restrict rev point payments only because of member inactivity or a lack of participation.
    - It is acceptable to restrict rev point payments for legal or tax compliance reasons or for violations of Quorum1’s rules and policies. Even in the case of restriction, however, rev point balances must be maintained and payments resumed once the underlying reasons are resolved.
    - All rev point payments must be made in compliance with all relevant laws and regulations.
- **Retraction:**
    - Once awarded, rev points may only be retracted for the following specific reasons:
        - (1) Inaccurate data used during the rev token awarding process
        - or (2) an administrative error in the rev token awarding process.
    - Rev points may never be retracted because the quorum has “changed its mind” about what the rev token awarding process should have been.
- **Transfers:**
    - Members must be able to transfer rev points to other members. Members must be protected from fraud such that transfers can be reversed if fraudulent behavior is found to have occurred.
    - Rev points are not an owned asset and may not be formally sold, though the quorum may strive in the future to provide a method for members to exercise greater liquidity with their rev points.
- **Major events:**
    - Upon the deactivation, suspension, or relinquishment of a Quorum1 member account (in accordance with Quorum1’s rules and policies), the member’s rev point balances are maintained for as long as they live, though rev point payments are paused while they are inactive. If at a future date the member becomes active again, the member’s rev point balances become immediately available.
    - Each member may specify another member as their designated beneficiary in the case of their death. Upon a member’s death, their rev point balance is transferred to their designated beneficiary. If no surviving beneficiary is designated, then the rev point balance is transferred to a shared ledger for the collective benefit of all members.
    - A member’s balance may be adjusted if Quorum1 is instructed and required to to so by a governmental authority.

### Rev Point Implementation & Compliance

The implementation of the rev token system must be legally compliant, technically reliable, auditable, secure, and transparent to members. It is particularly critical that the rev point implementation be compliant with the spirit and letter of tax regulations such that the awarding of rev points is not a form of income. The regular rev point payments should be structured as taxable independent contractor income.

The initial implementation will utilize traditional business systems and tools and the manual effort of the Foundation team. It is likely, but not mandatory, that the initial implementation will be built using [Workstream Wallets](./glossary.md#workstream-wallets).

The improvement and increased automation of the rev point implementation will be a key priority for the Foundation. There is no immediate plan for utilizing blockchain in the rev point implementation, since liquidity and external audibility are not critical requirements. But the Foundation is free to consider a blockchain-based implementation if it is deemed to be beneficial.

### Rev Point Downgrades

It is possible for the multiples of rev tokens to decrease (but not increase) over time if there is a token downgrade on the linked investment ledger. This should be a rare event, but a possibility of which all investors should be aware. The precise governance process surrounding token downgrades is defined by the ledger’s governance process. For more details refer to [Token Downgrade Governance](#token-downgrade-governance).

In the event of a token downgrade, all member rev point balances are decreased by the same factor (a decimal number between zero and one) while respecting the core parameters of the investment ledger, specifically the min multiple and max multiple downgrade. This may mean that there are slight variances in the effective downgrade factor across members to protect them from over-downgrading.

---

# Appendix

## Sale of Quorum1

Quorum1’s Governance Model will eventually define the formal process for a future sale of Quorum1. However, as outlined above, since that doc has yet to be formalized, this section will briefly lay out some requirements for any future sale of the quorum.

In order for Quorum1 to be sold, the following things would be required, in accordance with the Governance Model at the time of sale:

- Approval of the sale by both the Org leadership and the Foundation leadership.
- Approval of the sale by the active Org membership.
- Approval of the sale by a vote of all rev token owners and of all rev point holders.
- Either the purchaser’s agreement to continue honoring the rev token and rev point structure into the future, or the purchase by the purchaser of all issued rev tokens along with liquidation of all accrued rev point benefits.

In the case of a rev token purchase and rev point liquidation, the purchaser would offer a cash value equal to a purchase factor multiplied by the full value of all issued rev tokens. The same purchase factor must be applied to all rev tokens and when liquidating all rev point benefits.
