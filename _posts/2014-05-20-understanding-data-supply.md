---
layout: post
title:  Comparing Contract Data: Understanding Supply
date:   2014-05-20
author: Ana Brandusescu
image: /assets/images/opendatacomparison.jpg
---

The [Open Contracting Global Principles](http://www.open-contracting.org/global_principles) call for governments to "*require the timely, current, and routine publication of enough information about the formation, award, execution, performance, and completion of public contracts to enable the public, including media and civil society, to understand and monitor as a safeguard against inefficient, ineffective, or corrupt use of public resources.*"

Although there is a long way to go before all governments publish this information, many governments already maintain contracting portals and publish datasets that provide varying levels of detail about the contracting process.

## Key questions

As part of our supply-side research, we’ve been looking in-depth at these existing datasets, seeking to understand:

* Which elements of the contracting process are captured in currently published data?

* Which fields are commonly found across different datasets?

* How do different datasets represent and model the contracting process?

* How far are there common identifiers that can be used to join up between datasets, either from the same country, or across countries?

## Creating a platform

Rather than just run a one-off analysis through a tangle of spreadsheets, we’ve taken a tool-building approach, creating the Contracting Data Comparison site, and working with a growing team of volunteer developers to provide a platform for curating meta-data about public contracting datasets from [priority countries](http://open-contracting.github.io/pages/notes/datasets/priorities.html).

This platform is not about capturing the contract data itself but about capturing the metadata of the contract data available.

Through the **Contracting Data Comparison (CDC)** platform we are able to:

* Keep track of different publishers of contracting data, document their current publication practices and how data is structured by different publishers

* Log details of all the datasets they have available for download in different formats - also exposing these through an API - to support automated aggregation of data

* Import and store detailed mappings between the current data models used by publishers, and common classifications of fields and data structures

* Allows us to query the data in multiple ways once it is captured

* Provides an open platform for anyone to view and contribute (e.g., the San Mateo dataset was added by a community member)

* Store complex relationships that are not easily captured in spreadsheets

* Provides a database for data quality assurance, which tracks any revisions and changes made

We developed a multilingual documentation for the dataset ‘Description’ field, and decided that CDC should have English as the first language, followed by the original language of published datasets.

![Website Screenshot](/assets/images/2014-05-20-Supply/image_0.jpg)

We think this function can be duplicated for the ‘Publisher’s description field as well. Currently, all of our publisher description is in English.

Our hope is that, as it develops, the Contracting Data Comparison will allow us to keep developing an ever more detailed picture of the landscape of contracting data availability.

The next step of developing the platform is to add visualisations that help us dig into and analyse the information it now holds.

## Analysis so far

Over recent weeks, Open Contracting Data Standard researcher Ana has been focussed on adding datasets from a priority list of countries, and mapping out information about their respective publishers in the ‘[Publishers](http://ocds.aptivate.org/opendatacomparison/publishers/)’ and ‘[Datasets](http://ocds.aptivate.org/opendatacomparison/datasets/)’ tabs.

In most countries, whilst there might be a central government contract portal, public contracting information is in fact scattered across many different websites, portals and datasets. For example, in Canada contracts only make it into the central BuyAndSell.gc.ca portal if they are over a certain threshold value (based on values specificied in trade agreements), and regional or local government contracts may exist in various forms on local websites. In other countries, information on procurement processes and contracts awarded might exist in different systems, or data released might be split across files by month or by some other segmentation.

This suggests a simple standard may have substantial value inside a single country, linking up contracting information from multiple levels of government.

However, we now have 37 datasets with over 175 downloadable assets (different downloads of those datasets) from 27 publishers, from across the world. The 26 publishers are from 15 countries that were selected as priorities countries due to their current activity in open government and the [Open Government Partnership (OGP) Action Plan](http://www.opengovpartnership.org/how-it-works/action-plans). Next on the list are the countries that are in the stages of developing a first and second OGP Action Plan.

You can find the publishers and datasets from the top menu at [Contracting Data Comparison](http://www.google.com/url?q=http%3A%2F%2Focds.aptivate.org%2Fopendatacomparison%2F&sa=D&sntz=1&usg=AFQjCNE1kDsXBmBodRDHw9vlkb8XFxyF1A).

![Website Screenshot](/assets/images/2014-05-20-Supply/image_1.jpg)

We added the ‘Administrative Level’ and ‘Administrative Level Category’ fields for Publishers:

* *Administrative Level* determines what level the dataset is on (Provincial, State, County. The field is based on the appropriate term for the dataset, based on the dataset publisher. For example, if it is Canadian, use Province, if it is American,  use State.

* *Administrative Level Category* is divided into subsections: International, National, First-level, Second-level, Third-level, and Fourth-level and smaller

The Administrative Level Category’ field is structured pertaining to the ISO 3166-1 Table of administrative divisions by country, which are explained in detail [here](https://en.wikipedia.org/wiki/Table_of_administrative_divisions_by_country).

## Lessons learned

The contracting websites we have assessed vary immensely in their content and accessibility. It has been an interesting and challenging start. However, this is the nature of working with heterogeneous data portals and datasets. We know that we will be working with fragmented, incomplete and non-user friendly information. We began assessing the datasets from Canada, given their accessible and machine-readable properties.

We had some difficulties with translating some of the data portals (Spanish, Portuguese). Whilst we are committed to making the Open Contracting Data Standard useful across language barriers, we’re primarily working in English in our initial analysis (ideas or suggestions for effective ways we can broaden engagement across languages on our limited resources would be very welcome). The Google Chrome plug-in translator generally works well, but can struggle with the way some contracting websites are built. Our workaround for this issue was using Google Translate when the Chrome plug-in could not translate the website text. For KONEPS, we are waiting for Korean translation assistance as the entire site is available in just Korean.

At this stage, all datasets have been categorized under the ‘Contracting – Standard Category’. As we move into the extension phase, we will be collecting Land and Extractives datasets, which have a separate category for ease of identification.

We are currently documenting which 5 phases of the contracting process each dataset in Contracting Data Comparison covers. Details are coming soon!