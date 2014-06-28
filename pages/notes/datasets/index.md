---
layout: single
title: Datasets
date: 19/03/2014
---
There are already a lot of agencies publishing public contracting data. As a 
result its vital that we both learn from these existing sets and ensure that 
we can accomodate them.

We are reviewing as many as we can as part of our "supply side" analysis of 
open contracting data.

There are three types of possible review, which are documented [here](review_types.html).

The prioritized list of datasets for review including which type of review are [here](priorities.html).

We have been documenting our findings on our data comparison site [http://ocds.open-contracting.org/opendatacomparison](http://ocds.open-contracting.org/opendatacomparison)

### Building a datamap
Part of the supply side analysis is to *understand* what fields publishers are already publishing. We are documenting the fields with the following goals in mind:

* What fields *should* be in a standard is a question for our demand side analysis (asking users what they want and need). But when we ask that question its important to be informed by what's already readily available. Perfection is the enemy of good & knowing what the landscape of available data is can help inform a first draft of the standard. **Goal 1** Provide a landscape of available data
* Gather data to inform the harmonization challenge. Moving forward it is likely that there will be some fields that have a set of allowable values e.g. Contract category: goods, supplies, consultancy, leasing etc. As part of identifying a set of fields for the standard, we will also have to identify those that need to be harmonized so that they can be compared across multiple datasets. **Goal 2** Collect currently used values for fields so we can assess heterogeneity across datasets
* Computers love to identify things, understanding what datasets currently have as unique identifiers will help us to understand what identifiers are available and where challenges might lie with duplication (e.g. if we only have company name, and not an ID, then that name could be mispelt) **Goal 3** Identify unique identifiers.
* We need to follow a contract through its phases. Many publishers release datasets about the different phases seperately. e.g. the tender data is distributed seperately to the award data. We need to document if and how a contract is traceable from one phase to the next. **Goal 4** Document traceability through phases
* In creating a landscape where we identify common fields across multiple datasets, we are a step closer to having data be interoperable. We know that in the not to distant future we will want to attempt to convert some existing datasets into the new OC data standard so we can record mapping that will help that **Goal 5** Facilitate data conversion between existing datasets.
* Accomodate new contracts as we encounter them. In our attempt to build a landscape we need to incorporate different kinds of contracts e.g. framework contracts, land, extractives etc. **Goal 6** Our landscape should be able to document and capture new variations as we uncover them.

### Datamap Concepts (Note: June 27 2014 - needs updating)
* Planning (catch all just one for now)
* Tender
 * Awarding entity
 * Receving entity
 * Goods / services (need a better name for this?)
 * Budget
 * Documents
 * Other
 * Unique identifiers
 * Linking identifiers
* Awards
 * Awarding entity
 * Receving entity
 * Goods / services (need a better name for this?)
 * Contract Value
 * Contracted entity (entity that won the contract)
 * Documents
 * Other
 * Unique identifiers
 * Linking identifiers
* Performance
 * Payment from
 * Payment to
 * Transaction Value
 * Milestone
 * Other
 * Unique identifiers
 * Linking identifiers
* Close
 * Status
 * Final value
 * Other
 * Unique identifiers
 * Linking identifiers
