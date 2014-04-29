---
layout: single
title: Docs - Open Data Comparison
date: 28/04/2014
---
<div class="toc"></div>
#### repo [https://github.com/open-contracting/opendatacomparison](https://github.com/open-contracting/opendatacomparison)

### about
A Django application for comparing datsets, built on Open Comparison. 

The site is being used to store our research and findings as we complete our supply side analysis for 
the OCDS project.

Links:

* The [live site](http://ocds.aptivate.org/opendatacomparison)
* [staging server](http://ocds.stage.aptivate.org/opendatacomparison) - feel free to request an account
* [Github issues](http://github.com/open-contracting/opendatacomparison/issues)

### install
Pre-requisites:

    MySQL (sudo apt-get install mysql-server)
    virtualenv (sudo apt-get install python-virtualenv)
    pip (sudo apt-get install python-pip)


Create your database in MySQL with utf-8:

    CREATE DATABASE opendatacomparison CHARACTER SET utf8


#### Linux
    cd deploy
    ./bootstrap.py # automatically creates a virtual environment and installs packages in it
    ./tasks.py deploy:dev

#### OSX
Using CLANG for compilation (CLANG throws errors on unexpected arguments by default):

    cd deploy
    ARCHFLAGS=-Wno-error=unused-command-line-argument-hard-error-in-future ./bootstrap
    ./tasks.py deploy:dev

#### Windows
Not yet tested, contributions welcome.

See [dye](http://github.com/aptivate/dye) for more information on our setup & deploy code.

### contributing
Contributions are gratefully received, some notes to keep the process and code consistent:

* Code should be pep8 compliant (your favorite code editor should be able to help with this)
* Submit your code via a pull request (read about [github pull request workflow](https://help.github.com/articles/using-pull-requests))
* All tests must pass
* Code coverage must not decrease (won't be strictly enforced until travis reporting is setup)

In return, you can expect a timely code review and response (if you haven't heard anything in a week - nag!)
Contributors who consistently submit good patches will be given core committing rights.

To add to the docs please submit a pull request against this page in the [open-contracting.github.io](http://github.com/open-contracting/open-contracting.github.io) repository.
