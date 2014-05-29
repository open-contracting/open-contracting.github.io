---
layout: single
title: User Stories and Use Cases
redirect_from: /pages/notes/workshops/2014-04-Montreal/use-cases.html
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

* James McKinney describes how the [Popolo project](http://popoloproject.com/) developed use cases by looking at the demand side (especially what civil society organizations wanted in terms of legislative data) and looking at what existing standards had terms for (an indirect indication of needs, since those standards must have been created to fulfill use cases). The resulting "use cases and requirements" sections are brief summaries that describe particular data elements that might be valuable to a user, giving examples. The Popolo project also collects use cases and requirements through a [mailing list](http://lists.w3.org/Archives/Public/public-opengov/) and [issue tracker](http://popoloproject.com/specs/person.html). If at least two groups have a need for something, that’s usually sufficient reason to add it to the spec. The project target audience are tech-savvy civil society organizations.

We are exploring a hybrid approach, captured in the draft [template](template.html) which is being filled out based on desk research and conversations with potential users of open contracting data.

## Questions for Open Contracting user stories & use cases:

1. Should our user stories and use cases be based upon real people, or generalised cases? 

2. Should we have a standard format or different kinds of use cases?

# Draft Open Contracting User Stories

<ul>
{% for page in site.pages %}
{% if page.type == "usecase" %}
<li><a href="{{ page.url }}">{{ page.title }}</a> ({{ page.status }})</li>
{% endif %}   <!-- resource-p -->
{% endfor %} <!-- page -->
</ul>
