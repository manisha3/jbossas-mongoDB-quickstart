JBoss AS Quickstart for MongoDB
===============================

This is a simple Red Hat OpenShift example containing a JavaEE6
servlet that illustrates some of the steps in the MongoDB Java
Tutorial: <http://www.mongodb.org/display/DOCS/Java+Tutorial>



Running on OpenShift
----------------------------

Create an account at https://www.openshift.com

Create a jbossas-7 application with mongodb (you can call your application whatever you want)

    rhc app create testmongo jbossas-7 mongodb-2

Add this upstream repo

    cd testmongo
    git remote add upstream -m master git://github.com/openshift-quickstart/jbossas-mongoDB-quickstart.git
    git pull -s recursive -X theirs upstream master

Then push the repo upstream

    git push

That's it, you can now checkout your application at:

    http://testmongo-$yournamespace.rhcloud.com/mongoDB


The quickstart code is licensed under the Apache License, Version 2.0:
http://www.apache.org/licenses/LICENSE-2.0.html

