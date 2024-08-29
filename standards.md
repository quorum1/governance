# Quorum1 Governance Repo Standards

This doc outlines guidelines, standards, and best practices for the contents of the Quorum1 Governance Repo.

We are still in the process of porting our entire governance structure into this repo. As we develop the repo out more these standards are likely to shift and evolve. As such this doc should be considered in a draft state and subject to change.

## Guidelines

### Inter-File Links & Term Definitions

Markdown syntax allows us to link from on repo file to another like this: `[Example Link](../path/to-other-file.md#header-to-link-to)`. 

Direct references between repo files should be avoided unless the cited page is a critical dependency of the referring page. In such a case:
1. The inter-file link should only be included once
2. The inter-file link should appear either:
    1. At the very top of the file, just under the header.
    2. OR appear in a section *near* the very top of the file titled with an h1 or h2 with the exact text "Key Dependencies".

For all other cases, any terms which need to be shared between files should be defined in the [Gov Repo Glossary](./docs/glossary.md) with a unique header text at any level (h1, h2, h3, etc) and then linked to like this: `This aligns with the [Financial Model](./docs/glossary.md#financial-model).`

The Gov Repo Glossary can be thought to be an automatic dependency of every file in the gov repo and does not need to be specifically called out in each file, though it can be if it's useful to do so.
