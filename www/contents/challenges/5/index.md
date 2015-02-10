---
title: Week 5
lead: MongoDB Express
template: challenge.jade
---

Your learning challenge this week will be about [mongoDB](https://www.mongodb.org/). For the teaming learning component, your objective is to improve the two Express-based site your team has built, [Yelp Express](https://github.com/ucdd2-sp15/nn-express) and (2) [NN Express](https://github.com/ucdd2-sp15/nn-express), by connecting to a mongoDB server to retrieve data, rather than reading in static json files.

For the individual learning component, your objective is to build a dynamic site from scratch (almost) using the set of technologies you've learned so far: Jade, Express, and MongoDB.

# Team Learning (50 points)

## Objectives

1. Connect your team's Yelp Express site to a mongoDB server. 
1. Connect your team's NN Express site to a mongoDB server. 

## Data

Yelp and NN data are hosted in the cloud (i.e., [mongolab](https://mongolab.com/)) to be available for your site. You do not need to host your own mongodb server.

Server urls:

* Yelp: `mongodb://yelp:1234@ds039960.mongolab.com:39960/yelp`

* NN: `mongodb://nn:1234@ds053828.mongolab.com:53828/nn`

## Code

New code has been committed to yelp-express. Get the new code

    $ git pull

You will see these added:
    * mongo.js
    * mongo/doctorView.js
    * mongo/doctorList.js
    * mongo/restaurantView.js
    * mongo/restaurantList.js
    * mongo/userView.js
    * mongo/userList.js
    

Run the new express server entry script `mongo.js` (not `app.js`)  

    $ node mongo.js

`mongo/doctorView.js` and `mongo/doctorList.js` contain code exmples of getting data from mongodb.

For NN Express, there's no new example code given. You need to figure out on your own, following the example of Yelp Express.

## Learning Resources

* [try mongodb](http://try.mongodb.org/)
* [monk](https://www.npmjs.com/package/monk)

## Github Repository

<a href="https://github.com/ucdd2-sp15/yelp-express" class="btn btn-info">https://github.com/ucdd2-sp15/yelp-express</a>


<a href="https://github.com/ucdd2-sp15/nn-express" class="btn btn-info">https://github.com/ucdd2-sp15/nn-express</a>

## Milestones

1. Yelp Express
    - list users (5 points)
    - view user (5 points)
    - list restaurants (5 points)
    - view restaurant (5 points)
    - deploy to Heroku (5 points)
1. NN Express
    - view note (5 points)
    - list contexts (5 points)
    - view context (5 points)
    - list accounts (5 points)
    - view account (5 points)

(We skip the _list notes_ page because we don't want to handle pagination in mongoDB yet)

## Due
11:59pm, Friday

## Time and Location

Each team decides on a time and location to meet before the submission deadline.

## Submission

The team leader will again take individual teams' pull requests, merge them, and make a single pull request to the two original repositories, which are  [ucdd2-sp15/yelp-express](https://github.com/ucdd2-sp15/yelp-express) and [ucdd2-sp15/nn-express](https://github.com/ucdd2-sp15/nn-express).

Use the following Markdown template in the pull request message.

```
# Team members
Who?
Who?
Who?
Who?

# Score
?/50

# URL

which Heroku url to Yelp Express?

which Heroku url to NN Express?

# Meeting Location
where?

# Meeting Time
when? how long?

```

# Individual Learning (50 points)

Create a site to list and view a dataset. You can choose from these datasets:

* dataset 1 (TBA)
* dataset 2 (TBA)
* dataset 3 (TBA)

## Github Repository

<a href="https://github.com/ucdd2-sp15/my-express" class="btn btn-info">https://github.com/ucdd2-sp15/my-express</a>

## Requirements

* List and view pages for THREE collections (total six templates and routes)
* A search page that lists five interesting queries. Each query is a link one can click on to see the results of a query (similar to the search page of Yelp Express)

## Milestones

* List page (5 points)
* View page (5 points)
* List page (5 points)
* View page (5 points)
* List page (5 points)
* View page (5 points)
* Search page
    - interesting query 1 (5 point)
    - interesting query 2 (5 point)
    - interesting query 3 (5 point)
    - interesting query 4 (5 point)
    
## Due
11:59pm, Sunday

## Submission

* Make your own fork of [my-express](https://github.com/ucdd2-sp15/my-express)
* You do not need to make a pull request from your fork. You just need to make sure you commit your code and push this commit to your own Github fork. We will assume your most recent commit prior to the deadline is your submission. 
* Remember to include the points you've earned in the commit message.
* You do not need to get the site live on a public server.
