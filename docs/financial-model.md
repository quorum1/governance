# Financial Model v2

This agreement defines how Quorum1 (also referred to as “the quorum”) handles money as a collective, specifically the funds in the accounts held by Quorum1. Our goals are to ensure legal compliance, financial solvency, and operational reliability while making financial flows throughout the network as transparent as possible and supporting emergent innovation by directing significant funds to participatory budget allocation.

---

# Governance

This document is formally referred to as the **Quorum1 Financial Model Definition**, or more casually as the **Financial Model**. 

The **Financial Model** is a living document. Changes to the Quorum1 Financial Model Definition are governed by the [Change Process for Financial Model Definition](#change-process-for-financial-model-definition).

The operational implementation of the Financial Model is referred to as the **Financial Operations Plan**. Any details that are not defined in the Financial Model can be defined in the Financial Operations Plan. The Financial Operations Plan is managed more fluidly than the Financial Model itself and is documented separately. It must comply with the [Required Components of Financial Operations Plan](#required-components-of-financial-operations-plan). Changes are governed by the [Change Process for Financial Operations Plan](#change-process-for-financial-operations-plan).

---

# Quorum1 Structure

The full definition and specifications of Quorum1’s structure and governance are the domain of the Quorum1 Governance Model, not the Financial Model. As such, this section is somewhat beyond the intended scope of this document. However, as of the writing of this document, the Governance Model is still informally defined. This section lays out some basic aspects of Quorum1’s structure that are needed in order to properly contextualize the Financial Model. In future versions after the formal Governance Model is defined, this section may no longer be needed.

The relationship between the various parts of Quorum1 can be expressed thusly: 

- The Foundation manages and improves the Platform.
- The Org runs on top of the Platform and manages the Foundation.
- Hosted Entities also run on top of the Platform and contribute to the Org and Foundation.

## The Org

The Org is the entirety of Quorum1, including all members, and aspires to be democratic, poly-centric, and non-hierarchical with a fluid and emergent structure. Participatory democratic action and consensus-building are key goals of the processes happening within the Org. The Org as a whole is the source of ultimate decision-making authority within Quorum1.

The Org contains sub-groups called quorums, some designated as core quorums. Each quorum is led by a single “point” member, and potentially also by a “triad” of three members.

The Org is led by the Core Points (the points from each core quorum), and by the Org Point. Points are considered leaders but not executives, in that they do not hold specific executive authority. The triad members may have executive authority.

The Org has four levels of membership, listed in increasing levels of commitment and trust:

- **Network members** create user accounts in Quorum1’s app suite and agree to our terms of service, but make no specific commitments to engagement level and have limited access to our systems.
- **Community members** commit to a certain level of engagement and make lightweight agreements around collaboration and sharing. They are given increased but still limited access to our systems.
- **Contributor members** sign formal membership agreements and are able to participate in paid projects and make significant contributions. They are given full end user level access to most systems, though administrative permissions and systems are granted based on other criteria.
- **Partner members** sign formal partnership agreements and are owning members of Quorum1’s underlying legal entity. They have the highest level of end user level systems access.

## The Platform

The Platform is a term for referring to, in its totality, the infrastructure needed to support the continued thriving operation of Quorum1 as a whole.

## The Foundation

The Foundation is a set of executive-led teams which exists in order to maintain and improve the Platform.

The leadership, structure, and mandate of the Foundation is ultimately managed by the Org via its participatory democratic processes. The Foundation also aspires to be participatory and democratic, but with a greater focus on operational stability, safety, security, reliability, and predictability.

The Foundation is made up of executive-led teams which may change over time, but which must include the following:

- Team Finance is responsible for Quorum1’s financial operations
- Team Legal is responsible for Quorum1’s legal operations and compliance
- Team Ops is responsible for Quorum1’s business and technical operations
- Team Build is responsible for building and maintaining Quorum1’s core technology

The Foundation is led by the Managing Partners, a group of up to three members. The Managing Partners are considered leaders and executives and hold executive authority over the Foundation, but ultimately serve at the behest of the Org as a whole.

## Hosted Entities

The Platform also serves to host other “virtual” business entities which exist in order support entrepreneurial innovation and revenue generation. These Hosted Entities operate with a high degree of financial and creative autonomy and contribute financial support back to the Org and the Foundation.

The types of hosted entities are listed below. The process for creating, changing, and retiring hosted entities is defined by the [Hosted Entity Management Process](#hosted-entity-management-process). Hosted entities will be established as separate legal entities as needed.

Each hosted entity is also considered a quorum, has a triad and a point, and is able to define its own governance process.

### Types of Hosted Entities

- A **Line of Business** is a simple type of Hosted Entity intended primarily to manage a set of service offerings made under the Quorum1 brand or another brand (an “alt-brand”, described in the next section).
- A **Virtual Company** is a more complex type of Hosted Entity intended to support a wide range of entrepreneurial activities, including product development, professional services, marketplaces, paid memberships, investment, shared ownership, and more.

### Key Properties of Hosted Entities

- **Entity Fund:** All hosted entities have their own funds, usually a pass-through fund. The fund is managed and governed as defined by the hosted entity.
- **Brand:** A hosted entity is “Q1-branded” if it operates under the Quorum1 brand, or “alt-branded” if it operates under its own brand.
- **Investment:** A hosted entity is said to be “investable” if it is able to receive investment. Investable entities must have their own rev share fund.
- **IP Bucket:** Some hosted entities have a collection of IP containing original inventions, ideas, processes, designs, copyrights, and patents.
- **Ownership Agreement:** Some hosted entities have an agreement outlining the guidelines for how ownership will be allocated if the hosted entity is ever spun out into a separate legal entity.

### Property by Hosted Entity Type

Almost all of the properties are mandatory for a virtual company. Lines of Business are comparatively simpler and more limited.

| Hosted Entity Type | Fund? | Brand? | Investable? | IP Bucket? | Ownership Agreement? |
| --- | --- | --- | --- | --- | --- |
| Line of Business | ✅ | Optional | ❌ | ❌ | ❌ |
| Virtual Company | ✅ | ✅ | ✅ | ✅ | ✅ |

## Sale of Quorum1

Quorum1’s Governance Model will eventually define the formal process for a future sale of Quorum1. However, as outlined above, since that doc has yet to be formalized, this section will briefly lay out some requirements for any future sale of the quorum.

In order for Quorum1 to be sold, the following things would be required, in accordance with the Governance Model at the time of sale:

- Approval of the sale by both the Org leadership and the Foundation leadership.
- Approval of the sale by the active Org membership.
- Approval of the sale by a vote of all rev token owners and of all rev point holders.
- Either the purchaser’s agreement to continue honoring the rev token and rev point structure into the future, or the purchase by the purchaser of all issued rev tokens along with liquidation of all accrued rev point benefits.

In the case of a rev token purchase and rev point liquidation, the purchaser would offer a cash value equal to a purchase factor multiplied by the full value of all issued rev tokens. The same purchase factor must be applied to all rev tokens and when liquidating all rev point benefits.

---

# Funds

Funds are Quorum1’s financial accounts. Funds have inflows of money and rev points, can hold money and rev points, and have outflows of money and rev points. Funds can also award rev points.

The fund management infrastructure is maintained by Team Finance. There are a fixed set of [Standard Funds](#standard-funds) set out in this document, but the full database of funds will evolve organically over time, supporting an emergent financial design for the quorum. 

Team Finance manages the working database of all funds and defines clear processes for creating, changing, and retiring funds (the [Fund Management Process](#fund-management-process)). Team Finance is also responsible for maintaining permanent audit trails of all funds, changes to funds, and fund activity.

## Key Properties of a Fund

Below are some of the most important properties that make up a fund’s design.

- **Fund Manager:** A single contributor or partner member who is responsible for interfacing with Team Finance and assisting with the management and administration of the fund.
- **Fund Type:** The available types and their features are defined in this document.
- **Fund Allocation Model:** Describes the fund’s outflows.
- **Fund Governance Process:** Describes who is allowed to make changes to the fund’s design and how those changes are approved.
- **Fund Status:** “Proposed”, “Active”, or “Retired”
- **Receivable / Non-Receivable:** Only receivable funds are able to receive external income directly. Non-receivable funds only receive money through cross-fund outflows.
- **Rev Point Pool:** Funds are able to receive unawarded rev points through various mechanisms. These rev points sit in the fund’s rev point pool until awarded to a member or transferred to another fund’s rev point pool.
- **Rev Point Plan:** Describes how rev points from the rev point pool are awarded.
- **Rev Token Cohorts:** Only for investment funds, outlined in more detail in the [Investment Fund Rev Token Cohorts](#investment-fund-rev-token-cohorts) section.

## Allocation Models

A fund’s allocation model describes the fund’s outflows, meaning how money flows out of the fund. The exact format of the allocation model is defined by the [Allocation Model Templates](#allocation-model-templates) and is standardized for each fund type. All allocation models, however, are essentially lists of outflows. 

Each outflow has a single allocation target and specifies how much money should flow to that allocation target. The types of valid allocation targets are described in detail in the [Outflows](#outflows) section, but at a high level: internal outflows allow funds to pass money on to other funds or [Workstream Wallets](#workstream-wallets), while external outflows allow funds to send money out of the quorum. 

For receivable funds, the allocation model must include certain required allocations based on the type of income they receive. The details of this are outlined in the [Standard Income Allocations](#standard-income-allocations) section.

## Rev Point Pools & Plans

Funds are able to receive unawarded rev points and hold them in their fund rev point pool. The points are intended to be awarded to reward and incentivize contributions. Not all funds will have rev points in their rev point pool.

There are two ways to award rev points: (1) By designing a rev point plan and (2) by transferring rev points to [Workstream Wallets](#workstream-wallets) via an allocation model outflow. The rest of this sub-section is focused on the former method.

To award rev points directly to members, a fund must create a rev point plan outlining how the rev points will be awarded. The rev point plan must clearly define the parameters of how rev points are to be awarded including: who is able to participate, the earning cycle, the specific data that will be delivered, how the point earnings are calculated based on the data, what happens when there’s not enough rev points in the pool to cover all of the earnings in an earning cycle, and all other details required to properly administer the program.

It is allowed for a rev point pool to begin accruing rev points without having a rev point plan defined. It is also allowed to change the design of the rev point plan frequently as long as those changes are communicated to all impacted members and they are given a voice in the decision-making process.

Team Finance is responsible for administering the awarding of rev points as outlined in the rev point plan and based on the data provided by the fund manager. The fund manager must work with Team Finance to ensure that the fund design makes sense and is feasible to administer.

Unawarded rev points may be transferred to another rev point pool by the fund manager. Unawarded rev points may also be subject to reallocation by the source investment fund if they remain unawarded for a protracted period of time, according to the investment fund’s rev point plan.

Rev points and their related processes are outlined in more detail in the [Investment](#investment) section.

## Fund Types

Each fund type is designed to provide a specific set of features for managing our money. Taken as a whole, the fund types are intended to serve as modular building blocks able to be linked together by fund designers to build the infrastructure needed to support different parts of the quorum’s business.

The standardization of these fund types is critical for streamlining our financial and technical operations. The modularity of these fund types is critical for allowing the flexibility we need to grow, evolve, and adapt.

### Pass-Through Funds

Pass-through funds simply allocate all inflows directly to a list of allocation targets, with a specific percentage flowing to each target.

Pass-through funds may optionally also include a set of fixed dollar amount outflows which are taken “off the top” before the rest of the inflowing money is allocated based on percentages.

### Fulfillment Funds

Fulfillment funds (potentially also called “project fulfillment funds” or just “project funds”) hold money intended to compensate the fulfillment of a particular project or client engagement. They are necessarily a bit more complex than other fund types. Fulfillment funds are used for all consulting engagements, for internal Quorum1 projects, product development work, and anything else where outflows are linked to work fulfillment. 

Fulfillment funds keep track of how much revenue has been fulfilled and produce outflows based only on fulfilled revenue. Fulfillment funds also support a refund mechanism for returning the remaining balance to its source if a project is canceled before all of the revenue has been fulfilled.

There are two types of fulfillment funds:

- **Hourly** fulfillment funds are fulfilled by line item hours being tracked and verified in the [Time Tracking System](#time-tracking-system).
- **Percentage** fulfillment funds are fulfilled based on verified completion percentages for each line item. These can also be used to implement recurring payments in fixed amounts.

The allocation model of a fulfillment fund is also referred to as a “project cost model”. The project cost model defines two lists of allocation targets: 

- The **line item allocations** produce the fulfilled revenue. Each line item includes a bill rate and a cost rate. The bill rate yields the amount of revenue fulfilled. The cost rate, which must be equal to or lower than the bill rate, yields the amount received by the allocation target. The difference between the bill rate and cost rate yields the margin.
- The **margin allocations** each receive a fixed percentage of the fulfilled revenue. Note: The project cost model must be designed so that the smallest line item margin percentage is equal to or greater than the sum of all margin allocation percentages, to prevent cost overruns.

### Expense Funds

Expense funds hold money intended to pay for vendor expenses. Expense funds may have one or more virtual or physical debit cards linked to them, according to the [Debit Card Management Process](#debit-card-management-process).

Expense funds may only be used to pay for the following types of outflows:

- One-time payments to registered vendors, requiring a corresponding invoice
- Recurring payments to registered vendors, via the [Recurring Expense Management Process](#recurring-expense-management-process)
- Reimbursement requests from members, via the [Expense Reimbursement Process](#expense-reimbursement-process)

The fund manager is expected to maintain a viable level for the expense fund to ensure a reasonable runway to cover recurring expenses. Team Finance is responsible for providing fund managers with the tools and visibility needed to manage the levels in the fund. Overdrafts or shortfalls in an expense fund may result in Team Finance retiring the fund or requiring a different fund manager.

### Reserve Funds

Reserve funds hold money in reserve to provide financial security and help us manage risk. Reserve funds do not have any pre-defined outflows. Instead, each transfer of money out of a reserve fund must be approved according to an approval process defined in the allocation model for the reserve fund.

### Collaborative Funds

Collaborative funds hold money intended to be assigned to projects and initiatives as determined through collaborative processes open to the participation of some or all quorum members.

The allocation model of a collaborative fund defines the specific set of quorum members who should be included in the collaborative process and any guidelines or limitations that the collaborative process itself must meet, as well as how often the process should be run.

Before the running of a collaborative funding process, the process itself must be clearly defined. An appropriate audit trail must also be recorded as part of the collaborative funding process log.

### Bonus Funds

Bonus funds hold money used to award bonuses for certain activities which are part of a well-defined incentivization program. This includes sales & marketing commissions, client referral fees, new member recruiting bonuses, and other similar programs. 

Note that, like all funds, bonus funds may only direct outflows to valid [Fund Outflows & Allocation Targets](#fund-outflows--allocation-targets). This means that community members are not able to receive bonus payouts directly.

Team Finance is responsible for administering the calculation and disbursement of bonuses based on data provided by the fund manager. The fund manager must work with Team Finance to ensure that the bonus fund design makes sense and is feasible to administer.

The allocation model of a bonus fund must clearly define the parameters of the incentivization program including: who is able to participate, the earning cycle, the specific data that will be delivered, how the bonuses are calculated based on the data, what happens when there’s not enough money in the fund to cover all of the bonuses in an earning cycle, and all other details required to properly administer the program.

It is allowed for a bonus fund to begin accruing money without having an incentivization program defined. It is also allowed to change the design of the incentivization program frequently as long as those changes are communicated to all impacted members and they are given a voice in the decision-making process.

### Investment Funds

An investment fund is a special type of fund which can receive investment income, create rev tokens, create rev points, and share revenue passed from other funds back with active rev token recipients and rev point holders.

For more information on investment funds refer to the [Investment Funds Detail](#investment-funds-detail) section. The full details on the quorum’s investment mechanisms are outlined in the [Investment](#investment) section.

## Standard Funds

This section lists the set of standard funds that are mandatory and exist to serve key functions for operating and supporting Quorum1 holistically. These funds must always exist and are administered directly by Team Finance and managed either by the Managing Partners or by a foundation team appointed by Managing Partners. The fund manager of each standard fund is appointed by the team responsible for managing the fund.

The allocation models of each standard fund are part of the Financial Operations Plan and managed according to the [Change Process for Financial Operations Plan](#change-process-for-financial-operations-plan).

### Core Fund

The core fund is a pass-through fund. The core fund is used to pay for Quorum1’s operating expenses and core programs. All Quorum1 income must allocate a certain percentage to the core fund, based on the type of income. 

The core fund must allocate a percentage to each of the other standard funds listed in this section. The core fund may not directly allocate to any non-standard funds. The precise allocation percentages are defined by the core fund allocation model.

### Org Expense Fund

The org expense fund is an expense fund used to pay for all core vendor expenses. This includes things like operating costs, insurance, business systems, service providers, taxes, and fees. Over time many non-standard expense funds will exist and are by definition allowed to manage vendor expenses on their own. However, fund managers of non-standard expense funds are encouraged (but not required) to allocate particular vendor expenses to the standard org expense fund instead when it makes sense to do so (such as in order to negotiate a lower cost).

### Org Reserve Fund

The org reserve fund is Quorum1’s primary reserve fund. This fund can be used to pay for unexpected expenses or anything related to supporting the continued operation of the quorum. However, this fund’s balance should be kept at a sufficient level at all times.

Ideally this fund should target a balance sufficient to cover 2 to 3 months of foundation operations and org expenses. If the fund’s balance exceeds 12 months of foundation operations and org expenses, then the quorum should consider re-allocating some of the reserve to other uses.

### Foundation Operations Fund

The foundation operations fund is a pass-through fund intended to pay for everything required to keep the Foundation Team running and to provide operating capital for ongoing maintenance and investment in continued innovation of the quorum platform. This fund should be used to pay for Foundation Team salaries and contracts, and to allocate money to [Workstream Wallets](#workstream-wallets) to support maintenance and innovation of the systems managed by the Foundation Team. This fund may also be used to fund any other efforts that are related to the support, maintenance, improvement, promotion, and improvement of Quorum1.

### Org Investment Fund

The org investment fund is our primary investment fund and is maintained by Quorum1 for the org as a whole. Rev tokens in the org investment fund are exchanged with investors of both time and money. Prioritization, allocation, and other decision-making processes around the org investment fund must always be participatory and democratic in accordance with Quorum1’s established best practices as they evolve.

This fund and the linked rev tokens are a critical part of Quorum1’s financial infrastructure. More details are outlined in the [Investment](#investment) section, the fund design is part of the Financial Operations Plan as outlined here: [Org Investment Fund Design](#org-investment-fund-design).

In the event of the full fund liquidation of the org investment fund for any reason, all token holders must convert at the same discount rate, weighting, or liquidation preference.

### Org Bonus Fund

The org bonus fund is a bonus fund intended to fund Quorum1’s org incentivization program.  Quorum1’s org incentivization program should focus primarily on rewarding the sales, biz dev, marketing, and demand generation work needed to drive new paid project work. But the program may also reward efforts on critical initiatives that impact the entire quorum.

### Org Collaborative Fund

The org collaborative fund is a collaborative fund intended to fund internal Quorum1 projects and new product development projects that are selected via periodic participatory budgeting processes involving all community, contributor, and partner members.

---

# Inflows

Inflows are money or rev points that flow into a fund.

There are technically two types of inflows: internal inflows (from other funds) and external inflows (aka income). However, since internal inflows are very simple, the bulk of this section is dedicated to discussing income.

## Internal Inflows

Internal inflows are money that flows into a fund from another fund, through a cross-fund outflow. These are described in more detail in the [Cross-Fund Outflows](#cross-fund-outflows) section.

## Income (External Inflows)

External inflows are our income. Income is money that flows into Quorum1 from external sources. Each incoming payment is associated with a specific receivable fund and the money flows according to the fund’s allocation model.

Income may only flow into funds which are designated as being “receivable”. In order to be receivable, a fund must comply with the [Receivable Fund Requirements](#receivable-fund-requirements). For example, a receivable fulfillment fund for a client project may require a signed SOW.

### Income Types

The income type impacts many different things, including which types of funds may be targeted, the standard income allocations, and the required documentation checklist used during income reconciliation. 

All income must be categorized as a single income type. Payments which contain multiple types of income are split during the bookkeeping process so they can be processed separately.

- **Service** income comes from professional services work performed for clients.
- **Product** income comes from fees charged for physical or virtual products, including “Software-as-a-Service” fees and other product subscription fees. For now we are far more likely to sell software products rather than hardware products.
- **Investment** income (which is not considered “income” in the traditional sense, but which is an external inflow and thus “income” as defined in this document) comes from purchases of rev tokens as outlined in the [Investment](#investment)  section.
- **Marketplace** income comes from money loaded into a quorum-operated marketplace. This income type is still experimental and, for now, will only come from payments between [Workstream Wallets](#workstream-wallets). Revenue may not be recognized until the money loaded into a wallet is actually transacted via the workstream.
- **Other Income** which does not fit the above categories is processed and allocated ad hoc by Team Finance.

### Standard Income Allocations

All receivable funds must include the following standard income allocations, as relevant:

1. All income must allocate a required percentage to the **core fund.** The required percentage is defined by the [Standard Income Allocation Table](#standard-income-allocation-table), part of the Financial Operations Plan.
2. Income linked to a hosted entity must allocate a required percentage to its corresponding **hosted entity fund**. The required percentage is defined by the hosted entity in accordance to its governance process.

**Standard Income Allocation Table Format and Default Values:**

The [Standard Income Allocation Table](#standard-income-allocation-table) is part of the Financial Operations Plan, not the Financial Model and may be changed without updating this doc. 

The standard income allocation table defines the required percentage of recognized income that must be allocated to the core fund for each type of income based on various parameters, including whether the income is associated with a hosted entity and whether it uses the Quorum1 brand. 

The standard income allocation table should match the basic format outlined here. The actual values may differ, however. And the actual format may also differ slightly as long as it aligns with the spirit of this design.

In the interim period before an official standard income allocation table is finalized, the values in the table below will serve as defaults.

| Income Type | Hosted Entity? | Brand Type | Core Fund % |
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

¹ Projects operated under the Quorum1 brand and not associated with a hosted entity have a default core fund allocation of 20%. But when led by partner members, they may optionally allocation a lower amount, as low as 15%.

² Marketplace income is experimental for now and only pertains to transaction fees related to [Workstream Wallets](#workstream-wallets).

### Available Fund Types by Income Type

Each type of income may only be received by certain types of receivable funds.

| Income Type | Core Fund? | Hosted Entity Fund? | Generic Pass-Through Fund? | Project Fulfillment Fund? | Investment Fund? |
| --- | --- | --- | --- | --- | --- |
| Membership | ✅ | ✅ | ❌ | ❌ | ❌ |
| Service | ❌ | ❌ | ❌ | ✅ | ❌ |
| Product | ❌ | ✅ | ✅ | ❌ | ❌ |
| Investment | ❌ | ❌ | ❌ | ❌ | ✅ |
| Marketplace | ✅ | ✅ | ✅ | ❌ | ❌ |

### Income Reconciliation

Team Finance is responsible for reconciling each incoming payment. Only after a payment is reconciled does it become income. Any payments which cannot be reconciled may need to be refunded or held in escrow until they can be reconciled.

The income reconciliation process involves matching an incoming payment with a specific fund and verifying that the required documentation is complete. The [Required Income Documentation Checklist](#required-income-documentation-checklist) is part of the Financial Operations Plan.

### Fulfillment, Recognition, & Refunds

Most quorum income is recognized as revenue immediately upon receipt. But receivable fulfillment funds are unique in that they do not recognize revenue until it is fulfilled as defined by the fund’s project cost model. (More details on this fund type: [Fulfillment Funds](#fulfillment-funds))

Unfulfilled (and therefore unrecognized) revenue in a fulfillment fund may be refunded in accordance to the [Refund Process](#refund-process).

---

# Outflows

Outflows are money or rev points that flow out of a fund as defined by the fund’s allocation model. Each outflow has a single allocation target (where the money goes to).

There are two basic types of outflows: internal outflows and external outflows.

## Internal Outflows

Internal outflows are money that flows to allocation targets which are inside of the quorum.

### Cross-Fund Outflows

Cross-fund outflows are money or rev points that flow from one fund to another fund. Any fund is able to be an allocation target of any other fund.

Cross-fund outflows may optionally include usage requests that specify how the money or rev points should be used (such as paying for a specific expense). These usage requests are not strictly binding but the fund managers should make a good faith effort to respect them.

### Workstream Wallet Outflows

Workstream wallet outflows allow funds to move money or rev points into specific [Workstream Wallets](#workstream-wallets). This in turn enables more agile work structures and gives the wallet managers the ability to source help from the full quorum membership.

## External Outflows

External outflows are money that flows to allocation targets which are outside of the quorum.

### Member Outflows

Contributor and partner members are valid allocation targets based on their eligibility according to the [Member Payment Eligibility Process](#member-payment-eligibility-process). If members have joined the quorum via a corporate entity, then their payments are directed to their registered corporate entity.

### Vendor Company Outflows

Vendor company outflows send money to vendors that have been registered according to the [Vendor Registration Process](#vendor-registration-process). These types of outflows may be subject to additional requirements, such as needing copies of invoices or receipts.

### Rev Token Outflows

Rev token outflows are only available to investment funds. These outflows send money to the fund’s active rev token recipients. This process is outline in the [Investment](#investment) section. 

---

# Investment

We believe that Quorum1 has the potential to generate tremendous wealth over the coming years. If achieved, it is critical to our mission that this wealth be both re-invested in nurturing future success *and* shared equitably with the individuals and organizations that helped build the wealth engine. This is our dual investment mission: To balance our support of future innovation with our returns to our ever-growing community of investors.

The former goal of re-investment is achieved via the [Org Collaborative Fund](#org-collaborative-fund), and the other [Collaborative Funds](#collaborative-funds) which will emerge over time, as well as through the emergent properties intrinsic to our unique organizing model.

The latter goal of equitably sharing wealth with our investors—of both time and money—is addressed in this section.

In creating our design for a Quorum1 investment mechanism, we require that it be aligned with our goals, mission, and values. We also require that our investment mechanism function within the logistical and operational environment of our emergent org structure.

## Quorum Investment Model Key Concept Overview

These concepts are outlined in greater detail in later sections, but below is a brief summary of some of the key concepts which make up our investment model.

- **Investment Fund:** Special type of fund which can receive investment income, create rev tokens and rev points, and share revenue passed from other funds back with active rev token recipients and rev point holders.
- **Types of Investment:**
    - **Time Investment:** The contribution of work, effort, or support to the quorum.
    - **Formal Money Investment:** Money invested in a formal investment round
    - **Informal Money Investment:** Money informally invested outside of an investment round
- **Rev Token Concepts:**
    - **Rev Token:** An owned asset which entitles the owner to receive rev token payments. Each rev token is linked to an investment fund. Each rev token has a face value, a multiple, and a full value equal to the face value times the multiple.
    - **Rev Token Payments:** Revenue share income flows into an investment fund and is passed through to active rev token recipients via regular rev token payments.
    - **Rev Token Cohort:** Groups of rev tokens within an investment fund. Able to be nested via “sub-cohorts” within “parent cohorts”. Can be used to weight rev token payments.
- **Time Investment Concepts:**
    - **Time Investment Pool:** For investment funds only. A pool of issued rev tokens held by Quorum1 with the received payments powering the fund’s rev point program.
    - **Rev Point:** A reward mechanism for time investors which allows members to benefit financially in the future success of the quorum without the legal and tax implications of owning an asset.
    - **Rev Point Payments:** Rev token payments received by the rev tokens held in the fund’s time investment pool are passed through to rev point holders via regular rev point payments.
    - **Rev Point Pool:** Each fund (including non-investment funds) has a rev point pool which can hold unawarded rev points which are awarded to members who make contributions according to the fund’s rev point plan.

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

<aside>
⚠️ **Rev points are intended to be a form of supplementary or bonus income (analogous to stock options in a startup), not the primary form of compensation.** The primary form of compensation for time investors should be cash. In cash-lean periods it may be necessary for rev points to largely (or fully) take the place of cash compensation, but the practice should be avoided when possible.

</aside>

### Money Investment

Money investment in Quorum1 is the process of issuing rev tokens to investors in exchange for money. Each investor must be onboarded as defined by the [Investor Management Process](#investor-management-process). The face value of money investment rev tokens is always equal to the amount paid by the investor.

Money investment takes two forms:

- **Formal investment** is money investment associated with a specific investment round. Investment rounds are part of the fund’s rev token plan and are managed in accordance with the fund’s governance process.
- **Informal investment** is ad-hoc money investment not associated with a specific investment round. Informal investment can be used for “cash calls” to cover expenses or other purposes. Participation in informal investment is considered an earned privilege and is restricted to a members who meet the criteria outlined in the fund’s rev token plan. (For instance, informal org investment is limited to partners.)

## Investment Funds Detail

All investment in the quorum is managed through investment funds (one of our [Fund Types](#fund-types) ). An investment fund is a special type of fund which can receive investment income, create rev tokens and rev points, and share revenue passed from other funds back with active rev token recipients and rev point holders.

The [Org Investment Fund](#org-investment-fund) is our standard investment fund and must maintain ongoing continuity, but other investment funds may be created and changed over time according to the [Investment Fund Management Process](#investment-fund-management-process). Investment funds are necessarily complex, involving special legal contracts and, in some cases, custom technology to facilitate their ongoing operations. Each investment fund may also present unique regulatory and compliance challenges. This means that rev share funds require the support and alignment of Team Finance, Team Legal, Team Ops, Team Build, and the Managing Partners.

The org investment fund may be used to reward and incentivize investment in any part of Quorum1 or in areas deemed important by the quorum. Other investment funds will have their own design, limitations, and participation, defined by the members and leaders of each fund.

### Standard Process for Designing an Investment Fund

The exact process for creating a new investment fund is part of the [Investment Fund Management Process](#investment-fund-management-process) defined in the Financial Operations Plan. But it must align mostly with this standard process.

1. **Establish the Budget:** An investment fund is essentially a collection of loans (rev tokens) and can be thought of as one big loan with the average terms across all the rev tokens. So the first step is to determine the size of the entire loan. To do that we follow the steps below:
    1. Determine target “break-even” return for all investors. Something lower than the full multiple but good enough to count as a type of success. (For example: `BreakEvenReturn` = 5x.)
    2. Determine target timeline for break-even return. (For example: 10 years.)
    3. Set an optimistic revenue goal for the timeline. It’s ok to be extra optimistic or more conservative, based on the shared values of the fund founders, numbers can be adjusted later as more learning is generated. (For example: `RevGoal` = $1 billion.)
    4. Set a conservative estimate of the fraction of revenue allocated to fund rev share. (For example: `RevAllocationFraction` = 5%)
    5. Determine what you want your average multiple to be once the fund is full (meaning that the face value or total value of all of the created rev tokens has reached the fund budget and no more rev tokens can be created). Higher means you’ll be retiring risk more slowly, staying experimental for longer. Lower means you retire the rev tokens in less time. (For example: 20x)
    6. The total face value of the fund can be determined with the formula below, or another technique if desired. This technique makes the simplified assumption that generating half of the break even in a single year’s rev allocation results in break even that year, with the other half coming cumulatively over the preceding years. (For our example: Total Face Value is $20M)
        
        $$
        \{TotalFaceValue\} = \frac{\{RevGoal\} * \{RevAllocationFraction\}}{\{BreakEvenReturn\} * \frac{1}{2}}
        $$
        
    7. The total full value of the fund can then be determined thusly. (For our example: Total Full Value is $400M)
        
        $$ \{TotalFullValue\} = \{TotalFaceValue\} * \{AverageMultiple\} $$
        
2. **Design Cohorts:** Put together the initial rev token cohorts.
    1. **Legacy Cohorts:** You will likely start with one or more “legacy cohorts” for the time and money invested before the fund existed. The recommendation is to create one per year. Amongst the participants in each cohort you’ll want to align on the following:
        1. Rough estimate of time and money investments made and use that to create a **max budget** for each legacy cohort. At this stage it’s best to estimate on the high side and round up.
        2. The **multiple** for each year. The recommendation is that early high-risk years are around 100x and that that drops significantly almost every year.
        3. Any **guidelines around the participatory processes** which will be used to run the legacy allocation process after the fund is launched.
    2. **First Cohort:** The first cohort will kick off when the fund is launched and ideally last until the end of the current calendar year.
3. **Finalize Design:** Finish determining all of the other aspects of the investment fund’s design. Get all relevant stakeholders in alignment. Run whatever governance processes required to have authority to move forward.
4. **Launch Fund:** Get initial contracts signed and set everything up operationally. Can begin raising investment as needed. 
5. **Legacy Allocation:** Run a participatory legacy cohort allocation processes determined by the fund founders. For each legacy cohort, the process should do the following:
    1. Collect receipts and transaction logs for money investments (the distinction between formal and informal is irrelevant for now) and collaboratively verify the accuracy and qualification of each item
    2. Collaboratively determine a framework for valuing the time investments.
    3. Collaboratively assess precise rev point assignments for each member within each part of the determined framework.
    4. Result in a precise dollar amount of money investment rev tokens and time investment rev points which is less than or equal to the max budget established in the design phase.
6. **Begin Rev Token & Rev Point Payments:** Once the legacy allocations are complete, initial payments can begin.

### Investment Fund Implementation Details & Risk

At the time of writing and approving the Financial Model, the technical, operational, legal, and financial implementation details have not been finalized. This means that key details around contract structure, legal design, tax treatment, and ongoing operations are still being developed. This further means that there is some amount of risk that parts of this design will not be able to be implemented as intended. 

In order for us to fund and incentivize this development work (and to formally recognize the years of work already put into the quorum), however, it is necessary for Quorum1 to begin issuing rev tokens and awarding rev points before the development work is complete. We acknowledge that this approach creates the risk that these initial rev tokens and rev points will need to be modified in the future once the implementation details have been finalized. 

We believe, however, that the implementation of this model will ultimately succeed and that whatever further Financial Model iteration is required will produce minimal changes to the structure of the initial rev tokens and rev points. We further believe that it would be difficult or impossible to implement a model as novel as the rev token and rev point structure without an immediately real world use case.

It is important to note, though, that in the most severe case it is possible that the entire rev token and rev points structure may prove fundamentally infeasible. For that reason, every investment fund created before the finalization of the implementation details must include a “failsafe equity conversion” governance process. This process outlines the steps to be followed only in the case that rev token and rev point structures are considered to be fundamentally infeasible to implement.

This is outlined in more detail in this section: [Key Governance Process: Failsafe Equity Conversion](#key-governance-process-failsafe-equity-conversion).

### Investment Fund Inflows & Outflows

Investment funds have the following inflows:

- **Investment income¹** flows in from money investors and is exchanged for rev tokens.
- **Rev share inflows** flow in from other funds and are used to pay back investors.

Investment funds have the following outflows:

- **Investment outflows** allocate investment income to target funds, according to the fund’s allocation model
- **Rev token payments²** allocate rev share inflows to rev token recipients.
- **Rev point payments³** allocate the rev token payments from the time investment pool to rev point holders

***¹ Investment income:** Each investor must be onboarded as defined by the [Investor Management Process](#investor-management-process). Formal money investment is associated with an investment round, informal money investment is not associated with an investment round.*

***² Rev token payments:** Rev share inflows are passed through to the active rev token recipients as outlined in the [Rev Token Payments](#rev-token-payments) section.*

*³ **Rev token payments:** Time investment pool rev token payments are passed through to the rev point holders as outlined in the [Rev Point Payments](#rev-point-payments) section.*

### Investment Fund Core Parameters

Every investment fund has a set of core parameters which impose limits on its operations. Changes to these parameters have their own part of the fund’s governance process.

- **Fund Budget:** The upper limits for (1) the total full value and (2) the total face value of all outstanding rev tokens in the fund, including unissued rev tokens. Once either of these limits are reached, no new rev tokens can be created.
- **Min Multiple:** The lower limit for the multiple property of all rev tokens in the fund. During a token downgrade, no token multiples will be decreased below this limit.
- **Max Multiple Downgrade:** A percentage between 0% and 100% used during a token downgrade to prevent the multiple of any rev token from decreasing more than this amount from its originally issued multiple.

### Investment Fund Rev Token Cohorts

Each rev token in an investment fund is part of a rev token cohort. Each rev token cohort takes a chunk of the remaining fund budget and turns it into three different pools of rev tokens: 

1. **Formal Investment Pool:** Unissued rev tokens ready to be sold to money investors via formal investment rounds.
2. **Informal Investment Pool:** Unissued rev tokens ready to be sold to money investors as part of informal investments as outlined in the fund’s governance process.
3. **Time Investment Pool:** A pool of rev tokens (and a corresponding pool of rev points with quantity equal to the full value of the underlying rev tokens) which are issued right away, but held by Quorum1 with rev token payments being received by the fund’s rev points program. Details defined in the [Rev Points](#rev-points) section.

Each investment fund’s design must include a special section defining the rev token cohorts, including for each:

- **Budget:** The budget for the total full value of all rev tokens in the cohort.
- **Multiple:** All rev tokens issued within a cohort have the same multiple.
    - The multiple will change across cohorts over time to reflect the current perceived risk of investing in the fund. If things are going well the multiple should decrease over time, though it may also need to increase if risks increase.
- **Formal Investment Pool:** How many unissued rev tokens are reserved for formal investment rounds. Along with:
    - **Formal Investment Rounds:** A list of investment rounds, including for each:
        - How many unissued rev tokens are reserved for the investment round.
        - Key roles & responsibilities for managing the round.
        - Fee outlines: Commissions, finders fees, etc.
        - Success and failure criteria for the round.
        - Round failure process including whether money is refunded or re-allocated.
- **Informal Investment Pool:** How many unissued rev tokens are reserved for informal money investment and which members are able to be investors.
- **Time Investment Pool:** How many rev tokens will be issued to the rev point program. This also determines the number of rev points generated by the cohort. One rev point is created for every dollar of full value in this pool of rev tokens. The cohort design should also define:
    - How many rev points are reserved for the fund’s own rev point pool
    - How many rev points will be sent to other fund rev point pools
    - The terms by which the rev points sent to other funds can be reallocated if unawarded (likely a period of time)

### Investment Fund Rev Point Plan

Just like any other fund, an investment fund can have its own rev point plan which specifies how the rev points in its own rev point pool are to be awarded. They will likely be awarded based on activities related to fund raising or administering the fund, but that is just one possibility.

### Investment Fund Allocation Models

The allocation model of an investment fund must define:

- **Formal Investment Targets:** A list of one or more funds which may be targeted by formal money investors
- **Informal Investment Targets:** How informal money investment may be targeted
- **Top-Line Allocations:** Other allocation targets to include when allocating investment income (such as the core fund, a bonus fund for commissions, etc). Each investment round can also include its own top-line allocations.
- **Rev Token Weighting:** Defines the weighting algorithm used to calculate how much each active rev token recipient receives during rev token payment. Details outlined in [Rev Token Payments](#rev-token-payments) section.
- **Rev Point Weighting:** Defines the weighting algorithm used to calculate how much each rev point holder receives during rev point payment. Details outlined in [Rev Point Payments](#rev-point-payments) section.

### Investment Fund Governance Processes

The governance process of an investment fund must define:

- **Core Parameter Governance:** How changes can be made to the fund’s core parameters.
- **Token Downgrade Governance:** When and how a token downgrade process can be run.
- **Cohort Governance:** How rev token cohorts are managed.
- **Investment Round Governance:** How formal investment rounds are managed.
- **Informal Investment Governance:** How informal investments are managed.
- **Allocation Model Governance:** How changes to the allocation model are made.
- **Meta Governance:** How changes to the governance process are made.
- Participatory processes for:
    - **Investment Splitting:** Splitting rev tokens between time and money investment
    - **Time Investment Allocation:** Allocating time investment rev points to specific target funds

### Key Governance Process: Token Downgrade

<aside>
⚠️ Token downgrades are disruptive. They should be used rarely and must be used in good faith and with full transparency.

</aside>

It may become necessary to decrease the return multiple of all outstanding rev tokens in a fund. The fund governance process must define the exact criteria when a downgrade is allowed as well as the process for approving the changes.

For example: A token downgrade might be needed when the revenue growth of the fund inflows has proven to be too slow to reach the fund budget, or when more room for investment is needed without raising the fund budget. 

A token downgrade involves selecting a downgrade factor (a decimal number between zero and one) and changing the multiple property of all outstanding rev tokens by multiplying their originally issued multiple by that downgrade factor. During this process the min multiple and max multiple downgrade core parameters must be respected, meaning that all rev tokens may not decrease by the exact same factor.

**Token upgrades** (increasing the multiples of all outstanding rev tokens in a fund) **are specifically disallowed**. The rationale is that constraining multiples to a single direction of movement (1) makes it easier for investors to predict how rev token values might change and (2) encourages more accurate initial valuation of effort at the outset. This restriction is further justified by the fact that new rev tokens may easily be issued to recognize an increased valuation of past efforts, without requiring the disruption of all multiples.

### Key Governance Process: Failsafe Equity Conversion

As outlined in the [Investment Fund Implementation Details & Risk](#investment-fund-implementation-details--risk) section, in the case that the entire rev token and rev points structure is ultimately deemed to be fundamentally infeasible to implement, each investment fund must include in its governance process design a “failsafe equity conversion” process.

This process should outline steps that will result in issuing traditional equity in Quorum1 or an affiliated legal entity, proportionally based on rev tokens and rev points.

## Rev Tokens

Rev tokens are a type of debt instrument linked to a particular investment fund, similar to a corporate bond with a fixed return multiple but a variable payback rate (and therefore a variable interest rate) and the additional risk of the multiple being downgraded in the future. 

Rev tokens are an owned asset entitling the owner to a portion of the rev share inflows of the linked investment fund until the total payments received reach a certain value. Quorum1 facilitates investment by issuing rev tokens to our investors. 

For money investors, rev tokens are issued in exchange for money. For time investors, rev tokens are instead issued to and held by Quorum1 and used to power a [Rev Points](#rev-points) program.

Rev tokens may be owned by individuals or by other legal entities.

### Rev Token Properties

Below are some of the most important properties of a rev token.

- **Face Value:** The value of the money or time exchanged for the token at time of issuance.
- **Multiple:** The factor applied to the face value to calculate the full value.
- **Full Value:** Equal to the face value times the multiple.
- **Received Value:** The sum total of all payments received by the token to date.
- **Remaining Value:** The amount remaining to be received. Equal to the full value minus the received value.
- **Cliff:** The period of time, post-issuance, before the token begins receiving payments.
- **Status:** Where the token is at in its lifecycle (Unissued, Inactive, Active, Retired).
- **Owner:** The individual or entity which owns the token.
- **Recipient:** The individual or entity which receives payments (usually the owner).

### Rev Token Lifecycle

**Unissued** tokens belong to a specific rev token pool until they are issued. Though we may discuss “how many” unissued tokens exist in a rev token pool, that is just a shorthand for talking about the size of the rev token pool itself. Tokens are not actually individuated at this stage and exist only as a pool of potential tokens with a total max full value. Once a token is issued, it becomes individuated, gains all of the rev token properties outlined above, and then proceeds through the lifecycle outlined below.

An **Inactive** token is still in its cliff period and is not yet receiving payments. Tokens which are issued with no cliff will skip this status and become active immediately upon issuance.

Once a token passes its cliff it becomes **Active** and begins receiving payments.

When a token’s received value reaches its full value it becomes **Retired.** Retired tokens no longer receive payments and may never become active again. A token may also be prematurely retired, only by its owner, as outlined in the [Rev Token Ownership Processes](#rev-token-ownership-processes).

### Rev Token Transfers

The owner of a rev token may sell it or otherwise transfer it to a new owner as outlined in the [Rev Token Ownership Processes](#rev-token-ownership-processes). The transfer process is permanent.

### Rev Token Payments

Rev token payments are received by the rev token recipient on a regular basis. 

Rev token payments pass the rev share inflows which flow into the investment fund through to the rev token recipients of all active rev tokens linked to the fund. Team Finance administers these payments and should seek to increase their frequency over time until they are able to go out on a monthly basis, but it may take some time to reach that frequency. 

Once revenue is flowing into the rev share inflow source funds, at least one rev token payment should be made each year. The goal should be regular payments throughout the year.

Each active rev token receives a payment according to the rev token weighting algorithm defined in the investment fund’s allocation model. The algorithm must not use the rev token owner or recipient as a parameter and must allocate at least some revenue to each active rev token.

The fund managers may optionally decide to deduct an administration percentage from the gross rev share inflows, but the full amount must go directly to helping pay for the administration of the fund and the amount must be no more than 2%.

### Rev Token Implementation & Compliance

The implementation of the rev token system must be legally compliant, technically reliable, auditable, secure, and transparent to members. 

The initial implementation will utilize traditional business systems and tools and the manual effort of the Foundation team.

The v1 implementation will be a key priority for the Foundation and should be a primary focus of investment. The v1 implementation should utilize blockchain technology to streamline the technical operations, improve auditability, and provide greater liquidity.

### Rev Token Downgrades

It is possible for the multiples of rev tokens to decrease (but not increase) over time via the [Key Governance Process: Token Downgrade](#key-governance-process-token-downgrade) of the linked investment fund. This should be a rare event, but a possibility of which all investors should be aware. The precise governance process surrounding token downgrades is defined by the fund’s governance process.

In the event of a token downgrade, all rev token multiples are decreased by the same factor(a decimal number between zero and one) while respecting the core parameters of the investment fund, specifically the min multiple and max multiple downgrade. This may mean that there are slight variances in the effective downgrade factor across rev tokens to protect them from over-downgrading.

## Rev Points

Rev points are a reward mechanism for time investors which allows members to benefit financially from the future success of the quorum without the legal and tax implications of owning an asset. 

Rev points are not assets, but a member entitlement implemented as a simple set of properties associated with each Quorum1 membership. 

Rev points are awarded to time investors for their contributions. In general the number of rev points awarded should be equal to the face value of the time investment multiplied by the rev token cohort’s multiple, but this math may differ when needed.

Things to cover in this section:

### Rev Point Structure

Rev points are linked to an investment fund and are backed by the rev tokens in the fund’s time investment lipool. **One rev point is equal to $1 USD of full value of the rev tokens in the time investment pool.** The total number of rev points linked to an investment fund will always equal the total full value of all the rev tokens in the investment fund’s time investment pool.

Each Quorum1 member has a **rev point balance** for each investment fund. The rev point balance is an integer value indicating the number of rev points held by the member within that investment fund. Each member also has a **transaction history** of all changes made to their rev point balance.

In most cases, a member’s rev point balance goes up when they are awarded new rev points and goes down each time they receive a rev token payment. A full list of possible balance changing events is defined below.

### Rev Point Balance Changes

It is critical to the long-term success of Quorum1 that the rev point structure be safe and reliable. **Rev point balances cannot be changed arbitrarily.**

All new members start with a balance of zero rev points for all investment funds. Each change to a member’s rev point balance is considered a transaction and must be logged in their transaction history.

**Valid Transaction Types:**

Changes in rev point balances are only allowed for the transaction types listed in this sub-section. No other types of rev point balance changes are allowed.

- **Award:** Rev points are awarded to members from the rev point pools of funds according to the funds’ rev point plans.
- **Retraction:** Rev points awarded in error due to administrative errors or data quality problems may be retracted at a later date. Rev points may never be retracted for other reasons.
- **Transfer:** A member may transfer some of their rev points to another member.
- **Payment:** Each rev point payment received by a member reduces their balance, with each $1 USD received reducing the balance by 1 rev point.
- **Downgrade:** In the case of [Rev Point Downgrades](#rev-point-downgrades), all member rev point balances are decreased by the same factor.

### Rev Point Payments

Rev point payments are offered to each rev point holder on a regular basis.

Rev point payments pass the rev token payments received by the rev tokens in the investment fund’s time investment pool through to all holders of rev points linked to the fund. Team Finance administers these payments and should seek to increase their frequency over time until they are able to go out on a monthly basis, but it may take some time to reach that frequency.

Each active and eligible rev point holder is offered a payment according to the rev point weighting algorithm defined in the investment fund’s allocation model. The algorithm must not use the rev point holder’s identity as a parameter and must offer at least some revenue to each active and eligible rev point holder. (Eligibility is defined by the [Member Rev Point Payment Requirements](#member-rev-point-payment-requirements) in the Financial Operations Plan.)

The rev point payment process and rev point weighting algorithm should be designed to allow each rev point holder to opt-in or opt-out of each rev point payment. If a rev point holder opts-out of a particular payment, their rev point balance does not decrease and they should be offered a benefit as a reward for not exercising their liquidity. Some or all of their non-exercised payment should then be made available to increase the rev point payments of other members.

The fund managers may optionally decide to deduct an administration percentage from the gross time investment pool rev token payments powering the rev point program, but the full amount must go directly to helping pay for the administration of the fund and the amount must be no more than 2%.

Aside from the administration percentage, all of the rev token payments received from the time investment pool must eventually go to rev point holders. It is acceptable, however, for portions to be held in reserve in order to support the non-exercising rewards or other programs deemed to benefit the health and sustainability of the overall rev point program.

### Rev Point Rights & Restrictions

Only Quorum1 members may receive rev point payments and members must meet the [Member Rev Point Payment Requirements](#member-rev-point-payment-requirements) defined in the Financial Operations Plan in order to receive payments. 

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
    - Each member may specify another member as their designated beneficiary in the case of their death. Upon a member’s death, their rev point balance is transferred to their designated beneficiary. If no surviving beneficiary is designated, then the rev point balance is transferred to a shared fund for the collective benefit of all members.
    - A member’s balance may be adjusted if Quorum1 is instructed and required to to so by a governmental authority.

### Rev Point Implementation & Compliance

The implementation of the rev token system must be legally compliant, technically reliable, auditable, secure, and transparent to members. It is particularly critical that the rev point implementation be compliant with the spirit and letter of tax regulations such that the awarding of rev points is not a form of income. The regular rev point payments should be structured as taxable independent contractor income.

The initial implementation will utilize traditional business systems and tools and the manual effort of the Foundation team. It is likely, but not mandatory, that the initial implementation will be built using [Workstream Wallets](#workstream-wallets).

The improvement and increased automation of the rev point implementation will be a key priority for the Foundation. There is no immediate plan for utilizing blockchain in the rev point implementation, since liquidity and external audibility are not critical requirements. But the Foundation is free to consider a blockchain-based implementation if it is deemed to be beneficial.

### Rev Point Downgrades

It is possible for the multiples of rev tokens to decrease (but not increase) over time via the [Key Governance Process: Token Downgrade](#key-governance-process-token-downgrade) of the linked investment fund. This should be a rare event, but a possibility of which all investors should be aware. The precise governance process surrounding token downgrades is defined by the fund’s governance process.

In the event of a token downgrade, all member rev point balances are decreased by the same factor while respecting the core parameters of the investment fund, specifically the min multiple and max multiple downgrade. This may mean that there are slight variances in the effective downgrade factor across members to protect them from over-downgrading.

## Org Investment Fund Design Guidelines

The [Org Investment Fund](#org-investment-fund) is the only investment fund mandated by the Financial Model. The [Core Fund](#core-fund) includes a mandatory allocation to the org investment fund, meaning that a share of all Quorum1 revenue will pass through to this fund. This fund is a critical part of Quorum1’s financial infrastructure and key to our long-term sustainability. As such, the design of the org investment fund must meet our highest standard.

The org investment fund design itself is officially considered part of the Financial Operations Plan and is thus changed according to the more streamlined [Change Process for Financial Operations Plan](#change-process-for-financial-operations-plan).

However, the Financial Model does impose some guidelines on the org investment fund design. This section outlines those guidelines. Making changes to any of these guidelines requires modifying this doc in accordance with the [Change Process for Financial Model Definition](#change-process-for-financial-model-definition). 

### Guideline 0 - Launching the Fund

At the time of writing and approving this Financial Model, the org investment fund has yet to be launched. The initial launch should align with the guidelines outlined in this section and should follow the [Standard Process for Designing an Investment Fund](#standard-process-for-designing-an-investment-fund).

### Guideline 1 - Core Parameters

The core parameters must match the following.

- **Fund Budget:** $825M Full Value / $55M Face Value (Average Multiple: 15x)
- **Min Multiple:** 1.0x
- **Max Multiple Downgrade:** 90%

**How to Contextualize the Fund Budget:**

<aside>
🏦 The fund budget above is built around the goal of getting to a billion dollars in revenue in 2034 (with at least 5% of gross revenue going to rev token payments).

</aside>

The precise rev token payment amount in any future year will depend on both the amount of org revenue and the “org rev share allocation” (the net allocation to org investment fund rev token payments as a portion of overall revenue).

The org rev share allocation percentage in a year will be a factor of (1) the average core fund allocation percentage across the blend of revenue sources (refer to [Standard Income Allocations](#standard-income-allocations)) in that year and (2) the average percentage allocated by the [Core Fund](#core-fund) to the [Org Investment Fund](#org-investment-fund) over the year. This means that if the quorum is able to grow higher-margin revenue sources the org rev share allocation will generally increase, but also that the Foundation may impact the the org rev share allocation through the way it manages the core fund allocation model.

### Guideline 2 - Rev Token Cohorts

There will be annual rev token cohorts, with one created for each calendar year and sub-cohorts created for each investment type and rev token pool. 2020 is known as “year 0”, 2021 is known as “year 1”, etc.

The legacy cohorts for years 0 through 3 are listed below and will match these tables exactly, except that the actual face value, which must be under the maximums defined below, will be determined via a participatory process (to be determined by the Foundation) that runs soon after v2 of the Financial Model is initially approved and adopted. 

| Year | Max Face Value | Multiple | Max Full Value |
| --- | --- | --- | --- |
| Year 0 - 2020 ¹ | $100K | 100x | $10M |
| Year 1 - 2021 ² ³ | $300K | 100x | $30M |
| Year 2 - 2022 ² ³ | $600K | 75x | $45M |
| Year 3 - 2023 ² | $600K | 50x | $30M |
| Legacy Total | $1.6M | 71.9x (avg) | $115M |
- ***¹ For year 0:** All of the rev tokens will be issued to the time investment pool and awarded as rev points to the meta founder as a replacement for the originally planned meta-founder entitlement. Full details outlined in [Changes from Legacy Financial Model](#changes-from-legacy-financial-model).*
- ***² For year 1, 2, and 3:** A pass-through fund will be created to manage the retroactive issuance of the rev tokens.*
    - *First any money investments will be collected, documented and the amounts will be taken from the total pool. These cash investments will specifically include the unpaid legal fees to London Law, Inc less any amounts paid on the Initial Counsel Profit Share to date (full details outlined in [Changes from Legacy Financial Model](#changes-from-legacy-financial-model)).*
    - *Then the remaining amount will be available for allocation amongst all individuals who were members during that year via a participatory retroactive valuation process agreed on by at least 60% of the members from that year who remain active and are engaged enough to participate in the decision-making process.*
- ***³ For year 1 and year 2:** Member Q0005 will be awarded 750k rev points in each year (for a total of 1.5M rev points) as a replacement for the originally planned prime founder entitlement. Full details outlined in [Changes from Legacy Financial Model](#changes-from-legacy-financial-model).*

**The first live cohort will be year 4, defined exactly as below (including budget).**

| Year | Face Value | Multiple | Max Full Value |
| --- | --- | --- | --- |
| Year 4 - 2024 ¹ | $4M | 40x | $160M |
| Total from Y0 - Y4 | $5.6M | 49.1x (avg) | $275M |
| Remaining for Y5+ | $49.4M | 11.1x (avg) | $550M |
- ***¹ For year 4:** $1M will be allocated to a formal org investment round managed by the meta founder with all critical parameters requiring the 60% agreement of the partner members.*
    - *Any remaining un-raised amount from that $1M will be available for informal investment.*
    - *With the 60% agreement of the partner members, up to an additional $500K may be used for the investment round in an oversubscribed scenario.*
    - *The remaining $3M (less the investment round oversubscription) will be used for time investment and will be broken into allotments every 3 months or so, which may run into future years if needed. Each allotment will be allocated via a participatory process open at least to all community, contributor and partner members. Each of these allotments will be designed as an experiment intended to learn more about what sorts of participatory processes work best for the quorum.*

**The org investment fund’s governance process will begin determining annual rev token cohorts starting in year 5 (2025).**

### Guideline 3 - Allocation Model

The rev token weighting algorithm for the org investment fund will stay consistent over time to maximize predictability. 

Specifically, during a rev token payment, each active rev token recipient will receive a percentage of the overall rev token payment equal to the total full value of their rev tokens divided by the total full value of all rev tokens. Any left over amount allocated to rev tokens which are fully paid during this round will be split across the remaining active rev tokens in the round. This math will only include rev tokens that are part of the rev token payment.

As an example scenario: Assume in a particular rev token payment there are three rev token recipients: recipient A (with $10,000 of full value), recipient B (with $5,000 of full value), recipient C (with $5,000 of full value). In this scenario, recipient A would receive 50% of the rev token payment, with recipients B and C receiving 25% each.

### Guideline 4 - Governance Process

The org investment fund’s governance process will describe the process for determining annual rev token cohorts, with one created for each calendar year and sub-cohorts created for each investment type and rev token pool.

The process should align with the structure outlined below:

- Annual Process: To run every year, though it does not have to follow the calendar year precisely.
    1. Budgeting: Org & Foundation leaders define the investment budget for the year, which is the total face value, multiple, and total full value of the rev tokens in the year’s annual cohort. (This is the main point at which token downgrading might occur.)
    2. Splitting: A participatory process is used to determine the percentage split of the budget between time investment and money investment. Org & Foundation leaders determine the split between formal money investment and informal money investment.
    3. Allocating: A participatory process is used to allocate time investment rev tokens between funds which seek them.
    4. Planning: Each fund receiving investment creates its design. The designs should ideally involve a quarterly cadence of rev tokens allotments.
    5. Operation: The quarterly processes run throughout the year.
    6. Reporting: Each fund receiving investment reports on results.
- Quarterly Process: To run roughly every quarter, though the governance process can optionally allow greater flexibility. Describes how re-allocation is administered if rev tokens are unissued or rev points are unawarded.

The above process is built around a structure of regular annual investment rounds, with each round striking a balance between time investment and money investment according to the needs of the quorum and based on the market conditions at that time.

### Guideline 5 - Token Downgrade

Token downgrades should happen no more than once per year and should not happen before year 6.

### Guideline 6 - Failsafe Equity Conversion

As outlined in the [Investment Fund Implementation Details & Risk](#investment-fund-implementation-details--risk) section, in the case that the entire rev token and rev points structure is ultimately deemed to be fundamentally infeasible to implement, the org investment fund’s governance process must include details of a failsafe equity conversion process. 

The failsafe process should result in in converting all issued rev tokens and awarded rev options into shares of traditional equity with overall proportions matching each members’ respective full value holdings of rev tokens and rev options. The equity shares should be in Quorum1 or an affiliated legal entity. All equity shares must be in the same legal entity.

### Guideline 7 - Fund Liquidation Preferences

In the event of the full fund liquidation of the org investment fund for any reason, all token holders must convert at the same discount rate, weighting, or liquidation preference.

## Changes from Legacy Financial Model

The legacy financial model (aka Financial Model v1) is the set of agreements which preceded this Financial Model. It included a number of “mandatory revenue disbursements”, outlined in Section 7 of the Operating Agreement, which are being retired and replaced as part of this new design. This section outlines each of the retired structures and what replaces each of them.

The replacement structures are all outlined in the [Guideline 2 - Rev Token Cohorts](#guideline-2---rev-token-cohorts) section.

- **Meta Founder Revenue Share:**
    - **Financial Model v1:** 1% of gross revenue is paid to the meta founder for 20 years from initial incorporation.
    - **Original Intention:** An exchange for the initial thought work and effort that went into conceiving and founding of Quorum1.
    - **Financial Model v2:** This disbursement is removed and replaced by the 2020 rev point cohort issued to the meta founder, valued at $10M rev points ($100k at a 50x multiple).
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

---

# Required Components of Financial Operations Plan

The operational implementation of the **Financial Model** is referred to as the **Financial Operations Plan**. Any details that are not defined in the Financial Model can be defined in the Financial Operations Plan. The Financial Operations Plan is managed more fluidly than the Financial Model itself.

**This section does *not* define the Financial Operations Plan itself**, that will eventually be quite complex and may span many different documents. Rather, this section outlines a set of required components which must be clearly defined in order for the Financial Operations Plan to be considered complete. The actual Financial Operations Plan may include additional components that are not outlined here.

It is important to note that the full Financial Operations Plan will eventually compose a large body of work and, as of this writing, is nowhere near complete. As such, it is understood that certain required components may not be able to be properly and fully defined until the Foundation and Org are able to dedicate the time and resources needed, and that this will happen in an incremental process over time.

In the interim period during which the Financial Operations Plan is incomplete, any undocumented aspects of the plan will be clarified on an ad hoc basis by Team Finance.

## Required Documents

Each item in this section is a document which must eventually be defined as part of the Financial Operations Plan. They must be made available to all members and an audit trail of all changes must be kept. Additionally, any changes must be made in accordance with the [Change Process for Financial Operations Plan](#change-process-for-financial-operations-plan).

### Allocation Model Templates

***Referenced in:** [Allocation Models](#allocation-models)* 

The allocation model templates are a set of standard template docs for each fund type. These templates define the format, structure and options available to fund designers when creating allocation models for a fund.

These must be iterated and improved over time based on member input.

### Receivable Fund Requirements

***Referenced in:** [Income (External Inflows)](#income-external-inflows)* 

This document defines, for each type of fund, the exact requirements for a fund to be able to receive income from outside the quorum. This includes designating which types of funds are not able to receive income.

As an example of the former: a receivable fulfillment fund for a client project may require a signed SOW. An example of the latter: It may be decided that expense funds cannot receive income, that they should instead only have income allocated via pass-through from other funds.

These requirements must ensure that we are being compliant with applicable laws and regulations while also ensuring that the process for setting up new receivable funds is as streamlined as possible.

### Required Income Documentation Checklist

***Referenced in:** [Income Reconciliation](#income-reconciliation)* 

This document defines a standardized checklist of required documentation for each type of income.

For instance, we may require that clients provide us with tax ids or other information before we are able to accept payment from them. Or we may require that money investors provide evidence of accreditation before investing above a certain threshold.

These requirements must ensure that we are being compliant with applicable laws and regulations while also ensuring that the process for receiving income is as streamlined as possible.

### Member Rev Point Payment Requirements

***Referenced in:** [Rev Point Payments](#rev-point-payments), [Rev Point Rights & Restrictions](#rev-point-rights--restrictions)*

***Must align with:** [Rev Point Rights & Restrictions](#rev-point-rights--restrictions)* 

Defines the precise list of requirements for a Quorum1 member to be able to receive rev point payments.

### Standard Income Allocation Table

***Referenced in:** [Standard Income Allocations](#standard-income-allocations)*

***Must align with:** [Standard Income Allocations](#standard-income-allocations)*

The standard income allocation table defines the required percentage of recognized income that must be allocated to the core fund for each type of income based on various parameters, including whether the income is associated with a hosted entity and whether it uses the Quorum1 brand. 

The standard income allocation table should match the basic format outlined in the [Standard Income Allocations](#standard-income-allocations) section. The actual values may differ, however. And the actual format may also differ slightly as long as it aligns with the spirit of this design.

### Org Investment Fund Design

***Referenced in:** [Org Investment Fund](#org-investment-fund), [Org Investment Fund Design Guidelines](#org-investment-fund-design-guidelines)* 

***Must align with:** [Org Investment Fund Design Guidelines](#org-investment-fund-design-guidelines)* 

The org investment fund design defines all of the properties of the org investment fund, as outlined in [Investment Funds Detail](#investment-funds-detail) section. It must meet all guidelines outlined in [Org Investment Fund Design Guidelines](#org-investment-fund-design-guidelines).

## Required Process Definitions

### Change Process for Financial Model Definition

***Referenced in:** [Governance](#governance), [Org Investment Fund Design Guidelines](#org-investment-fund-design-guidelines)*

This defines the governance process for making changes to this document. 

Making changes to the Financial Model should be considered a formal process requiring a high-level of confidence in the quality of the changes being made. The Financial Model will need to evolve as we learn more about what works and what doesn’t. It is, however, important that the Financial Model maintain a level of stability due to its importance and the potential negative impact of improperly considered changes.

Until this process is formally documented, making changes to this document should require the 75% approval of Quorum1 partner members (allowing for partners to appoint another partner as a proxy as needed).

### Change Process for Financial Operations Plan

***Referenced in:** [Governance](#governance), [Standard Funds](#standard-funds), [Org Investment Fund Design Guidelines](#org-investment-fund-design-guidelines), [Required Documents](#required-documents)*

This defines the governance process for making changes to the Financial Operations Plan which is the set of documents defining the operational implementation of the Financial Model. 

This is a critical governance process because the Financial Operations Plan will eventually be composed of a large, complex, wide-ranging set of documents which will be iteratively created and improved over time. As such it is important that we allow for fluidity and agility as we work to learn what works and what doesn’t.

Until this process is formally documented, making changes or additions to the Financial Operations Plan should require the written agreement of the Foundation Leadership. The members included in the Foundation Leadership are appointed by the Managing Partners and must be clearly documented. Each change or addition to the Financial Operations Plan must be documented and explained in a central repository of changes which is visible to all contributor and partner members.

### Fund Management Process

***Referenced in:** [Funds](#funds)* 

This process must define workflows for creating new funds, making changes to existing funds, retiring funds, and administering the ongoing operations of funds.

It is important that fund management be as streamlined as possible, while also ensuring that the overall fund structure is operationally reliable and administration is secure, accurate, and compliant.

### Vendor Registration Process

***Referenced in:** [Vendor Company Outflows](#vendor-company-outflows)*

This process defines how new vendors are registered and onboarded so that they may be targeted by outflows.

### Hosted Entity Management Process

***Referenced in:** [Hosted Entities](#hosted-entities)* 

This process defines workflows for managing hosted entities. This includes creating new hosted entities, making changes to existing hosted entities, retiring hosted entities, and spinning hosted entities out into separate companies.

### Recurring Expense Management Process

***Referenced in:** [Expense Funds](#expense-funds)*

This process defines how recurring expenses within expense funds are managed. It is important that we closely manage these types of expenses so that we’re balancing the outgoing expenses with expected income, and so that any potential shortfalls can be identified and mitigated well ahead of time.

### Expense Reimbursement Process

***Referenced in:** [Expense Funds](#expense-funds)*

This process defines how expense reimbursement requests are submitted by members, and then either approved or denied by the fund managers of an expense fund. Due to our collective structure and focus on ethical financial structures, and due to the potential risk of misappropriation involved in expense reimbursement, it is critical that this process meet our highest standards of transparency and accountability.

### Debit Card Management Process

***Referenced in:** [Expense Funds](#expense-funds)*

This process defines how debit cards linked to expense funds are managed. This includes workflows for allowing the fund managers to request new debit cards, the Foundation responding to those requests, creating and retiring cards, setting and changing limits, and other workflows as needed.

This process must also include appropriate training and verification for debit card holders to ensure that they are aware of best practices for managing these debit cards and how to mitigate potential fraud or theft risks. 

The Foundation may opt to impose security requirements on debit card holders to prevent potential fraud or theft.

### Investment Fund Management Process

***Referenced in:** [Investment Funds Detail](#investment-funds-detail), [Standard Process for Designing an Investment Fund](#standard-process-for-designing-an-investment-fund)*

***Must align with:** [Standard Process for Designing an Investment Fund](#standard-process-for-designing-an-investment-fund)*

This process defines how investment funds are created, changed, retired, and operationally managed.

### Investor Management Process

***Referenced in:** [Money Investment](#money-investment), [Investment Fund Inflows & Outflows](#investment-fund-inflows--outflows)*

This process defines how money investors are onboarded, off-boarded, what required documentation is needed, and other details necessary to manage the money investors.

### Member Payment Eligibility Process

***Referenced in:** [Member Outflows](#member-outflows)* 

This process is important to ensure that the quorum has collected appropriate financial information and ensured that we are not restricted from sending a particular member money for some reason.

In order for a fund to directly target a member for outflow allocation, the member has to have signed a formal agreement with Quorum1. If members have joined the quorum via a corporate entity, then their payments are directed to their registered corporate entity. Some members may be restricted from direct allocation if there are legal or regulatory restrictions that apply to them.

### Rev Token Ownership Processes

***Referenced in:** [Rev Token Lifecycle](#rev-token-lifecycle), [Rev Token Transfers](#rev-token-transfers)*

This process defines how rev tokens are purchased, issued, and managed by the owner. It also defines all key workflows needed to support the ongoing management of rev tokens. It must include workflows for updating the rev token’s recipient, for splitting the rev token into multiple rev tokens, and for transferring ownership (as part of either a gift or a sale). It must also include a workflow for retiring a rev token.

This process may optionally define a slightly different process for Quorum1-owned rev tokens.

### Refund Process

***Referenced in:** [Fulfillment, Recognition, & Refunds](#fulfillment,-recognition,--refunds)* 

This process defines how unfulfilled revenue in a fulfillment fund may be refunded back to its source (such as back to an external client or back to another internal fund). 

---

# Appendix

## Term Definitions

### Workstream

The Workstream is a system that Quorum1 uses to manage requests, tasks, and facilitate collaboration. Workstream reqs (short for “requests”) are discrete work units or tasks. Each req belongs to a stream (the primary organizational structure within the Workstream). The Workstream is a custom app designed and built by the quorum to facilitate collaboration \while maximizing visibility and discoverability of work items across the organization. The Workstream is a critical part of Quorum1’s operational infrastructure.

### Workstream Wallets

***Referenced in:** [Allocation Models](#allocation-models), [Foundation Operations Fund](#foundation-operations-fund), [Income Types](#income-types), [Standard Income Allocations](#standard-income-allocations), [Workstream Wallet Outflows](#workstream-wallet-outflows), [Rev Point Implementation & Compliance](#rev-point-implementation--compliance)* 

As of this writing, the [Workstream](#workstream) does not yet have Workstream Wallet functionality. This sub-section describes the planned future functionality.

Each quorum member will have a personal wallet and shared wallets will be able to be created linked to quorums or other groups. Each wallet will have a cash balance (initially denominated in USD) and a rev point balance for each investment fund. 

Members will be able to load cash into and withdraw cash out of their personal wallets. Withdrawals will be subject to appropriate taxes, such as income tax, and categorized as independent contractor income.

Members will also be able to add cash and rev points from their personal or shared wallets to Workstream reqs (targeted at the runner, reviewer, or creator), in a manner similar to Workstream bounties. Once this happens the req is described as becoming a “compensated” req. The corresponding cash and rev points are deducted from their source wallets upon being added as req compensation. 

A compensated req requires extra verification before completion. If the req is canceled, the cash and rev points are refunded to their source wallets. If the req is completed, the cash and rev points are transferred to the wallets of the runner, reviewer, and/or creator.

### Time Tracking System

***Referenced in:** [Fulfillment Funds](#fulfillment-funds)* 

Our time tracking system is a critical part of the quorum’s operational infrastructure. At this time of this writing we are using a system called Xero to facilitate time tracking, but that may change in the future.

Regardless of the implementation, the time tracking system is a key tool which allows all members to track time which they spend working on internal and external projects, as well as time they spend in ways which are related to the quorum but not necessarily linked to specific projects.

Our time tracking system is maintained by the Foundation.

---

## Financial Model v2 Implementation

**This section is intended to clarify and explain only and will not be considered binding guidance on the Financial Model or the Financial Operations Plan.** Certain details outlined below may be changed in the actual implementation without making and approving changes to this section.

This section is not intended to be a comprehensive project plan, but rather a summary of the various work areas and steps involved in fully implementing the Financial Model v2. It is assumed that, with adequate funding, most of the core aspects of the Financial Model v2 can be at least partially implemented by the end of 2024, with the remaining aspects implemented by the end of 2025. It is further assumed that the Financial Model will continue to iterate during this process as we discover what works and what doesn’t.

Each of the work areas listed below has its own set of phases which are not directly linked. There are dependencies between some of these items which are not fully detailed here.

- **Bookkeeping, Time Tracking, Xero & Gusto**
    - **Phase 1 - Streamlining:** Also known as the “Financial Model v1.5” project (already underway as of this writing), this work establishes clear weekly and monthly workflows for recognizing income, linking it to accounts in Xero, processing tracked time, determining outflows, and generating detailed member summaries, and then transmitting payments via Gusto. This phase also focuses on increasing the overall bandwidth and capability of manual human bookkeeping effort we have available to support our financial processes.
    - **Phase 2 - Standard Fund Transition:** While keeping the core (v1.5) processes largely the same, this phase would refactor them to be built around the [Standard Funds](#standard-funds). It would also focus on beginning to transition client projects into [Fulfillment Funds](#fulfillment-funds). Critically, it would include configuring our bookkeeping processes to be able to keep track of fund balances (likely as “accounts” in Xero).
    - **Phase 3 - Custom Fund Support:** This phase would add support for operating an arbitrary set of interconnected custom funds, including support for all [Fund Types](#fund-types). It would have interdependencies with the “Fund Management” work area.
    - **Phase 4 - Automation:** This phase would focus on streamlining the workflows built our in previous phases, automating manual processes, and improving process KPIs.
- **Fund Management & Financial Operations (Fin Ops) Plan**
    - **Phase 1 - Standard Fund Design & Fin Ops Beta:** This phase would focus on building out a fund design database (likely in Notion) for managing the fund designs and keeping an audit trail of all changes. It would then work to populate that database with the initial designs for the [Standard Funds](#standard-funds). It would also focus on landing draft versions of the most important parts of the [Required Components of Financial Operations Plan](#required-components-of-financial-operations-plan).
    - **Phase 2 - Custom Fund Beta & Fin Ops v1:** This phase would land finished versions of everything in the [Required Components of Financial Operations Plan](#required-components-of-financial-operations-plan) along with any additional components which arise. It would also begin beta testing the process for letting members design and launch custom funds, testing it by focusing only on the “back-population” of custom funds for existing lines of business, quorums, and virtual companies. It would specifically not focus on creating new investment funds yet.
    - **Phase 3 - Custom Fund v1 & Investment Fund Beta:** This phase would focus on opening up the custom fund creation process to new funds and streamlining the fund management process. It would also focus on beta testing the process for creating new investment funds, which would have interdependencies with the “Legal Work” work area.
    - **Phase 4 - Investment Fund v1 & Streamlining:** This phase would focus additional streamlining and automation for all fund management processes. It would also work to launch the investment fund creation process more widely.
- **Workstream Wallets**
    - **Phase 1 - Q1 App Suite:** As of this writing, this phase is already underway. It is focused on launching the “Quorum1 App Suite”, a technology stack which allows us to have a “network” membership tier and a Quorum1 online account linked to a suite of apps.
    - **Phase 2 - Individual Wallets:** This phase would focus on enabling individual cash wallets within the Q1 app suite, letting members load money in, pull money out, and attach cash to workstream reqs. It would implement an improved req review process to ensure that req funders are able to do a final review before cash is released.
    - **Phase 3 - Shared Wallets:** This phase would add the ability to created and managed shared wallets. It would have interdependency with the bookkeeping work area with regard to supporting shared wallets as outflow allocation targets.
- **Rev Tokens & Rev Token Payments**
    - **Phase 1 - First Fund Raise:** This phase is already underway as of this writing and is focused on the “minimum viable product” implementation of the rev token structure needed to raise investment. It will also set the groundwork for running the the first rounds of rev token payments via a manual spreadsheet-based process.
    - **Phase 2 - Formal Implementation:** This phase would focus on launching the likely blockchain-based final implementation of rev tokens. It would culminate with all existing money investors being issued new rev tokens. It would likely stick with a manual spreadsheet-based process for managing rev token payments, but would begin the process of automating the payouts themselves (either utilizing blockchain or more traditional means or perhaps accommodating a mix).
    - **Phase 3 - Streamlining & Automation:** This phase would focus on streamlining and automating as many aspects of the rev token management and payment process as possible.
- **Rev Points & Rev Point Payments**
    - **Phase 1 - First Fund Raise:** This phase is already underway as of this writing and is focused on the “minimum viable product” implementation of the rev point structure needed to raise investment. It will also set the groundwork for running the the first rounds of rev point payments via a manual spreadsheet-based process.
    - **Phase 2 - Q1 App Suite Implementation:** This phase would attached to the “Workstream Wallet” work area and would focus on adding rev point balances to member accounts within the Quorum1 app suite. The rev point payments themselves would still run via the manual process, but members would be able to see and manage their balances via an app. Members would also be able to link rev points to reqs.
    - **Phase 3 - Streamlining & Automation:** This phase would focus on improving the app implementation of rev points and on fully automating as many parts of the rev point payment process as possible.
- **Legal Work**
    - **Phase 1 - First Fund Raise:** This phase is already underway as of this writing and is focused on the “minimum viable product” implementation of the rev token and rev point structures needed to raise investment.
    - **Phase 2 - Formalizing Rev Tokens & Rev Points:** This phase would be interrelated with the rev token and rev point work areas above. It would focus on formalizing the legal and compliance aspects of these two key structures.
    - **Phase 3 - Hosted Entities & Custom Investment Funds:** This phase would focus on implementing a nested legal structure (such as series LLCs) to support hosted entities which need greater separation around liability, ownership, and the like. It would also focus on laying the legal and compliance groundwork for launching additional investment funds.
    - **Phase 4 - Formalizing Governance:** This phase is not strictly related to the Financial Model, but is important. It would likely begin much earlier and in parallel with the other phases. It would focus on gradually formalizing more aspects of our governance, including the funds, fin ops plan, and Financial Model.

---

## Scenario Walkthroughs

This section includes some explanatory walkthroughs of key scenarios along with links to the relevant parts of the Financial Model document above.

**These walkthroughs are intended to clarify and explain only and will not be considered binding guidance on the Financial Model or the Financial Operations Plan.** Certain details outlined below may be changed in the actual implementation without making and approving changes to this section.

### Scenario Walkthrough: New Line of Business Fund Structure

For this example, a new line of business (LOB) is starting up focused on providing consulting services to manufacturers of widgets. They’ll be called the “Widget LOB”.

1. **Group Formation**: First the Widget LOB assembles a team of members interested in collaborating to generate revenue. They agree that they are going to collaborate to come up with service offerings, branding, and marketing efforts to drive paid consulting projects with widget companies.
    1. They agree roughly on how they want to organize as a group, including ideally who will be the initial leaders of the group. 
    2. They’re able to pull from Quorum1’s library of organizing structures or they can create their own. 
    3. For this example: They decide to have a triad of three leaders, a group of contributors and some supporters, each with different commitment expectations.
2. **Decision-Making Process**: The Widget LOB agrees on a governance structure they’ll use to make decisions together, but also specifically to approve and then modify their LOB’s fund design. 
    1. This structure can be simple or complex. They can pick from a library of governance design options or create their own. 
    2. For this example: They decide to start simple. They will require unanimous consent of the triad to make changes to the fund design and that significant changes must be presented to the full group for feedback first. They also decide to vote on triad members every 6 months using a liquid democracy model provided by the quorum.
3. **Fund Structure Design**: The Widget LOB then proceeds to design their “fund structure”, a set of multiple funds which piece together to provide the financial infrastructure they’re envisioning. This process is led by their triad via a series of meetings inviting input from all LOB members. For this example, they eventually come up with a structure of the following funds:
    1. As with all LOBs, each individual client project will have it’s own **project fulfillment fund** (see [Fulfillment Funds](#fulfillment-funds)).
        1. Per the [Standard Income Allocations](#standard-income-allocations), because their LOB is operating under the Quorum1 brand to start, it will allocate 15% of gross revenue to the core fund.
        2. They decide that an additional 10% of client project revenue will be allocated to their main LOB fund, to incentivize sales and reinvest in driving more business.
        3. This means that they must have a margin of 25% on all of their project work. So, for instance, if a client project member were to want to make $150 per hour, the bill rate would need to be $200 per hour.
    2. The **Widget LOB Main Fund** will be a pass-through fund which allocates a portion of its income to each of the remaining funds. (See [Pass-Through Funds](#pass-through-funds))
    3. The **Widget LOB Bonus Fund** will receive 30% from the main fund and will pay out commissions to members who helped to bring in each lead and close each deal. The Widget LOB comes up with what they think is a fairly simple point system they’ll use to determine how much each person received: 1 point for the original lead, 2 for the qualification call, etc. (See [Bonus Funds](#bonus-funds))
    4. The **Widget LOB Expense Fund** will receive 10% from the main fund and be used to pay for vendor expenses like a series of LinkedIn and Google ad programs the group is planning on running. (See [Expense Funds](#expense-funds))
    5. A **Widget LOB Workstream Wallet** will receive 30% from the main fund, will be managed by the triad, and will be used to add cash to workstream reqs for various tasks that the group comes up with. These tasks could be content-creation-focused, such as creating ads, blog posts, or landing pages. Or they could be business development or sales activities, or anything else the group comes up with. (See [Workstream Wallets](#workstream-wallets))
    6. A **Widget LOB Collaborative Fund** will receive 30% from the main fund and will gather money to reinvest in project initiatives. (See [Collaborative Funds](#collaborative-funds))
        1. As with most collaborative funds, once enough money pools up the group will run a collaborative process where LOB members come up with pitches for potential projects and then vote on which receive funding.
        2. Some potential project ideas might include: Sponsoring a booth at a conference, investing in paid outbound sales, or building out a complex but potentially profitable hybrid product-service offering.
        3. Each funded project will get its own **project fulfillment fund**, with a budget and members and cost rates, just like a client project except that the margin will be 0%. (See [Fulfillment Funds](#fulfillment-funds))
4. **Fund Launch:** With the fund structure design in hand, the Widget LOB works with the Foundation to get their new funds launched! They follow the workflow outlined in the [Fund Management Process](#fund-management-process).
    1. Team Finance reviews their fund designs and works with them to make sure everything is possible to implement. 
    2. In some cases Team Finance might suggest changes to the fund designs (for instance, simplifying the logic used in the bonus fund so that it’s easier to implement), working with the triad to get their approval (in accordance with the governance process defined by the LOB members).
    3. In other cases Team Finance might work with Team Ops and/or Team Build to add functionality to the base platform in order to better support the Widget LOB’s vision.
    4. As part of launching the funds, all of the funds are setup in our bookkeeping system as virtual accounts. The expense fund is created as an actual “virtual” bank account within our Relay bank account, with its own routing number and debit card(s). The triad is given the ability to manage these accounts themselves.
5. **Fund Operation:** As money flows into the fund, Team Finance handles the bookkeeping and delivers weekly reports to the LOB on their various fund balances and transactions. Any errors or issues can be reported to Team Finance and they work to promptly resolve them.
6. **Rev Points:** Going forward, the Widget LOB Main Fund may also receive [Rev Points](#rev-points) from the [Org Investment Fund](#org-investment-fund) that the LOB can use as an additional form of compensation. 
    1. For instance, they could move some rev points to their workstream wallet and link them to reqs.
    2. Or they could allocate them to project funds and specify a certain number of rev points per hour in addition to project member cash compensation.
    3. Or they could direct some rev points to the bonus fund and incorporate them into their bonus structure.
    4. Whatever the LOB decides to do with its rev points, they have a high degree of autonomy in their decision-making. However, if they do not do anything with the rev points they may be “reallocated” to other groups after a certain period of time (see [Rev Point Pools & Plans](#rev-point-pools--plans)).

### Scenario Walkthrough: Client Consulting Revenue Flow

This scenario walks through how revenue from a consulting project with Acme Corp, led by contributor member Jane Lee, flows through the quorum and then back out to project members and investors.

1. **Scoping the Deal:** After discussing the project with Acme, Jane built a cost model using one of a wide variety of templates provided by the Foundation. 
    1. She design the project to be billed hourly. 
    2. The project has three members, two will make $120 per hour, the other is Jane herself, making $150 per hour. These are the “cost rates”. She determined them by searching for qualified members whose rates were within a margin she knew would work for the client’s budget.
    3. Per the [Standard Income Allocations](#standard-income-allocations) she will need to ensure that 20% of the margin goes to the core fund. She decides to add on an additional “top-line allocation” of 10% to herself as a commission for bringing in the deal.
    4. This means that she needs a margin of 30% on everyone’s time (including her own). That means that the two project members will be billed at ~$172 per hour, and the third (herself) ~$215. These are the “bill rates” and they are calculated by working backwards to achieve a gross margin of 30%: for example, $120 / 70% = $171.4 or about $172.
    5. The project is designed with a budget of $15,000 and an initial deposit of $5,000 invoiced at signing. The client is to be invoiced monthly for the hours worked in each month, with the deposit being credited towards the final invoice.
2. **Closing the Deal:** A new client project is brought in by Jane Lee from her personal network.
    1. The deal is closed when Acme Corp signs a master services agreement (MSA) with an attached statement of work (SOW). 
    2. Upon contract signing, Team Finance creates a new **project fulfillment fund** for the project and invoices Acme for the deposit amount of $5,000 specified in the SOW. (See [Fulfillment Funds](#fulfillment-funds)).
    3. When that deposit is received it is credited to the **project fulfillment fund** but the revenue is not yet recognized since the work hasn’t yet been performed.
3. **Doing the Work:** As the project members perform the work, they track their time in our [Time Tracking System](#time-tracking-system).
    1. Team Finance & Team Ops run a weekly process for the **project fulfillment fund** which tabulates the hours worked by each project member and how much money is left in the overall budget. This process also determines how much money each project member is due to earn from their work that week, including the 10% commissions top-line allocation to Jane Lee.
    2. Each week the project members receive statements of their earnings (Jane’s statement includes her commissions and her hourly earnings) and the project lead (Jane Lee) receives an overall budget progress statement.
    3. During this process, Team Finance also begin to pay out the project members each week, until the initial deposit amount is depleted. Once the deposit amount is depleted, project member earnings statements will continue to be generated but they won’t be paid until more funds are received.
    4. Each time that project member payments are processed, that revenue is officially “recognized”. The 20% top-line allocation to the core fund is also processed then, but only on that specific payment amount, to ensure that money does not flow into downstream funds until it is recognized. That is explained more below.
4. **Core Fund Allocation:** Each time project revenue is recognized (aka “fulfilled”), 20% is allocated to the core fund.
    1. For example if in the first week, there was $3,000 of total fulfilled revenue then 20% or $600 will be allocated to the [Core Fund](#core-fund) .
    2. From there the core fund must allocate a portion to each of the other [Standard Funds](#standard-funds), the precise split is defined in the core fund allocation model, which is part of the Financial Operations Plan and managed by the Foundation.
5. **Investor Rev Share:**
    1. There are 6 other standard funds which will receive a portion of the $600 allocated to the core fund in the prior step. 
    2. But in this example we’ll trace the path back out to investors. So for that we care about the portion that goes to the [Org Investment Fund](#org-investment-fund). For this example let’s say that the core fund allocation model specifies that 20% goes to the org investment fund. This means that $120 goes to the org investment fund as a rev share inflow. (See [Investment Fund Inflows & Outflows](#investment-fund-inflows--outflows))
    3. That $120 and all of the other rev share inflows then pile up over in the org investment fund, waiting for the next round of [Rev Token Payments](#rev-token-payments) (which by this point are happening on a monthly basis).
    4. When the next monthly rev token payment happens, for this example let’s say that there is a total of $10,000 which has piled up and is ready to be paid out. This is done by using the rev token weighting algorithm (which for the org investment fund is an equal proportion to each based on their respective full values).
    5. If there happened to be 10 active rev token recipients, each with an equal full value of rev tokens, that would yield each of them getting 10% or $1,000 in rev token payments that month. 
    6. The received value of each rev token would increase by the amount it received, decreasing its remaining full value by that amount.

---

That’s it! This is the end of the document. You made it. 🙂
