---
layout: post
title:  Montreal Python Conference (PyCon) Sprint - What We Worked On 
date:   2014-06-10
author: Ana Brandusescu
image: /assets/images/opendatacomparison.jpg
---

We (Sarah, Ana, Tim and Michael) met at PyCon in Montreal (April 14-17) to lead the Open Contracting sprint in the Open Spaces rooms. There were many interesting discussions held over the four days of sprints from topics on data ontologies to public procurement phases. 

This blog post covers the ways in which we applied what we discussed in the previous blog post.  

## PyCon Sprint Teams

We divided the project work planned over the 4 day sprint by forming 3 main teams: 

1. Python and machine learning team ([Developer Documents](http://www.google.com/url?q=http%3A%2F%2Fopen-contracting.github.io%2Fpages%2Fdocs%2F&sa=D&sntz=1&usg=AFQjCNErVaGGGBd2qenPczGG2Krc5F-oRw))

2. User case studies team - demand side research ([User Stories Tool](http://www.google.com/url?q=http%3A%2F%2Fopen-contracting.github.io%2Fpages%2Fusecases%2Fshareyours.html&sa=D&sntz=1&usg=AFQjCNGYDIkoMgcJ7wBzHcYV_24huOZJsQ))

3. Data field landscape team - supply side research ([Hackpad Notes](https://www.google.com/url?q=https%3A%2F%2Fopencontractingdata.hackpad.com%2FPyCon-2014-Sprint-Project-Open-Contracting-Datamap-Landscape-ei3XM4ruVi3&sa=D&sntz=1&usg=AFQjCNF_CDGjSO2wSjr0W4JPo9DGF2hLsg))

Sarah led the coding/Python team. There were many developers interested in collaborating their Python skills for technical contributions to Contracting Data Comparison (CDC). Two of the focus areas included machine learning and CDC functionality. Contributors included Aaron Cohen, Andreas Dewes, Simon Frid, Michael Glaude, Bryan Gorges, Brittain Hard, Brantley Harris, Matt Lamberti, Dan Langer, Teddy McWilliams, Aaron Rothenberg, David Street, Nick Zaccardi. 

Tim led the user case studies team, building the [User Stories Tool](http://open-contracting.github.io/pages/usecases/shareyours.html) for participants to share their open contracting stories, available on the Open Contracting Data Standard page. Discussions were held with John Jordan and Louis Charbonneau, as well as with other developers at PyCon.

Ana led the data field landscape team. We found many researchers and open government enthusiasts interested in data ontologies, standards and analysis of open contracting. The team: Eric Canen, John Jordan, Herb Lainchbury and Noé Domínguez Porras.

## The Data Field Landscape Team  

As we are in the initial phases of the open contracting data standard, the focus for the sprint was on **[Goal **1](http://open-contracting.github.io/pages/notes/datasets/)** of Building a Datamap: ****Provide a landscape of available data**. For this goal, a deep analysis of the datasets and fields within the datasets was required. The question we focused on was the following:

What fields *should* be in a standard is a question for our demand side analysis (asking users what they want and need). But when we ask that question it is important to be informed by what is already readily available - so what data is currently available from contracting portals? 

When answering this question, we should keep in mind what users actually need. Knowing the landscape of available data can help inform decision making for a first draft of the standard. This phase is the *data audit*.

The first step is to categorize datasets into concepts that really make sense from both a data and a procurement point of view. In doing so, we began consolidating datasets that we would subject to a deep analysis. We worked with 7 specific contracting datasets drawn from our [Priority Countries list](http://www.google.com/url?q=http%3A%2F%2Fopen-contracting.github.io%2Fpages%2Fnotes%2Fdatasets%2Fpriorities.html&sa=D&sntz=1&usg=AFQjCNFdwTRX8oLxhwOmdbSWnGHFdPB0jA): Canada, UK, Mexico, Georgia, Moldova, EU and UNOPS. 

![Website Screenshot](/assets/images/2014-06-10-pycon-b/image_0.jpg)

The datasets are available to view in [CDC Open Contracting Data Field Landscape](https://docs.google.com/spreadsheet/ccc?key=0AqLP9fZSKM8jdFg2WGhHQi1QbE54Wml5aDNyaUVDRGc&usp=sharing#gid=0). 

We created column headings to show the progress from original dataset names to standard ones we would be using in our refinement process. This was especially important when handling non-English datasets and portals.  

We constructed a field data name convention to be used across all datasets (e.g.,  lower case, separated by underscores). Throughout our analysis, we realized some datasets were had aggregated information, not individual contracts, and included new datasets subject to a deep analysis. We also decided to focus on three of the open contracting process phases: tender, award and contract. The next section, datamap concepts, details our process.

## Datamap concepts: Contracting phases

After many discussions about concepts and all phases of public procurement, we decided to focus on 3 of the 6 phases of contracting we agreed upon: Tender, Award and Contract. Having an in-depth analysis of the 7 datasets aided that decision. Most data found in the prioritized datasets was related to these particular phases. 

All phases are listed below. They include field names that are linked to each phase.   

1. **Planning**

2. **Tender** (sprint focus)
 * awarding / facilitating / procuring entity (e.g., party obtaining goods and services)
 * receiving entity (e.g., party that won) 
 * goods 
 * budget (e.g., min value, max value, currency type)
 * tender date (e.g., published date, closing date)
 * tender status (e.g., active, closed, cancelled)
 * tender type
 * procurement strategy
 * documents (e.g., link to RFP - Request for Proposal)
 * other 
 * tender unique identifier (e.g., numbers and/or letters pertaining to tender)
 * linking identifiers

3. **Award** (sprint focus)
 * awarding entity
 * receiving entity
 * goods / services 
 * contract start date 
 * contract end date
 * contract value
 * currency type 
 * contracted entity (entity that won the contract)
 * documents
 * other
 * contract unique identifier (e.g., numbers and/or letters pertaining to the contract itself)
 * linking identifiers

4. **Contract** (sprint focus)
 * amendment number (very important for transparency)
 * amendment reason
 * contract record / PO / credit card data

5. **Performance**
 * invoices
 * payment from
 * payment to
 * transaction value
 * milestone
 * other
 * unique identifiers
 * linking identifiers
 * contract Status

6. **Close**
 * status
 * final value
 * other
 * unique identifiers
 * linking identifiers


Each dataset included the following columns: Original Name, English Name, Formatted Name, Standard Name, Description of Field, English Translation of Description. These were created to have clear links from the original dataset names to names that are finalized for CDC.  

We decided to categorize the dataset information in linked concepts: Phase - Entity - Group. All field names we found in the datasets are integrated in these 3 linked concepts. 

e.g., tender (phase) - solicitation (entity) - tender_status (group)

We also added information about the field names in terms of ‘Allowable Values’ and ‘Data Types’ (shown in detail below).

Allowable Values are constrictions to free text inputted and exclusive parameters given.  For example, the field name "tender_openness" can only be Open, Selective or Limited; these terms are the allowable values. 

Data Types represent the format of the data in the following categories: 

* Free Text

* Date or Date Time

* Currency Value

* Currency Type

* Single Select

* Multiselect

* Email

* URL

 

In addition to the in depth analysis of these datasets, we brainstormed visualizations for dataset comparisons across countries. An example of a potential target comparative capability would be to have visualization capabilities *across jurisdictions*, as rendered in [Georgia’s procurement portal](http://www.google.com/url?q=http%3A%2F%2Ftendermonitor.ge%2Fen%2Fanalysis%2Findex&sa=D&sntz=1&usg=AFQjCNGWPKMdTYNqzvSYTGzH4ZefbnQY8w). 

## Epilogue

The discussions and analysis of the contracting datasets proved to be a valuable learning experience. After the sprints, we had learned that we needed to consolidate a part of this work, because there was too much detail in the phases we focused on (e.g., tender, award, contract) and not enough clarity. We should keep in mind that it was necessary to go through this process in order to achieve clarity on contract phases and the type of information that needs to be included for the standard. We aim to find a balance between simplicity without too little detail.  

The next blog post will discuss the changes and progress made since the PyCon Sprint. 

