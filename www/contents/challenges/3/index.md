---
title: Week
lead: Getting More Jaded
template: challenge.jade
---

Your learning challenge this week has two parts. 

First, for team co-learning, the topic will be, again, [Jade](http://jade-lang.com/). You will continue to improve our reversed-engineered knockoff version (i.e., `ucdd-jaded`).

Second, for individual learning, continue to develop your resume to make its contents as complete as possible, something you would be happy to show to a potential employer.

# Team Learning (50 points)

<span class='btn btn-danger'>IMPORTANT</span> New teams! Check the announcements for your new team assignment. We will spend the last 20 minutes of the Monday class for you to meet with your new teammates and get started on the week's team learning challenge.

## Objectives

Implement new capabilities for a template to

1. evaluate JavaScript expressions (e.g., `div= article.title`) 
1. iterate through an array to render contents for each array element (e.g., `for x in xs`).

## Github Repository

Your own fork of `ucdd-jaded`

<a href="https://github.com/ucdd2-sp15/ucdd-jaded" class="btn btn-info">https://github.com/ucdd2-sp15/ucdd-jaded</a>

You should work off your own fork. More skeleton code has been added. Grab new code from upstream by

	$ git pull

You should see these files added:

* `lib/ucdd-jaded.part2.js`: skeleton code to support the new features
* `lib/logic/forin.js`: skeleton code to implement the `for x in xs` feature. It currently has hard-coded output for a specific test case, but must be changed in order to pass other test cases more generally.
* `test.part2.js`: code to test the new features. It has five additional test cases (6 - 10). Initially, only two test cases can pass. Your team needs to work together to get all the test cases to pass.

## Milestones

1. Have passed `test6` (10 point)
1. Have passed `test7` (10 point)
1. Have passed `test8` (10 point)
1. Have passed `test9` (10 point)
1. Have passed `test10` (10 point)

## Due
11:59pm, Friday

## Time and Location

Each team decides on a time and location to meet before the submission deadline.

## Submission

Same as last week. The team leader should accept pull requests from team members, merge them, and make a single, combined pull request to the original repository (i.e., [ucdd2-sp15/ucdd-jaded](https://github.com/ucdd2-sp15/ucdd-jaded)).

Use the following Markdown template in the pull request message.

```
# Team members
Who?
Who?
Who?
Who?

# Score
?/50

# Meeting Location
where?

# Meeting Time
when? how long?

```

# Individual Learning (50 points)

Make your resume complete. Continue what you have already done during the [Resume Hackathon](../../hackathons/resume). Fill the resume page with your own contents. You should take this opportunity to make the resume as complete as possible so that you may share with an employer later.

## Github Repository

Your own fork of `resume`

<a href="https://github.com/ucdd2-sp15/resume" class="btn btn-info">https://github.com/ucdd2-sp15/resume</a>

## Milestones

* Personal Information (5 points)
* Work Experiences (10 points)
* Portfolio (10 points)
* Education (5 points)
* Skills (5 points)
* Honors (5 points)
* References (5 points)
* Published to gh-pages (5 points)

Note that these are exactly the same set of milestones as those in the Resume Hackathon. The major difference is that, this time, this resume must be about __YOU__.

## Due
11:59pm, Sunday

## Submission

* You do not need to make a pull request from your fork. You just need to make sure you commit your code and push this commit to your own Github fork. We will assume your most recent commit prior to the deadline is your submission. 
* Remember to include the points you've earned in the commit message.
* Make sure your resume is published successfully on `gh-pages` and can be accessed at `http://[your-github-account].github.io/resume`.
