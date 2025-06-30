# Group-Task-3- Docker and Java

**Team Members**
**Kate Abunassar**
**Soliana Getachew**

##  Description

This group project was created to practice using Docker to compile and run a simple Java application. The main task was to write a `HelloWorld.java` program, compile it, package it using Docker, and run it inside a container.

We followed a step-by-step guide to:
- Install the required tools (JDK, Docker, IDE)
- Write a basic Java program
- Build the project to generate `.class` files
- Create a `Dockerfile` for building a Docker image
- Run the image in a container and confirm it prints the correct message


---

## Use of Docker

Docker was used to create a lightweight container that runs our Java program in a controlled environment. Instead of relying on each team member having the same setup, Docker ensured consistency by using an image (`openjdk:23`) that contains everything needed to run the app.

The Dockerfile includes instructions to:
- Create a working directory
- Copy compiled Java files into the image
- Run the Java application (`Main.class`)

We used the following Docker commands:

docker build -t hello-java .
docker run hello-java
