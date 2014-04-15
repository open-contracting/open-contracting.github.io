---
layout: single
title: Developing User Stories and Use Cases
date: 14/04/2014
---

_This is a draft document exploring different approaches to developing user stories and use cases for the OCDS project. It is being actively developed over the course of the Montreal Development Sprints at pyCon. You can edit and suggest changes from the link at the bottom of the page._

# Background

An open contracting process has many stakeholders. They many have many different information and data needs in different settings and at different times. Use cases provide a way to identify particular users, and to describe their particular information and data needs. 

In developing a draft data standard for Open Contracting we will draw on use cases to:

* Develop and check our understanding of what different stakeholders want to do with open contracting information and data;
* Indentify technical, data content and data quality requirements that may be needed to meet specific use cases. 

# Methodology

There are a range of different methods for developing user stories and use cases. For example:

* Wikipedia (at the time of writing) describes [user stories](http://en.wikipedia.org/wiki/User_story) as "one or more sentences in the everyday or business language of the end user or user of a system that captures what a user does or needs to do as part of his or her job function". Simple user stories may take the form ‘As a *role*, I want *goal/desire* so that *benefit’* and can be linked to specific software features. They may also be framed within the context of persona profiles or descriptions of particular problems and challenges. 

* Wikipedia describes [use cases](http://en.wikipedia.org/wiki/Use_case) as involving a goal, a main success scenario, steps required to meet it, and potential extensions. They can be represented in Unified Modelling Language with actors and goals. 

* The [CSV on the Web Working Group](http://w3c.github.io/csvw/use-cases-and-requirements/#UC-DigitalPreservationOfGovernmentRecords) have written a set of Use Cases and Technical Requirements. These describe a particular technical challenge faced, and detail the particular technical elements involved (e.g. requiring a Primary Key, or a transformation from CSV to XML), as well as summarising how some more advanced standardisation or tooling could help with the scenario described. 

* James McKinney describes hows the [Popolo project](http://popoloproject.com/) developed use cases by ooking at the demand side (especially what civil society organizations wanted in terms of legislative data)  and looking at what existing standards had terms for (an indirect indication of needs, since those standards must have been created to fulfill use cases). The resulting "use cases and requirements" sections are brief summaries that describe particular data elements that might be valuable to a user, giving examples.

The project also collects use cases and requirements through a [mailing list](http://lists.w3.org/Archives/Public/public-opengov/) and [issue tracker](http://popoloproject.com/specs/person.html). If at least two groups have a need for something, that’s usually sufficient reason to add it to the spec. The project target audience are tech-savvy civil society organizations.

Questions for Open Contracting user stories & use cases:

1. Should our user stories and use cases be based upon real people, or generalised cases. 

2. ?

# A draft Open Contracting User Story

## Monitoring infrastructure building.

### Goals

An elected officials of a municipal authority is responsible for oversight of public budgets and spending. The city currently budgets on a three-yearly cycle for works, but projects may take many years from budget to completion. A road refurbishment project is taking place. The elected official wants to ensure that the authority is getting value for money for the project, that the work is completed to a high quality, and that no funds are lost through corruption. 

### The situation now

A budget is set for the project, and tenders issued. A contractor is selected on the basis of the lowest bid. The project begins, but no realised budgets are available until 14-months after the end of the financial year, and these are not directly linked to contracts. During implementation it is discovered that the original tender made an error in stating the length of road to be laid, and so an amendment is made to the contract to cover an extra 10-miles. Payments against the contract are made over a number of years, with the total substantially exceeding the original budget, although the reasons for the over-run are not clearly documented. Payments may be delayed many months after work is completed, with large firms able to accept six-month and longer delays in payment, but small firms forced into bankruptcy by these delays. 

Later on, revenue budgets for repairing the road are not linked to the original capital expenditure. Sometimes repairs take place through the capital budget when city engineers are paid as contractors at the year-end. 

The road built through this contract breaks up much quicker than other roads by the same contractor, due to the low quality of work by a particular subcontractor who worked on the project.

### User stories

* As an elected official I want to be able to monitor the progress of a contract throughout it’s implementation, able to check in on how far budget has been realised at each stage of the contract;

* As an elected official I want to see the linkage between a contract and the specific infrastructure it has funded, and for that link to be maintained into the future;

* As an elected official I want to understand which part of the public authority is responsible for implementing and monitoring a contract;

* As an elected official I want to be able to compare bids based on the cost and quantity of inputs to be used (e.g. Asphalt; Crushed Stone), rather than always opting for lowest-cost bids;

* As an elected official I want to be able to compare the cost of inputs and work in my local area to the cost of inputs and work in other areas;

* As an elected official, if I can see information on the tender, and final realisation, of a contract, I can know where to investigate for more information - but if I only know about one end of the process (start or end) it is hard to know where to look.

### Related persona profiles:**

[Ravi Shrestha](http://open-contracting.github.io/pages/notes/workshops/2014-01-Montreal/personas.html#ravi-shrestha-owns-small-store)

###Related use cases

ToDo

### Related requirements: 

* **Lifetime tracking**- ToDo - ID that connects budget, contract and cheque-book entries


* **Line Items** - It should be possible to record line-items required by the contract, including using a controlled list of kinds of contract 

* **Geographic Information System Linkage - **It should be possible to relate particular elements of a contract to entries in a Geographic Information System (either the internal authority system, or a public system such as Open Street Map). 

## Use case 2 (stub)

Civil society organisations has been republishing PDFs of government contracts and transparency requests. Gets agreement from government that it will supply the data in machine-readable format
