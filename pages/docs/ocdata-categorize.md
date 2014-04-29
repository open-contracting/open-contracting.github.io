---
layout: single
title: Docs - OCData Categorize
date: 28/04/2014
---
<div class="toc"></div>
### repo
[github.com/open-contracting/ocdata-categorize](https://github.com/open-contracting/ocdata-categorize)

### the problem
There are already many publishers (governments at country, federal, state, municipal level) publishing
open contracting data. But this information is not published in a consistent manner, people use their own field names,
publish their own unique set of fields, and use their own coding system.

Building an understanding of the data that is already available is a vital part of our process in
building a first version of an open contracting data standard.

We have begun to work through the datasets by hand, but would like to use some classification / categorization 
techniques to speed up the process so we can work through more datasets.

In addition, this work should be of use later to help publishers see what areas they are already covering and which
they aren't so there is value beyond the initial supply side analysis.

#### the nitty gritty
What we are trying to classify is basically the column headings from csv files into standardized buckets.

What the buckets are continues to evolve, as we explore the data more, and although this maybe somewhat frustrating
from a developer point of view, it is a vital and useful part of building our standard.

See the repo [pycon-sprint-2014](http://github.com/open-contracting/pycon-sprint-2014/) for details of the initial
work that was done under the landscape directory.  At that time we tried to use 7 buckets:

* buyer - the person buying the good
* authority - the authority that's handling the procurement for the buyer
* supplier - the entity contracted to provide the goods/services
* solicitation - information about the initial tender notice / solicitation
* notice - notices are provided about solicitations, awards and contracts
* contract - information about the contract
* good - information about the good or service being contracted

The problem with this was that the distinction between solicitation, notice, and contract was 
hard for both us the humans and also the machine to distinguish (unsurprisingly given that the 
humans were confused).

We're currently working on new buckets.


### this repo
This project is structure as follows, please keep pull requests to this format:

    data/
    experiments/
    ocdata_categorize/
        tests/
        visualization/

* data is where we can store sample data for testing against and working with.
When committing to this directory, make sure that you have the right to republish the data,
if not, just link to it.
* experiments - keep notebooks and other snippets where we play with the data,
demonstrate approaches etc., does not need to be under test, try and name things clearly and 
to document. All reusable / helper / util code should go into ocdata-categorize. Whenever you do an experiment, please add an entry in the journal.md file so we can know what we've tried and what we've found.
* ocdata_categorize contains all our code which we can wrap up into library to use 
elsewhere. All code in here, should be under test
* ocdata_categorize/tests are the tests for the code in ocdata-categorize that
will get shipped with the package
* ocdata_categorize/visualization - the d3 code that lets us display and interact with the
results of categorization


### install
This repo uses packages like scipy and scikit-learn which need to be compiled and so are
available as binaries for many operating systems. 

Get your virtual environment setup (Ubuntu):

    # Install the necessary libraries and get your virtualenv setup
    $ sudo apt-get install python-pip python-dev build-essential 
    $ sudo pip install virtualenv virtualenvwrapper
    $ mkdir ~/.virtualenvs
    $ echo "export WORKON_HOME=~/.virtualenvs" >> ~/.bashrc
    $ echo "source /usr/local/bin/virtualenvwrapper.sh" >> ~/.bashrc 
    $ echo "export PIP_VIRTUALENV_BASE=~/.virtualenvs" >> ~/.bashrc 
    $ source ~/.bashrc 

To install everything in a virtual environment on Ubuntu (the order is important - I have had issues otherwise):
    
    $ sudo apt-get install libatlas-base-dev gfortran # needed for compiling
    $ mkvirtualenv ocdata-categorize
    (ocdata-categorize)$ pip install numpy
    (ocdata-categorize)$ pip intall scipy
    (ocdata-categorize)$ pip install -U scikit-learn
    (ocdata-categorize)$ pip install pandas

Install the rest of the packages:

    (ocdata-categorize)$ pip install nltk requests

To install iPython notebook

    (ocdata-categorize)$ pip install pyzmq jinja2 tornado pygments ipython

### running the code

#### experiments
To run the experiments in the ipython notebooks, navigate at your command line to the directory with the notebooks in it. While in your virtual environment that you setup above:

    (.ocdata-categorize)$ ipython notebook

Note that the latest version of ipython notebook allows folder navigation (hurrah!) so you can start your ipython notebook anywhere and navigate to your notebooks.

### data pre-processing
In order to be able to work with the column headers we need to split them into constituent words, sometimes we get headers like ````org_contactemail```` which we want split into ````org, contact, email````. The method words/split_words.py handles this for us.
