# Quorum1 Governance Repo - Release 4 (Working)

This repo contains Quorum1's official governance processes and models. 

Quorum1 is a professional collective. Our website is at: https://quorum.one

Our governance repo is hosted on Github and managed using branches, pull requests, and other Git-based tools. The audit history of changes to this repo is considered part of Quorum1's public record.

## Release 4 Checklist

- [ ]  Privacy Policy
- [ ]  Terms of Service
- [ ]  Operating Agreement
- [ ]  Rules & Regs: Adapt to point to codes of conduct
- [ ]  Codes of Conduct: Adapt something like this:  (Starting point: https://docs.google.com/document/d/1_nRl5Q3DsajCqkQH3JQMjNp1NmkgEjHc7KEMA-qzwjA/edit)
- [ ]  SOW Templates: This is probably a subfolder of docs with a few different templates for things like co-ventures, client project roles, etc.
- [ ]  Update all existing docs to new membership level names (Network > Contributor > Foundation > Steward)
    - [ ]  Also rename contributor agreement back to ic-agreement (Independent Contractor Agreement)

## Structure of this Repo

- [/docs](docs/): Contains our governance docs. These define important processes, agreements, structures, models, and workflows. Collectively they are our "governance design".
- [/flows](flows/): Contains our governance change flows. These define how changes to different parts of the governance repo are made. Collectively they are our "meta governance process" (the change management process for our governance design).

## Current Status of our Governance Repo

This is Release 3, the current live release.

We are still in the process of porting our entire governance structure into this repo. Prior to June 2024 our governance structures have been managed in many different places. This repo is an effort to unify those pieces in order to increase transparency, streamline change management, and facilitate greater collaboration.

**Roadmap:**
- Short-Term:
    - Finish adding operating model to gov repo (requires refactoring)
    - Migrate more existing docs into gov repo (code of conduct, member SOW templates, partner agreement, etc)
    - Finish building out member review process in Q-Git
    - Consider re-architecting Q-Git structure to separate dev flow from release flow
    - Improve the [Quorum1 Governance Repo Standards](./standards.md) doc
    - Iterate the [Gov Repo Glossary](./docs/glossary.md)
- Medium-Term:
    - Begin work on formal governance framework
    - Create other repo(s): Fin Ops, potentially others
    - Work on set of modular, re-usable governance flows w/ templated roles

## Why is Quorum1's governance structure managed on Github?

We are committed to transparency, trust, and collaborative decision-making.

Open-sourcing our own organizational operating system is in strong alignment with those commitments. 

In addition, git-based workflows are amongst the most effective ways to facilitate wide-scale collaboration around text-like documents. By building our governance processes on top of git, we're taking advantage of a robust & mature set of tools & change management processes.

## License Status of this Repo

We are still determining the best license to use for our governance repo. While we make this determination, all rights are reserved by Quorum One LLC, a collectively owned and managed company incorporated in California, USA.
