# Gov Repo Glossary

This doc serves as a linking layer between different docs in this repo and potentially other repos or external sources.

# Financial Operations Plan

The operational implementation of the **Financial Model** is referred to as the **Financial Operations Plan**. Any details that are not defined in the Financial Model can be defined in the Financial Operations Plan. The Financial Operations Plan is managed more fluidly than the Financial Model itself.

**This section does *not* define the Financial Operations Plan itself**, that will eventually be quite complex and may span many different documents. Rather, this section outlines a set of required components which must be clearly defined in order for the Financial Operations Plan to be considered complete. The actual Financial Operations Plan may include additional components that are not outlined here.

It is important to note that the full Financial Operations Plan will eventually compose a large body of work and, as of this writing, is nowhere near complete. As such, it is understood that certain required components may not be able to be properly and fully defined until the Foundation and Org are able to dedicate the time and resources needed, and that this will happen in an incremental process over time.

In the interim period during which the Financial Operations Plan is incomplete, any undocumented aspects of the plan will be clarified on an ad hoc basis by Team Finance.

## Required Documents

Each item in this section is a document which must eventually be defined as part of the Financial Operations Plan. They must be made available to all members and an audit trail of all changes must be kept. Additionally, any changes must be made in accordance with the [Change Process for Financial Operations Plan](#change-process-for-financial-operations-plan).

### Allocation Model Templates

***Referenced in:** [Allocation Models](#allocation-models)* 

The allocation model templates are a set of standard template docs for each ledger type. These templates define the format, structure and options available to ledger designers when creating allocation models for a ledger.

These must be iterated and improved over time based on member input.

### Receivable Ledger Requirements

***Referenced in:** [Income (External Inflows)](#income-external-inflows)* 

This document defines, for each type of ledger, the exact requirements for a ledger to be able to receive income from outside the quorum. This includes designating which types of ledgers are not able to receive income.

As an example of the former: a receivable fulfillment ledger for a client project may require a signed SOW. An example of the latter: It may be decided that expense ledgers cannot receive income, that they should instead only have income allocated via pass-through from other ledgers.

These requirements must ensure that we are being compliant with applicable laws and regulations while also ensuring that the process for setting up new receivable ledgers is as streamlined as possible.

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

The standard income allocation table defines the required percentage of recognized income that must be allocated to the core ledger for each type of income based on various parameters, including whether the income is associated with a hosted entity and whether it uses the Quorum1 brand. 

The standard income allocation table should match the basic format outlined in the [Standard Income Allocations](#standard-income-allocations) section. The actual values may differ, however. And the actual format may also differ slightly as long as it aligns with the spirit of this design.

### Org Investment Ledger Design

***Referenced in:** [Org Investment Ledger](#org-investment-ledger), [Org Investment Ledger Design Guidelines](#org-investment-ledger-design-guidelines)* 

***Must align with:** [Org Investment Ledger Design Guidelines](#org-investment-ledger-design-guidelines)* 

The org investment ledger design defines all of the properties of the org investment ledger, as outlined in [Investment Ledgers Detail](#investment-ledgers-detail) section. It must meet all guidelines outlined in [Org Investment Ledger Design Guidelines](#org-investment-ledger-design-guidelines).

## Required Process Definitions

### Change Process for Financial Model Definition

***Referenced in:** [Governance](#governance), [Org Investment Ledger Design Guidelines](#org-investment-ledger-design-guidelines)*

This defines the governance process for making changes to this document. 

Making changes to the Financial Model should be considered a formal process requiring a high-level of confidence in the quality of the changes being made. The Financial Model will need to evolve as we learn more about what works and what doesn’t. It is, however, important that the Financial Model maintain a level of stability due to its importance and the potential negative impact of improperly considered changes.

Until this process is formally documented, making changes to this document should require the 75% approval of Quorum1 partner members (allowing for partners to appoint another partner as a proxy as needed).

### Change Process for Financial Operations Plan

***Referenced in:** [Governance](#governance), [Standard Ledgers](#standard-ledgers), [Org Investment Ledger Design Guidelines](#org-investment-ledger-design-guidelines), [Required Documents](#required-documents)*

This defines the governance process for making changes to the Financial Operations Plan which is the set of documents defining the operational implementation of the Financial Model. 

This is a critical governance process because the Financial Operations Plan will eventually be composed of a large, complex, wide-ranging set of documents which will be iteratively created and improved over time. As such it is important that we allow for fluidity and agility as we work to learn what works and what doesn’t.

Until this process is formally documented, making changes or additions to the Financial Operations Plan should require the written agreement of the Foundation Leadership. The members included in the Foundation Leadership are appointed by the Managing Partners and must be clearly documented. Each change or addition to the Financial Operations Plan must be documented and explained in a central repository of changes which is visible to all contributor and partner members.

### Ledger Management Process

***Referenced in:** [Ledgers](#ledgers)* 

This process must define workflows for creating new ledgers, making changes to existing ledgers, retiring ledgers, and administering the ongoing operations of ledgers.

It is important that ledger management be as streamlined as possible, while also ensuring that the overall ledger structure is operationally reliable and administration is secure, accurate, and compliant.

### Vendor Registration Process

***Referenced in:** [Vendor Company Outflows](#vendor-company-outflows)*

This process defines how new vendors are registered and onboarded so that they may be targeted by outflows.

### Hosted Entity Management Process

***Referenced in:** [Hosted Entities](#hosted-entities)* 

This process defines workflows for managing hosted entities. This includes creating new hosted entities, making changes to existing hosted entities, retiring hosted entities, and spinning hosted entities out into separate companies.

### Recurring Expense Management Process

***Referenced in:** [Expense Ledgers](#expense-ledgers)*

This process defines how recurring expenses within expense ledgers are managed. It is important that we closely manage these types of expenses so that we’re balancing the outgoing expenses with expected income, and so that any potential shortfalls can be identified and mitigated well ahead of time.

### Expense Reimbursement Process

***Referenced in:** [Expense Ledgers](#expense-ledgers)*

This process defines how expense reimbursement requests are submitted by members, and then either approved or denied by the ledger managers of an expense ledger. Due to our collective structure and focus on ethical financial structures, and due to the potential risk of misappropriation involved in expense reimbursement, it is critical that this process meet our highest standards of transparency and accountability.

### Debit Card Management Process

***Referenced in:** [Expense Ledgers](#expense-ledgers)*

This process defines how debit cards linked to expense ledgers are managed. This includes workflows for allowing the ledger managers to request new debit cards, the Foundation responding to those requests, creating and retiring cards, setting and changing limits, and other workflows as needed.

This process must also include appropriate training and verification for debit card holders to ensure that they are aware of best practices for managing these debit cards and how to mitigate potential fraud or theft risks. 

The Foundation may opt to impose security requirements on debit card holders to prevent potential fraud or theft.

### Investment Ledger Management Process

***Referenced in:** [Investment Ledgers Detail](#investment-ledgers-detail), [Standard Process for Designing an Investment Ledger](#standard-process-for-designing-an-investment-ledger)*

***Must align with:** [Standard Process for Designing an Investment Ledger](#standard-process-for-designing-an-investment-ledger)*

This process defines how investment ledgers are created, changed, retired, and operationally managed.

### Investor Management Process

***Referenced in:** [Money Investment](#money-investment), [Investment Ledger Inflows & Outflows](#investment-ledger-inflows--outflows)*

This process defines how money investors are onboarded, off-boarded, what required documentation is needed, and other details necessary to manage the money investors.

### Member Payment Eligibility Process

***Referenced in:** [Member Outflows](#member-outflows)* 

This process is important to ensure that the quorum has collected appropriate financial information and ensured that we are not restricted from sending a particular member money for some reason.

In order for a ledger to directly target a member for outflow allocation, the member has to have signed a formal agreement with Quorum1. If members have joined the quorum via a corporate entity, then their payments are directed to their registered corporate entity. Some members may be restricted from direct allocation if there are legal or regulatory restrictions that apply to them.

### Rev Token Ownership Processes

***Referenced in:** [Rev Token Lifecycle](#rev-token-lifecycle), [Rev Token Transfers](#rev-token-transfers)*

This process defines how rev tokens are purchased, issued, and managed by the owner. It also defines all key workflows needed to support the ongoing management of rev tokens. It must include workflows for updating the rev token’s recipient, for splitting the rev token into multiple rev tokens, and for transferring ownership (as part of either a gift or a sale). It must also include a workflow for retiring a rev token.

This process may optionally define a slightly different process for Quorum1-owned rev tokens.

### Refund Process

***Referenced in:** [Fulfillment, Recognition, & Refunds](#fulfillment-recognition--refunds)* 

This process defines how unfulfilled revenue in a fulfillment ledger may be refunded back to its source (such as back to an external client or back to another internal ledger). 

---
