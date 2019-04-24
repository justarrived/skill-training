# Learn Continuous Deployment

Continous Deployment is the idea that software in production is as close as possible to software in development at all times.
This limits the size of code that needs to be searched for bugs when problems surface in the production environment and enables 
teams to quickly roll back software to a known working version without inflicting users with regression of features.

This guide will provide a dive into Continous Deployment (CD).

Before starting it can be useful to familiarize yourself with [The 12 Factor App](https://12factor.net/) methodology.


## Steps

In this guide we will setup a basic CD pipeline on [Heroku](https://heroku.com) which will deploy code from [GitHub](https://github.com).

This guide assumes you are familiar with GitHub. If you are unfamiliar with Heroku, please read more about it on [Wikipedia](https://en.wikipedia.org/wiki/Heroku).


### Setup GitHub account.

* Go to [github.com](https://github.com) and register an account or use your existing one.

* Pick a repository or create a new basic project.
  For simplicity pick a project (language) that uses [one of Herokus officially supported buildpacks](https://devcenter.heroku.com/articles/buildpacks#officially-supported-buildpacks).


### Setup Heroku account.

* Setup a [Heroku](https://heroku.com) account or use your existing one.

* Create your first Heroku app by following [Getting Started on Heroku](https://devcenter.heroku.com/start).


### Integrate GitHub with Heroku.

* Connect your Heroku app to your GitHub repo and setup automatic deploys
  [GitHub Integration](https://devcenter.heroku.com/articles/github-integration).
  
* Push code to `master` branch and have it deploy automatically.


### Configure Review Apps.

Review apps is an essential part of stable CD. It enables code to be tested properly before integrated into master. In order to understand how GitHub and Heroku works with review apps it is important to first understand Pull Requests in GitHub. You can read more about Pull Requests here: [About Pull Requests](https://help.github.com/articles/about-pull-requests/).

* Setup your Heroku app to use review apps 
  [GitHub Integration Review Apps](https://devcenter.heroku.com/articles/github-integration-review-apps). 
