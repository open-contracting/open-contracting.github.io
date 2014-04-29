---
layout: single
title: Docs - Blender
date: 29/04/2014
---
<div class="toc"></div>
### the problem
There are already many publishers (governments at country, federal, state, municipal level) publishing
open contracting data. But this information is not published in a consistent manner, people use their own field names,
publish their own unique set of fields, and use their own coding system.


### this repo
This project is structure as follows, please keep pull requests to this format:

    data/
    experiments/
    ocdata-blend/
        tests/
        visualization/

* data is where we can store sample data for testing against and working with. When committing to this directory, make sure that you have the right to republish the data, if not, just link to it.
* experiments - keep notebooks and other snippets where we play with the data, demonstrate approaches etc., does not need to be under test, try and name things clearly and  to document. All reusable / helper / util code should go into ocdata-blend. Whenever you do an experiment, please add an entry in the journal.md file so we can know what we've tried and what we've found.
* ocdata-blend contains all our code which we can wrap up into library to use elsewhere. All code in here, should be under test
* ocdata-blend/tests are the tests for the code in ocdata-categorize that will get shipped with the package
* ocdata-blend/visualization - any visualization front-end code to help us see our results


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
    $ mkvirtualenv ocdata-blend
    (ocdata-blend)$ pip install numpy
    (ocdata-blend)$ pip intall scipy
    (ocdata-blend)$ pip install -U scikit-learn
    (ocdata-blend)$ pip install pandas

Install the rest of the packages:

    (ocdata-blend)$ pip install nltk requests

To install iPython notebook

    (ocdata-blend)$ pip install pyzmq jinja2 tornado pygments ipython

### running the code

#### experiments
To run the experiments in the ipython notebooks, navigate at your command line to the directory with the notebooks in it. While in your virtual environment that you setup above:

    (.ocdata-blend)$ ipython notebook

Note that the latest version of ipython notebook allows folder navigation (hurrah!) so you can start your ipython notebook anywhere and navigate to your notebooks.
