---
assigned: 2021-04-09 13:00
desc: 'First Project Increment: Hello World, and launch'
due: 2021-04-16 14:00
github_org: ucsb-cs148-w21
layout: lab
num: lab01
ready: true

---

<div style="display:none">
https://ucsb-cs148.github.io/s21/lab/lab01/
</div>

<style>
div.grade { margin: 2em; padding: 1em; border: 2px solid #0c0; background-color: #efe; }   
</style>

<div style="float:right; width: auto;">

<table style="margin-top:1em;">
<tr>
   <th>Points</th>
</tr>
<tr>
   <td class="pointCount"></td>
</tr>
</table>

</div>



# Step 1: Checking over your deliverables for [lab01]({{'/lab/lab01/' | relative_url }}) 

Deliverables are due today for [lab00]({{'/lab/lab00/' | relative_url }}) .   Check over them and make sure these are complete by the end of Section today.
The mentors/TAs will start the official grading after this lab ({{page.num}}) is complete this evening.  So this is your last opportunity for those points.

# Step 2: Document your meetings

During [lec03]({{'/lec/lec03/' | relative_url }}), you have first practiced logging meetings in GitHub. Make sure to log today's meeting as well, and capture it as `lab01.md` in the `sprint01` folder you created in lecture. Reminder: In your github repository, you structure the documentation of your meetings into 'sprints' (which are week-long unless you as a team decide on a different interval). 

<div class="grade" markdown="1">

**Graded**: (20 pts) You earn these points if/only if:
* your group logged `lec03.md` and `lab01.md` meetings in the `sprint01` subfolder. 
* you took accurate attendance, accounting for all members of your group
   (See the [teams page]({{'/teams_page/' | relative_url }}) for a list of group members)
* the meeting notes the scribe took are added to the above files. For future meetings, you will replace `lab01` with the respective meeting time denominator (e.g. `lec05` or `01-17-2pm`)
</div>

From now on, please document all your meetings in the github repository in this way.


# Step 3: Discuss the User Journey

As a team, discuss the "user journey" for your proposed application. 

That is, try to describe all of the events that lead someone to seek out your product and have an interaction with it, or perhaps a series of interactions. 

There should be a beginning, a middle and an end, where **value is exchanged**: 
* the user came with a *goal, need, or desire*, and 
* that goal was *met*, that need was *satisfied*, or that desire was *fulfilled*. 

Identify: 
* What is that goal, need or desire?
* What is the series of events, in chronological order?

Discuss this with your group, and capture (perhaps in a Google Doc?) whatever comes to mind.  

The beginning of your user journey is a *Problem Scenario* as discussed in class, which is basically a short story, involving a subset of the concrete *Personas* you came up with in assignment *h02* and expressing what the people eventually will want to achieve with your product and what the problem is with current solutions.

Beyond the problem scenario, you can document the design of your user journey in free form. 

At this stage, it is important to get the ideas flowing.  There is no specific "right or wrong" way to get your ideas down on paper (or, rather, eventually, a GitHub markdown file).  Just write something
that captures the group consensus, or the candidate proposals, for the "user journey".

It can take any form: a list, or pictures,  a collection of <tt>As a __ I can __ so that __ </tt> type stories, or any combination of those.  Don't get bogged down on what form it takes.  Just get something down.

NOTE: Try to keep your description VERY HIGH LEVEL, avoiding specific implementation details.

* Good:  User selects a beverage from among several choices
* Too much detail: User clicks on a drop down menu; each beverage has an image which flashes with an animation as you hover over it, etc. etc. 

You don't have to do this "perfectly" the first time.  You may need to first get it all out as "brain dump" that contains too much detail, and then move to a higher level.  But get to the higher level as soon as you can.

Don't move on to the next step until you have the "spine" of your customer journey captured in some fashion.

You'll know you have it, and you are ready for this step when:

* It tells a coherent story.  You can describe this to any reasonable person 
   (e.g. a UCSB student that isn't in this class, particularly one that might be a target user) 
   and they will be able to follow what you are saying.
* None of your "spine" should be "implementation" focused.  It shouldn't depend, for example, even on whether
  it happens to be a webapp, or a mobile app, or even an app at all. It shoudn't depend on technology specifics.

* The <b>value exchange</b> part is clearly identified: the goal/need/desire of the user, and how that gets acheived/met/fulfilled

<div class="grade" markdown="1">

**Graded**: (20 pts) You earn these points if/only if:
* your group produced a problem scenario in the form of a github file './team/problem_scenario.md', and 
* a user journey documentation in the format of your choice. Summarize what you came up with in a file './team/user_journey.md'
</div>

# Step 4: Move towards minimum viable product (MVP)

(This step is not graded, per se, but you can't meaningfully accomplish later stages if you try to skip it.)

At the moment, you have an idea and scenarios for your application.

At this stage, the story you have might have gone in one of two directions:

* **Grand Vision** (GV): You might have a story that really is very much your "ideal dream state" of the application when fully built out.   Keep in mind that this may be far more than you can reasonably accomplish in the next 8 weeks.
* **Minimum Viable Product** (MVP) You might have already been thinking in terms of "minimal viable product", and you might have a really nice thin slice of value for your end user, something you might *actually* be able to deliver in, say 4 weeks (or 1 week, or even 1 day.)
   
It's likely that each of our teams will be somewhere on the spectrum between these two extremes.  Discuss where you think
your team is on that spectrum.
   
Assuming that your team is somewhere closer to GV than to MVP, you'll now want to set aside the description of your
GV for the moment.  Use it as a reference to inform your efforts to redo the exercise, but focusing on an MVP.

Maybe you can draw on top of your GV description, and highlight the parts that you think might
be part of your MVP.

The big question to keep in mind is:

> How can we make "this" possible for the user with less complexity, less code, less time

Here, "this" is the goal/need/desire.



# Development deliverables for lab01

As the Agile Methodology strives to get to a working live software as quickly as possible (to be improved constantly thereupon), it is now also time to experiemtn with potential technology stacks, so that your team has a good basis for choosing a particular implementation platform and framework in an informed fashion! 

By the due date of this assignment (i.e. {{page.due |  date: "%a, %b %d at %l:%M%p"}}), every team member (either individually or as part of a group of team members all following the same steps on their own host computers) should have created a simple running  `Hello World` app on a platform and with a technology stack of each person's choice. Variety among your team members w.r.t. the tried technologies will help you gather valuable information about the pros and cons of different choices, but it is not required that you all do something different. It is also ok to do this as a group experience or in breakout groups of 2 or 3 people. 

A `Hello World` app demonstration includes all of the following:
* Each team member has participated either as a solo programmer, or as part of a group (but with their own deployed demo), in producing a "Hello World" type app for a
   framework you are exploring for your project.  You will get two grades for this: one as part of your team grade, and another as
   an individual grade, as explained below.
* As a team, you've settled on the work you are going to do after the Hello World phase to move towards your minimum viable product (MVP).

More on this below, and on how we'll be assessing this for both a team and an individual grade.


# Grading for {{page.num}}

<div class="grade" markdown="1">

**Graded (lab01-I)**: (30 pts) towards (lab01-I) is your individual grade for lab01.  Your mentor will check with each of the team members to see if they got a `Hello World` app running. These reviews can be as simple as pointing the mentor to a deployed heroku web app, or it could involve the team member demoing an app to the mentor via Zoom. Your TA or instructor will then do an independent assessment, informed by the mentors review, and assign a grade. If you are unsure about your code/project following good practice, you are encouraged to complete it early and meet with your mentor, your TA, or another mentor/TA during arranged meeting time or office hours to go over it in advance.
The components of this grade are listed below. These points cover the basic functionality and code of your Hello World app on the basis of the app review.  The remaining points cover mechanics of the release process (issues, version control, deployment/demos).

**Graded (lab01-T)**: (30 pts) (lab01-T) is your Team grade for lab01.  As part of this grade, each team member should have contributed to a hello world assignment as an individual or as part of a group by the due date/time of this lab, i.e.  ({{page.due |  date: "%a, %b %d at %l:%M%p"}})

For teams of 5, this part of your grade is 6 points per team member. For teams of 4, it is 7.5 points.  Those points are all or nothing; if you've made a reasonable attempt, even if you didn't earn 100% on lab01, your team will earn 6 or 7.5 points for your contribution towards the whole.

This component of your team grade is designed to encourage each team member to reach out to all the other members of the team, and be aware of the progress they are making towards the goal of having every team member complete a hello world assignment as an individual or as part of a pair. The most important learning goal of the course is to learn to work as a team, supporting one another.

</div>  


# What *each* "Hello World" branch/pull-request must contain for full credit.
   
* Each individual or pair should have built a hello world app suitable for your framework.
* You should have instructions in your ReadMe on what software must be installed in order to deploy your app. 
   A TA, Mentor, or another class member should be able to follow these instructions and successfully deploy your app.
* The app does not have to have any particular functionality other than what is normal for the framework.  It should display
   either the text "Hello, World", or something similar such as "Welcome to the foobar app" (where "foobar" is the name of your
   team's app.) To get full credit here you must also:
   * Have a *branch and a pull request* for your hello world app (the one that you did as an individual or as part of a sub-group) by the due date of this assignment (i.e. {{page.due |  date: "%a, %b %d at %l:%M%p"}})
and: 
   * deployed your app live on the public web (if it is a webapp) through Heroku, or another provider, *or* demoed your app to your mentor during open lab hours, or another mentor if that doesn't work for your schedule.

* By functionality normal to the framework, we mean for example:
   * If it a "game", there should be a "start game" button, and then after a moment, it displays "game over" with a "play again" button.
   * If it is a mobile app, it should have the most basic UI feature that are expected for the app to be "well-behaved" on the iOS or Android platform.  
   * If it is a webapp, it should be formatted as an HTML page, not just a plain text page with the words "Hello World". (Full navigation can come later, though it's nice if you can include it at this stage.)
* In no case should there be a "crash" if/when users interact with the app in a reasonable fashion.  

## *Each* webapp "Hello, World" branch/pull-request should be deployed

If your app is being deployed as a webapp: you should have have DEPLOYED it so that it runs on a service such as Heroku, Google App Engine, Amazon Web Services, etc. at a stable URL. The easiest platform on which to do this
for Java Spring Boot, and Python Flask is Heroku.   If you don't know how to go about it, ask on the slack channel (well in advance, not at the last minute), 
and mentors and other students can point you to the resources to get started with this.

Put the URL of your running app in the README in your branch.

## *Each* non-webapp "Hello, World" branch/pull-request should be demoed

If you are NOT doing a webapp, you must set up a time with your mentor, or your TA, to demo your app to them. Mobile apps should be demoed deployed on a physical device through Zoom. You need to do 
the demonstration BEFORE the lab next Thursday/Friday. The TAs hold 
office hours and you can arrange meeting times with your mentors during which you can schedule this demo.   The last opportunity to do this demo
is right after or just before lab on the due date for this assignment, if you can grab your mentor or TA, but it may not be possible to fit all of those in, and in that case, regrettably, you may lose the opportunity to do so (and earn the points.)  Please coordinate with your team to
get as many of these demos done *before* lab on the due date of this assignment.

If working in a pair/sub-group, *each* member of the pair should demo the app, to show that they understand how to run it.

NOTE: If you cannot schedule with your own mentor, you may coordinate on slack between your mentor and another mentor/TA holding open lab hours that better fit your schedule.  Please use the slack to coordinate this.  

# Some starting points for selected platforms: 

Vincent Tieu has put together [a Github repository with starter code for React and Google Authentication ](https://github.com/vincentktieu101/ReactGoogleAuthStarter) The README.md and [an accompanying YouTube video](https://www.youtube.com/watch?v=XZceEXlYC1w&amp;ab_channel=VincentTieu)  also cover how to use the Google Develop Console and how to host the application on Heroku. 

If you are using Heroku for hosting a web app, you may also find [these instructions from CS48 a year ago](https://ucsb-cs48.github.io/s20/lab/lab01/) helpful. 

# Starting Sprint02 
Some time during or after this Lab Section, you will enter Sprint02. This may be different for each of the teams - it depends on when you do your sprint review and sprint planning meetings. In any case, when you switch over to Sprint02, please create a new team/sprint02 directory in your GitHub and document all your sprint02 meetings in that directory from there on. 
