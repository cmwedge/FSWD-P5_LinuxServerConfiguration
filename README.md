Udacity Full-Stack Web Developer Nanodegree Project 5: Linux Server Configuration
=================================================================================
##Overview
This README outlines the changes made to a bare Ubuntu distribution to secure it
and serve a previous project (the catalog application) for the final Full Stack
Web Developer nanodegree.

##Summary of Changes
* Software Installed
 - Full package update/upgrade
 - Apache2
 - git
 - libapache2-mod-wsgi
 - postgresql
 - python
 - pip
 - virtualenv
 - flask
 - sqlalchemy
 - bleach
 - oauth2client
 - http2lib
 - requests
 - psycopg2
 - sqlite
* Configuration Made
 - Changed SSH default port
 - Set firewall to limit deny traffic except on ports 2200, 80, and 123
 - Set timezone to UTC
 - Set initial git configuration (name, email)
 - Set up configuration for catalog application
 - Set up virtual environment / host for catalog application
 - Denied .git folder requests in apache
 - Set ServerName in apache
 - Set up grader user
 - Set up catalog database role
* Application Changes
 - The catalog application needed some updates to run successfully
 - Switched from sqlite to postgresql
 - Changed name of base file (application.py) to avoid name collisions with Flask
 - Added module paths in wsgi startup file
 - Changed name of users table to avoid collision with postgresql table
 - Updated references to users table in python code
 - Changed column type of last_update from integer to bigint


##Third-Party Sources
I made gratuitous use of the following websites for install/configuration:
* Digital Ocean
* StackOverflow / StackExchange
* Ubuntu
* PostgreSQL
* Udacity (forums)
* Flask

##Server Details

IP:
* 52.11.46.3

SSH Port:
* 2200

URL:
* http://52.11.46.3
