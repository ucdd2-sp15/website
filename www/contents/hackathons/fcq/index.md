---
title: FCQ
lead: FCQ
date: 2015-2-9
location: ATLAS Lounge
template: hackathon.jade
---

[FCQ](http://www.colorado.edu/fcq/) really needs a better website. Like the hackathon last week, a skeleton site has been made and is hosted at: [https://murmuring-stream-1490.herokuapp.com/](https://murmuring-stream-1490.herokuapp.com/). Ten [issues](https://github.com/ucdd2-sp15/fcq-express/issues) have been created for improving this skeleton site. How many can your team address in 150 minutes?

# Github

The Github repository for this site is at

<a href="https://github.com/ucdd2-sp15/fcq-express" class="btn btn-info">https://github.com/ucdd2-sp15/fcq-express</a>

# Data
This site's data on a mongodb server as three separate collections: `courses`, `instructors`, and `departments`.

The URL to connect to the server is:

`mongodb://ucdd:hackathon@ds043971.mongolab.com:43971/fcq`

Use the mongo shell to explore the data

    $ mongo ds043971.mongolab.com:43971/fcq -u ucdd -p hackathon

For each collection, find a document and examine what fields are available

    PRIMARY> db.courses.findOne()
    PRIMARY> db.instructors.findOne()
    PRIMARY> db.departments.findOne()

Try some queries

    PRIMARY> db.courses.find({'Subject':'CSCI'}).limit(3).pretty()

    PRIMARY> db.courses.find({'insname1':'GRUNWALD, DIRK C'}).pretty()

    PRIMARY> db.instructors.find({'name':'GRUNWALD, DIRK C'}).pretty()

    PRIMARY> db.departments.find({department:'CSCI'}).pretty()    

    PRIMARY> db.departments.find({department:'CSCI'}).pretty()


# Objective

Solve all the issues marked for the [hackathon](https://github.com/ucdd2-sp15/fcq-express/milestones) milestone.

# Q/A

* __Is the site going to be used at one point?__ Quite possibly. We may continue to build this site as the semester progresses.Some campus partners have expressed interests in using this site.

## Logistics

* __Who works on what?__ The work must be fairly distributed among the team members. The site's functionality is broken down into small, individual script files in [routes/](https://github.com/ucdd2-sp15/fcq-express/tree/master/routes) and template files in [views/](https://github.com/ucdd2-sp15/fcq-express/tree/master/views) and its subdirectories, to make it easy for concurrent development and to minimize conflicts.
* __How can I indicate that I've fixed an issue?__ Each time you've fixed an issue, make a commit. Suppose you've just fixed issue 1 and are ready to commit to your branch, write `fixed issue #1` in the commit message.

        $ git commit -a -m 'fixed #1'    

* __Should the site go live?__ Yes. You'ver practiced a couple times so far. It should be quite smooth. The team leader should publish the site to Heroku following this [instruction](https://devcenter.heroku.com/articles/getting-started-with-nodejs#prepare-the-app). You only need to do the [Set up](https://devcenter.heroku.com/articles/getting-started-with-nodejs#set-up) step and the [Deploy the app](https://devcenter.heroku.com/articles/getting-started-with-nodejs#deploy-the-app) step. Ask for help if you are stuck. 

# Time

2.5 hours

# Team

Work together with the same team from the previous week.

# Procedure

Use the same two-level fork-pull procedure you've done a few times so far.

1. __Fork.__ The team leader creates a fork (i.e., team's fork).
1. __Fork.__ Each team member creates a fork of this team's fork.
1. __Work.__ The team distributes works fairly to individual members to do.
1. __Pull.__ Once done, each team member makes a pull request to the leader.
1. __Pull.__ The leader merges all the pull requests and then make a single pull request to the course's repository (i.e., [https://github.com/ucdd2-sp15/fcq-express](https://github.com/ucdd2-sp15/nn-express)).

# Milestones

* [Issue 1](https://github.com/ucdd2-sp15/fcq-express/issues/1) (5 points)
* [Issue 2](https://github.com/ucdd2-sp15/fcq-express/issues/2) (5 points)
* [Issue 3](https://github.com/ucdd2-sp15/fcq-express/issues/3) (5 points)
* [Issue 4](https://github.com/ucdd2-sp15/fcq-express/issues/4) (5 points)
* [Issue 5](https://github.com/ucdd2-sp15/fcq-express/issues/5) (5 points)
* [Issue 6](https://github.com/ucdd2-sp15/fcq-express/issues/6) (5 points)
* [Issue 7](https://github.com/ucdd2-sp15/fcq-express/issues/7) (5 points)
* [Issue 8](https://github.com/ucdd2-sp15/fcq-express/issues/8) (5 points)
* [Issue 9](https://github.com/ucdd2-sp15/fcq-express/issues/9) (5 points)
* [Issue 10](https://github.com/ucdd2-sp15/fcq-express/issues/10) (5 points)

# Submission Template

Use the following template in the pull request message:

```markdown

# Team members
Who?
Who?
Who?
Who?

# Score
?/50

# URL
What Heroku URL to access this site? (e.g., https://frozen-tor-4197.herokuapp.com/)

```

