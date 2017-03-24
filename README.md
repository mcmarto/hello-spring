# hello-spring

This project started from the Spring Boot documentation - specifically the section title [Developing your first Spring Boot Application](http://docs.spring.io/spring-boot/docs/current/reference/html/getting-started-first-application.html).  Its purpose is to give me some experience of working with git (locally and via GitHub) and to provide a small application to allow me to experiment with and to learn about related topics. 

The application is a very simple Spring Boot web application which does nothing other than print "Hello World" to the browser.

# Building

To build it run

    ./mvnw package

or, if you are using Windows:

    ./mvnw.cmd package

This will download maven the first time you run it.

You should then be able to run the application with

    java -jar .\target\myproject-0.0.1-SNAPSHOT.jar

And browse to

    http://localhost:8080

to see 'Hello World'

# Docker

Docker support was added by following the guide at [Spring Boot with Docker](https://spring.io/guides/gs/spring-boot-docker/)

Build the docker container with

    mvn package docker:build

This is best done from within a Docker quickstart terminal for easy access to the docker environment. If you run it from a standard command prompt then you will need to set up the environment variables which point to your docker host.

Once the Docker image is built you should be able to see it listed (again, from Docker Quickstart shell) using

    docker images

You can then run your image with

    docker run -p 8080:8080 -t springio/myproject

And browse to 

    http://<docker-host-ip-address>:8080

to see *Hello World*
