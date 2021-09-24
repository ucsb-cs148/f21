---
title: First MVP
layout: default
---

# First MVP

This document describes what should be in place at the end of the iteration where you deliver your minimum viable product,
i.e. the *smallest* (minimum) possible working software system that actually *delivers value to the user* (viable product) in some way

Deliver value means that it supports the user in:
* meeting a need, OR
* achieving a goal, OR
* satisfying a desire.

You should have a complete set:
* a complete set of users stories that are connected with this minimum viable product, as a result of the users story mapping exercise.
* a completed set of completed issues that support those user stories
* a "definition of done" for each user story (i.e. an acceptance test)
* pull requests that have been accepted into master, indicating for each which issues are addressed

All of the user stories and issues should be in the "Done" column of your Kanban board (or the equivalent, if you've expanded beyond "To Do", "In Progress" and "Done" at that point.

Here's a more complete version of the process.  We may or may not be able to incorporate all of these practices into our iterations (sprints) by the time we reach our first MVP, but by the end of the course, we should have at least sampled each of them:

* creating issues for those user stories
* doing point estimation on those user stories
* writing up acceptance tests for each of those user stories
* assigning a subset of those user stories to developers
* dragging those issues into the In-Progress column of your Kanban board
* writing unit tests and integration tests, as appropriate for those issues
* completing the issues
* doing QA on the code written for the issues, including:
  * checking against acceptance criteria
  * checking against coding standards, 
  * checking test coverage
  * checking for documentation (e.g. Javadoc for Java, docstrings for Python) 
* doing one or more pull requests for these issues to the master branch
* accepting those pull requests to deliver working software to the master branch.

