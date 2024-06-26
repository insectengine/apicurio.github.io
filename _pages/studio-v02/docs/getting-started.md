---
title: "Getting Started with Apicurio Studio"
layout: guide-v02
permalink: /studio-v02/docs/getting-started
slug: "getting-started"
excerpt: "This page will get you up and running with Apicurio Studio quickly!"
hidden: false
guide-v02: true
createdAt: "2017-07-18T11:05:58.247Z"
updatedAt: "2019-04-11T11:04:03.343Z"
---
This overview article explains how to download Apicurio Studio and run it locally. If you want to simply evaluate Apicurio Studio to see what it can do, you can try the [Live Version](https://studio.apicur.io/) first.

## Download the Quickstart
Obviously the first thing to do is download the Quickstart!  The latest version can always be found on the [Apicurio Studio web site](http://www.apicur.io/).  You can also find the [latest release directly on GitHub](https://github.com/Apicurio/apicurio-studio/releases).

## Running the Quickstart
As long as you run the quickstart on your local machine (localhost) and you have an internet connection, everything should work fine right out of the box.

> **Apicurio Studio Quickstart Authentication**
>
> The Apicurio Studio quickstart is configured to use an OpenShift Online instance of Keycloak for authentication.  This is great for running the quickstart locally, but is not suitable for production.

All you need to do is unpack the quickstart .zip file and then start up WildFly using the Apicurio configuration file:
```shell
cd ~/Downloads
unzip apicurio-studio-VERSION-quickstart.zip
cd apicurio-studio-VERSION
./bin/standalone.sh -c standalone-apicurio.xml
```
This will start up Apicurio Studio on localhost.

## Login to Apicurio Studio
Now that everything is up and running, you can log in to Apicurio Studio by using the following URL:

[https://localhost:8443/studio/](https://localhost:8443/studio/)

## Notes and Further Reading
The quickstart is designed to be run on localhost and is configured to use an H2 database.  Please see other articles in this knowledge base to learn about more advanced configuration options such as using a different database or running on an external server.