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
