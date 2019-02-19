# Learn Docker

This document outlines how to learn Docker. 
If you are completely unfamiliar with Docker, please consult the following resources.
Don't expect to understand the Docker concept immediately. Especially if you have little or no DevOps experience.

* [Wikipedia](https://en.wikipedia.org/wiki/Docker_(software))
* [Why Docker](https://www.docker.com/why-docker)

**In short, Docker solves the following head aches common in software development and deployment.**

* Onboard faster and stop wasting hours trying to set up development environments, spin up new instances and make copies of production code to run locally.

* Enable polyglot development and use any language, stack or tools without worry of application conflicts.

* Eliminate environment inconsistencies and the "works on my machine" problem by packaging the application, configs and dependencies into an isolated container.


## Steps

### Setup

Docker runs as an engine on your local computer which powers Docker Images. 
An Image contains all the information to represent a complete, standalone computer. 

Follow the below link to register and account with Docker and install and setup Docker on your computer.

* [Get Started with Docker](https://www.docker.com/get-started)


### Familiarize yourself with Docker

Get down and dirty with the first steps of Docker by following the guide below.

* [Get Started, Part 1: Orientation and setup](https://docs.docker.com/get-started/)
* [Get Started, Part 2: Containers](https://docs.docker.com/get-started/part2/)


### Run your own application in Docker

Examples are all good and well, but nother beats the hands on experience of having run your own application in Docker.

* Pick a simple application you have created yourself.
  If your application have external dependencies like a database it is a little more work to get it working. 
  If you are unfamiliar with networking it is better to pick a project without external dependencies.

* Find a suitable base image from [Docker Hub](https://www.docker.com/products/docker-hub).

* Create a `Dockerfile` to setup your image.

* Iterate on your `Dockerfile` until your application can run on your local computer.
