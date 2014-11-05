Pararell Deployment Sample
==
[![Build Status](https://travis-ci.org/nagaseyasuhito/sample-pararell-deployment.svg?branch=master)](https://travis-ci.org/nagaseyasuhito/sample-pararell-deployment)

Setup
--
    $ brew install tomcat
	$ git clone git@github.com:nagaseyasuhito/sample-pararell-deployment.git
	$ cd sample-pararell-deployment
    $ cp tomcat-users.xml $(brew info tomcat | grep "*" | awk '{ print $1 }')/libexec/conf
    $ catalina start
    $ mvn clean deploy
