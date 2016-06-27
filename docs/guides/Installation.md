# Installation

## Requirements

* WebServer with PHP 5 or later
* mySQL Database version 5.5 or later
* [ExpressionEngine Core CMS](https://store.ellislab.com/#ee-core)
* [EE LTI Module](https://bitbucket.org/sijpkes/ee3-lti-module/src/a11a43632b3a65f1a36e5d0b70566f24d79ef456/?at=extension_hooks)
* [EE Peer Assessment Plugin](https://bitbucket.org/sijpkes/lti-peer-assessment)
* Git version control system

## Steps

1. Download and install a webserver (Apache is recommended), PHP 5, mySQL, git and [ExpressionEngine Core CMS](https://store.ellislab.com/#ee-core)

    _There are countless resources on the web to install the above online.  The suggested items are all open source or free_

2. Clone and Install the ExpressionEngine Modules
  The most up to date version of the application is available on Bitbucket and comes in two parts,
  the [EE LTI Module](https://bitbucket.org/sijpkes/ee3-lti-module/src/a11a43632b3a65f1a36e5d0b70566f24d79ef456/?at=extension_hooks) and the [Peer Assessment Plugin](https://bitbucket.org/sijpkes/lti-peer-assessment)

        git clone https://sijpkes@bitbucket.org/sijpkes/ee3-lti-module.git

3. change the name of the folder to learning_tools_integration
4. copy the entire folder to:

        /system/users/addons

5. Clone the Peer Assessment Plugin

        git clone https://sijpkes@bitbucket.org/sijpkes/lti-peer-assessment.git

6. Repeat steps 3 & 4 for the peer assessment module (you don't need to change the folder name)
