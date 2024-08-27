# Org Investment Ledger Governance Flow

_**Dependencies:** [Informal Governance Model Definition & Roles](./igs-roles.md), [Q-Git Governance Change Flow](./q-git.md)_

This flow defines the process for making changes to the [Org Investment Ledger Design](../docs/glossary.md#org-investment-ledger-design) in alignment with the requirements of the [Financial Model](../docs/glossary.md#financial-model).

Changes to the Org Investment Ledger Design follow the standard Q-Git flow with the additions and changes outlined below.

## Additions to Standard Q-Git Flow

### Development Roles

The Ledger Manager must be included in the approvals step and has the ability to veto.

## Investment Ledger Governance Parameters

### Token Downgrade Governance

This section describes how token downgrades are executed.

#### Restrictions

Token downgrades should happen no more than once per year and should not happen before year 6.

#### Process

A token downgrade is documented by adding a description to the 'Token Downgrades' section of the Org Investment Ledger Design doc. This description should include:
- Date of Token Downgrade
- Downgrade Factor
- Rev Token Full Value Grand Total (Before Downgrade)
- Rev Token Full Value Grand Total (After Downgrade)

A token downgrade is approved via the amended Q-Git change management flow defined in this file.

#### Special Review Requirements

When a token downgrade is present in a Release:
1. The gap between the start of Step 3c (Member Review) and the start of Step 3f (Partner Approval) must be a minimum of 45 days.
2. All money investors should be notified per their duly stated preferences upon the start of Step 3c (Member Review).

## Failsafe Equity Conversion

A Failsafe Equity Conversion can only be triggered with the approval of the Steward and at least 75% of Partners, and it must be approved along with a detailed execution plan that must align with the following parameters:

1. A suitable Destination Legal Entity is identified that will have stock issued such that its final ownership percentages match the proportions established below.
2. The Destination Legal Entity may have either one or two classes of stock:
    1. If one:
        1. The same class of stock will be used for both time and money investors.
        2. All time investors will collectively own 50% of the shares with each individual owning a percentage proportional to their total remaining rev point balances.
        3. All money investors will collectively own 50% of the shares with each individual owning a percentage proportional to the total remaining full value of the active rev tokens they own.
    2. If two: One class of stock will be used for time investors and another will be used for money investors.
        1. Each individual time investor will own a percentage of the time investor stock class proportional to their total remaining rev point balances.
        2. Each individual money investor will own a percentage of the money investor stock class proportional to the total remaining full value of the active rev tokens they own.
