---
layout: post
title:  Montreal Python Conference (PyCon) Sprint - What We Discussed 
date:   2014-05-25
author: Ana Brandusescu
image: /assets/images/opendatacomparison.jpg
---

We (Sarah, Ana, Tim and Michael) met at PyCon in Montreal (April 14-17) to lead the Open Contracting sprint in the Open Spaces rooms. There were many interesting discussions held over the four days of sprints on topics ranging from data ontologies to public procurement phases.

This blog post covers the ideas we brainstormed on public procurement and contracting data. These include information about standards and documentation and varying contexts that range from Canadian e-portals to global organizational systems and procurement laws.  It also details contracts and trade agreements, international standards, classification and coding schemes and taxonomies.

## Priority Countries, Standards and Documentation

## Canadian context

One discussion focused on Canadian portals and public procurement. BuyAndSell.gc.ca shares data on behalf of Canada for public procurement by Public Works and Services Canada who cover a small percentage of contracts but large percentage of the dollar value; their information is linked to Data.gc.ca. Every government department in Canada is required to show their contracts on their page, however there are many inconsistencies in their portals. This includes the sheer number of departments (100+) that would need web scraping if we would want to consolidate and link all information to one portal (e.g., BuyAndSell.gc.ca).

## Global context

Different countries have different organizational systems and procurement laws. For example, Chile and UK have a central procurement agency that has the authority to provide services to all other levels of jurisdiction, therefore these governments have good data. In contrast, Public Works and Services Canada does not have the authority to offer services to individual provinces, as each province manages this process independently, where a stronger relationship between counties and cities exists. Similarly in the US, states have a lot more power, decentralized system where, for example, a government body such as the General Services Administration (GSA) is not a mandatory service and so they have to compete to get this data.  Even though some countries are open about their public procurement process, more clarity in the internal country portals/systems is needed. For example, in Mexico, the Secretary of Finance and Public Procurement has published a [document](http://www.apartados.hacienda.gob.mx/presupuesto/temas/pef/2000/documentos/introduccion/anexo2.pdf) that describes how the data about the buyers and public spending is aggregated. However, more information could be provided on how the money is spent.

## Contracts and trade agreements

Trade Agreements drive the fields for tender notices and the need for them to be public. These could be considered to be a basic subset of contracting fields as tenders are typically the earliest and most publicly shared artifacts of the procurement process. For example, [Article 1010](https://www.nafta-sec-alena.org/Default.aspx?tabid=97&ctl=SectionView&mid=1588&sid=a550e516-c181-49fc-9176-76db29b2969b&language=en-US#A1008): Invitation to Participate of the North American Free Trade Agreement specifies what tender notices need to contain to be considered compliant to the agreement. Other agreements such as the World Trade Organization Agreement on Government Procurement has a similar [definition](http://www.wto.org/english/docs_e/legal_e/gpr-94_01_e.htm#articleIX).

## International standards in the same / similar domain

We also had fruitful discussions on the importance of processes and data types that have already been modelled, and what these mean to the standard we are creating. One such standard to consider is the [OASIS Universal Business Language](https://www.oasis-open.org/committees/tc_home.php?wg_abbrev=ubl) standard. This standard is based on "defining a common XML library of business documents (purchase orders, invoices, etc.)."  It includes the tendering process documented and fully described [here](http://docs.oasis-open.org/ubl/os-UBL-2.1/UBL-2.1.html#S-TENDERIN).

![Website Screenshot](/assets/images/2014-05-25-pycon/image_0.jpg)

Source: [OASIS Universal Business Language standard](http://docs.oasis-open.org/ubl/os-UBL-2.1/UBL-2.1.html#S-UBL-2.1-BUSINESS-OBJECTS).

The section of the specification which goes through a procurement process in detail is a *must read* for anyone interested in understanding generally how procurement works *and* the data artifacts that may be involved in a procurement from conception to contract close out. In addition, the document provides an interesting contextualization of the "buy" process which includes procurement and purchasing as sub-actions. This is an important distinction, as in reality they are separate processes, organizations and outcomes, resulting in different data artifacts.

## Classification schemes, coding schemes and taxonomies

The [Product Classification Systems as Web Ontologies](http://www.ebusiness-unibw.org/ontologies/pcs2owl/) site has started a list of classification schemes. The site uses the [PCS2OWL tool](http://www.ebusiness-unibw.org/ontologies/pcs2owl/) for the transformation from product classification systems to classification schemes. The [CEN cMap Project](http://www.cmap.eu/index.php?option=com_content&view=category&layout=blog&id=7&Itemid=101) is a great EU project that addressed crosswalks between some major classifications schemes. The United Nations Standard Products and Services Code (UNSPSC) Wikipedia [page](http://en.wikipedia.org/wiki/UNSPSC) has a list of other similar schemes.

Classification schemes are key for interoperability. However, these are not always clearly labeled. For example, if contracts for desktop computers are "tagged" using [UNSPSC](http://www.unspsc.org/) "43211507, Desktop computers" in Jurisdiction 1 and "tagged" as "N7021: ADP Central Processing Unit (CPU, Computer) Digital" in Jurisdiction 2, comparative benchmarking activities can become quite difficult and frustrating. Therefore, the standard should consider these key classification schemes and determine if a value add of the standard community could be "mappings" or "concordances" between the major coding schemes would enable users of contracting data gain more context to have greater insight and benchmarking capabilities.
