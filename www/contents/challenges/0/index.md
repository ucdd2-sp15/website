---
title: Week 0
lead: Introduction to Learning Challenges
date: 2015-01-12
location: ATLAS Lounge
template: challenge.jade
---

# What is a learning challenge?

* __Learn by reverse-engineering__: You will be asked to implement your own _reduced_ version of a particular tool or library.
* __Learn in teams__: You will most likely to succeed if you learn together with your classmates in small teams. 
* __Visualize by screenshots__: You will take and submit screenshots to visually demonstrate that you've learned a topic, thereby fulfilling a learning challenge.
* __Flipped classroom__: You will do your learning __not__ in the classroom.

# Warmup: html-generator

<code>html-gen</code> is a small library providing a set of helper methods for generating HTML structures.

```javascript
	var html = require('./lib.js')
	html.generateHeading1('some heading text')
	
	// --> <h1>some heading text</h1>
```

## Prerequisites

These must be completed before the class.

* Have obtained access to a laptop (bring it!!)
* Have installed [Node.js](http://nodejs.org/)
* Have installed a text editor (e.g., [Sublime Text](http://www.sublimetext.com/)) for writing code
* Have created a Github account
* Have signed up for the [course announcements](https://github.com/ucdd2-sp15/announcements)

## Github Repository

<a href="https://github.com/ucdd2-sp15/ucdd-htmlgen" class="btn btn-info">https://github.com/ucdd2-sp15/ucdd-htmlgen</a>

<code>lib.js</code> is where all the library methods are implemented. Currently, only one method has been implemented.

<code>test.js</code> is a test script that invokes each of the library methods and print the return value of each method as a debug message.

![screen](screen.png)

<code>README.md</code> has instructions on how to run <code>test.js</code>.

# Part 1: Team Learning

In this course, we are taking a strong stance in promoting team-based collaborative learning. Thus, 50% of the points you can earn from each week's learning challenge will be through physical, face-to-face, team-based co-learning time. Normally, this co-learing time take place outside of the classroom. Only this week, we will practice co-learning in class.

## Objective

Each team member has learned to implement ONE function in <code>lib.js</code>

## Procedure

1. Form teams of four
1. Elect a team leader
1. The team leader creates a fork from the repository (i.e., [https://github.com/ucdd2-sp15/ucdd-htmlgen](https://github.com/ucdd2-sp15/ucdd-htmlgen))
1. Each member creates a fork from the team leader's fork
1. Each member works on his or her own fork. Implement ONE function in <code>lib.js</code>. Coordinate to ensure each member works on a different function.
1. Each member makes a pull request to the team leader's fork
1. The leader accepts and merges all pull requests from other members
1. The leader makes a single pull request to the original repository

## Submission

Normally, the deadline for your team's submission is __Friday 11:59pm__. For this exercise, the deadline is in ONE hour.

# Part 2: Individual Learning

Each week, after you've finished co-learning, you will spend the rest of the week to do individual learning to further enhance your knowledge and skill about a certain topic.

## Objective 
Implement ONE more function in <code>lib.js</code>

## Procedure

1. Continue to work on your fork
2. Commit and push your work to Github

## Milestones

1. Have implemented ONE more function
2. Have committed and pushed this implementation to one's own fork (no need to make a pull request)

## Submission

The individual learning part has two milestones. For each milestone, take a screenshot to visually document your accomplishment.

* __What screenshots to take?__ Discuss with your team members what screenshots make sense.
* __How to submit screenshots?__ For now, save your screenshots. Next, in today's hackathon, we will work together to build a website to post your screenshots.

Normally, the deadline for individual submission is __Sunday 11:59pm__. For this exercise, the deadline is in 30 minutes.

If you are able to finish early, you can continue to implement other functions, because you will be asked to do so for the [first learning challenge](../1).