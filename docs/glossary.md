# Gov Repo Glossary

This doc serves as a linking layer between different docs in this repo and potentially other repos or external sources. Refer to the [Quorum1 Governance Repo Standards](../standards.md) doc for more guidance around the usage of the glossary.

# Financial Model

The Quorum1 Financial Model ("Financial Model" for short) defines how we manage money as a collective. It is currently in "V2". The prior version was called "V1" and is now referred to as the "Legacy Financial Model".

The Financial Model is part of the gov repo: [/docs/financial-model.md](./financial-model.md)

## Org Investment Ledger Design

The Org Investment Ledger Design defines all of the properties of the org investment ledger, as required by the Financial Model.

The Org Investment Ledger Design is part of the gov repo: [/docs/org-investment-ledger-design.md](./org-investment-ledger-design.md)

## Time-vs-Money Split Rate

The time-vs-money split rate (TVMSR) for an investment ledger may change from payment to payment as needed. The updates must comply with the time-vs-money split rate guidelines defined in the investment ledger design.

The TVMSR process exists to (1) provide a tool for creating parity between time and money investors and (2) ensure that a large amount of investment of one type does not impact the repayment schedule of investors of the other type.

# Financial Operations Plan

The operational implementation of the [Financial Model](#financial-model) is referred to as the Financial Operations Plan. Any details that are not defined in the Financial Model can be defined in the Financial Operations Plan. The Financial Operations Plan is managed more fluidly than the Financial Model itself.

At this time, the Financial Operations Plan is not fully defined in an readily accessible format. In the interim period during which the Financial Operations Plan is incomplete, any undocumented aspects of the plan will be clarified on an ad hoc basis by Team Finance.

This section contains specific definitions which will eventually be defined in the Financial Operations Plan.

Once the Financial Operations Plan is more formally defined, this section will be updated accordingly.

## Allocation Model Templates

The allocation model templates are a set of standard template docs for each ledger type. These templates define the format, structure and options available to ledger designers when creating allocation models for a ledger.

## Receivable Ledger Requirements

This doc defines, for each type of ledger, the exact requirements for a ledger to be able to receive income from outside the quorum. This includes designating which types of ledgers are not able to receive income.

As an example of the former: a receivable fulfillment ledger for a client project may require a signed SOW. An example of the latter: It may be decided that expense ledgers cannot receive income, that they should instead only have income allocated via pass-through from other ledgers.

These requirements must ensure that we are being compliant with applicable laws and regulations while also ensuring that the process for setting up new receivable ledgers is as streamlined as possible.

## Required Income Documentation Checklist

This doc defines a standardized checklist of required documentation for each type of income.

For instance, we may require that clients provide us with tax ids or other information before we are able to accept payment from them. Or we may require that money investors provide evidence of accreditation before investing above a certain threshold.

These requirements must ensure that we are being compliant with applicable laws and regulations while also ensuring that the process for receiving income is as streamlined as possible.

## Member Rev Point Payment Requirements

*Must align with the rev point rights & restrictions defined in the [Financial Model](#financial-model).*

Defines the precise list of requirements for a Quorum1 member to be able to receive rev point payments.

## Standard Income Allocation Table

The standard income allocation table defines the required percentage of recognized income that must be allocated to the core ledger for each type of income based on various parameters, including whether the income is associated with a hosted entity and whether it uses the Quorum1 brand. 

## Ledger Management Process

This process must define workflows for creating new ledgers, making changes to existing ledgers, retiring ledgers, and administering the ongoing operations of ledgers.

It is important that ledger management be as streamlined as possible, while also ensuring that the overall ledger structure is operationally reliable and administration is secure, accurate, and compliant.

## Vendor Registration Process

This process defines how new vendors are registered and onboarded so that they may be targeted by outflows.

## Recurring Expense Management Process

This process defines how recurring expenses within expense ledgers are managed. It is important that we closely manage these types of expenses so that we’re balancing the outgoing expenses with expected income, and so that any potential shortfalls can be identified and mitigated well ahead of time.

## Expense Reimbursement Process

This process defines how expense reimbursement requests are submitted by members, and then either approved or denied by the ledger managers of an expense ledger. Due to our collective structure and focus on ethical financial structures, and due to the potential risk of misappropriation involved in expense reimbursement, it is critical that this process meet our highest standards of transparency and accountability.

## Debit Card Management Process

This process defines how debit cards linked to expense ledgers are managed. This includes workflows for allowing the ledger managers to request new debit cards, the Foundation responding to those requests, creating and retiring cards, setting and changing limits, and other workflows as needed.

This process must also include appropriate training and verification for debit card holders to ensure that they are aware of best practices for managing these debit cards and how to mitigate potential fraud or theft risks. 

The Foundation may opt to impose security requirements on debit card holders to prevent potential fraud or theft.

## Investment Ledger Management Process

This process defines how investment ledgers are created, changed, retired, and operationally managed.

## Investor Management Process

This process defines how money investors are onboarded, off-boarded, what required documentation is needed, and other details necessary to manage the money investors.

## Member Payment Eligibility Process

This process is important to ensure that the quorum has collected appropriate financial information and ensured that we are not restricted from sending a particular member money for some reason.

In order for a ledger to directly target a member for outflow allocation, the member has to have signed a formal agreement with Quorum1. If members have joined the quorum via a corporate entity, then their payments are directed to their registered corporate entity. Some members may be restricted from direct allocation if there are legal or regulatory restrictions that apply to them.

## Rev Token Ownership Processes

This process defines how rev tokens are purchased, issued, and managed by the owner. It also defines all key workflows needed to support the ongoing management of rev tokens. It must include workflows for updating the rev token’s recipient, for splitting the rev token into multiple rev tokens, and for transferring ownership (as part of either a gift or a sale). It must also include a workflow for retiring a rev token.

This process may optionally define a slightly different process for Quorum1-owned rev tokens.

## Refund Process

This process defines how unfulfilled revenue in a fulfillment ledger may be refunded back to its source (such as back to an external client or back to another internal ledger). 

---

# Quorum1 Tools & Terms

## Workstream

The Workstream is a system that Quorum1 uses to manage requests, tasks, and facilitate collaboration. Workstream reqs (short for “requests”) are discrete work units or tasks. Each req belongs to a stream (the primary organizational structure within the Workstream). The Workstream is a custom app designed and built by the quorum to facilitate collaboration \while maximizing visibility and discoverability of work items across the organization. The Workstream is a critical part of Quorum1’s operational infrastructure.

## Workstream Wallets

As of this writing, the [Workstream](#workstream) does not yet have Workstream Wallet functionality. This sub-section describes the planned future functionality.

Each quorum member will have a personal wallet and shared wallets will be able to be created linked to quorums or other groups. Each wallet will have a cash balance (initially denominated in USD) and a rev point balance for each investment ledger. 

Members will be able to load cash into and withdraw cash out of their personal wallets. Withdrawals will be subject to appropriate taxes, such as income tax, and categorized as independent contractor income.

Members will also be able to add cash and rev points from their personal or shared wallets to Workstream reqs (targeted at the runner, reviewer, or creator), in a manner similar to Workstream bounties. Once this happens the req is described as becoming a “compensated” req. The corresponding cash and rev points are deducted from their source wallets upon being added as req compensation. 

A compensated req requires extra verification before completion. If the req is canceled, the cash and rev points are refunded to their source wallets. If the req is completed, the cash and rev points are transferred to the wallets of the runner, reviewer, and/or creator.

## Time Tracking System

Our time tracking system is a critical part of the quorum’s operational infrastructure. At this time of this writing we are using a system called Xero to facilitate time tracking, but that may change in the future.

Regardless of the implementation, the time tracking system is a key tool which allows all members to track time which they spend working on internal and external projects, as well as time they spend in ways which are related to the quorum but not necessarily linked to specific projects.

Our time tracking system is maintained by the Foundation.
