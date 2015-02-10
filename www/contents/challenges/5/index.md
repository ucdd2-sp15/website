---
title: Week 5
lead: MongoDB Express
template: challenge.jade
---

Your learning challenge this week will be about [mongoDB](https://www.mongodb.org/). For the teaming learning component, your objective is to improve the two Express-based site your team has built--[Yelp Express](https://github.com/ucdd2-sp15/nn-express) and [NN Express](https://github.com/ucdd2-sp15/nn-express), by connecting them to a mongoDB server to retrieve data, rather than reading data from static json files.

For the individual learning component, your objective is to build a dynamic site from scratch (almost) using the set of technologies you've learned so far: Jade, Express, and MongoDB.

# Team Learning (50 points)

## Objectives

1. Connect your team's Yelp Express site to a mongoDB server. 
1. Connect your team's NN Express site to a mongoDB server. 

## Data

Yelp and NN data are hosted in the cloud (i.e., [mongolab](https://mongolab.com/)) to be available for your site. You do not need to host your own mongodb server.

Urls to use in the code to connect to the servers:

* Yelp: `mongodb://yelp:1234@ds039960.mongolab.com:39960/yelp`

* NN: `mongodb://nn:1234@ds053828.mongolab.com:53828/nn`

## Learning Resources

* [try mongodb](http://try.mongodb.org/)
* [Getting Started with the mongo shell](http://docs.mongodb.org/v2.2/tutorial/getting-started-with-the-mongo-shell/)
* [monk](https://www.npmjs.com/package/monk)

## Shell

It is a good idea to practice using the mongo shell to test out queries and see results.

__Yelp__

Start mongo shell and connect to the Yelp dataset

    $ mongo ds039960.mongolab.com:39960/yelp -u yelp -p 1234

Find the first document of the _business_ collection

    PRIMARY> db.business.findOne()

And you will see a document shown like below:

```
{
    "_id" : ObjectId("544e139631f3775756ac4ab8"),
    "business_id" : "vcNAWiLM4dR7D2nwwJ7nCA",
    "full_address" : "4840 E Indian School Rd\nSte 101\nPhoenix, AZ 85018",
    "hours" : {
        "Tuesday" : {
            "close" : "17:00",
            "open" : "08:00"
        },
       
        ....
```

Queries to get the first document of each collection:

    PRIMARY> db.business.findOne()
    PRIMARY> db.user.findOne()
    PRIMARY> db.tip.findOne()
    PRIMARY> db.checkin.findOne()

You will only need to use _db.business_ and _db.user_ for this challenge.

__NatureNet__

Start mongo shell and connect to the NN dataset

    $ mongo ds053828.mongolab.com:53828/nn -u nn -p 1234

Queries to get the first document of each collection:

    PRIMARY> db.notes.findOne()
    PRIMARY> db.accounts.findOne()
    PRIMARY> db.contexts.findOne()

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

For Yelp Express, `mongo/doctorView.js` and `mongo/doctorList.js` contain code exmples of sending a query to a remote mongodb server and getting data back.

For NN Express, there's no new example code given. You need to figure out on your own, following the example of Yelp Express.

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

(We skip the _list notes_ page because we don't want to handle pagination in mongodb, at least not yet)

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

Create a site to list and view Github data about our class. 

## Github Repository

<a href="https://github.com/ucdd2-sp15/my-express" class="btn btn-info">https://github.com/ucdd2-sp15/my-express</a>

## Data

There are four collections. Choose any TWO of these collections:

* repos (all repos of [ucdd-sp15](https://github.com/ucdd2-sp15))
* events (last 30 events of [ucdd-sp15](https://github.com/ucdd2-sp15))
* pulls (pulls requests of [nn-express](https://github.com/ucdd2-sp15/nn-express))
* issues (issues of [nn-express](https://github.com/ucdd2-sp15/nn-express))

Static versions of these data are stored in `data/` for you convenience.

Server URL: `mongodb://github:1234@ds041871.mongolab.com:41871/github`


Connect to the shell:

    $ mongo ds041871.mongolab.com:41871/github -u github -p 1234

Queries to try:

    PRIMARY> db.repos.findOne()
    PRIMARY> db.events.findOne()
    PRIMARY> db.pulls.findOne()
    PRIMARY> db.issues.findOne()

## Requirements

* List and view pages for TWO collections. In total, you will implement four templates and four routes.
* The skeleton code is nearly empty, on purpose, taking off training wheels. You will practice creating your own Express app and adding other necessary files or npm packages from scratch. Use nn-express and yelp-express as examples.

## Milestones

* List page I (10 points)
* View page I (10 points)
* List page II (10 points)
* View page II (10 points)
* Deploy to Heroku (10 points)
    
## Due
11:59pm, Sunday

## Submission

* Make your own fork of [my-express](https://github.com/ucdd2-sp15/my-express)
* You do not need to make a pull request from your fork. You just need to make sure you commit your code and push this commit to your own Github fork. We will assume your most recent commit prior to the deadline is your submission. 
* Last week, you were not asked to deploy the app live. This week, you will need to be able to deploy the app to Heroku.
* __NEW__ : In the commit message, include
    - Points you've earned
    - Heroku URL to your Express app
