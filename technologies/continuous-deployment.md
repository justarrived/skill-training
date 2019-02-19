# Learn Continuous Deployment

Continous Deployment is the idea that software in production is as close as possible to software in development at all times.
This limits the size of code that needs to be searched for bugs when problems surface in the production environment and enables 
teams to quickly roll back software to a known working version without inflicting users with regression of features.

This guide will provide a dive into Continous Deployment (CD).

Before starting it can be useful to familiarize yourself with [The 12 Factor App](https://12factor.net/) methodology.


## Steps

In this guide we will setup a basic CD pipeline on [Heroku](https://heroku.com) which will deploy code from [GitHub](https://github.com).


### Create a GitHub account.

* Go to [github.com](https://github.com) and register an account or use your existing one.

* Pick a repository or create a new basic project.
  For simplicity pick a project (language) that uses [one of Herokus officially supported buildpacks](https://devcenter.heroku.com/articles/buildpacks#officially-supported-buildpacks).

