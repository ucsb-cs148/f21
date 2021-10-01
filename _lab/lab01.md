---
assigned: 2021-10-01 11:00
desc: Getting Started
due: 2021-10-08 23:59
layout: lab
num: lab01
ready: false
signup_app: https://ucsb-cs-github-linker.herokuapp.com/
slack_url: https://ucsb-cs148-f21.slack.com
github_org_name: ucsb-cs148-f21

---

<div style="display:none">
https://ucsb-cs148.github.io/f21/lab/lab01/
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


## Announcements 

* COVID-19
* Making sure teams are all 4-6 students, accommodating students without groups
* Possibility to switch (as the whole team) from 11am to 12pm Lab Section
* TA will go over today's lab work (do be done in team groups) 


This lab has two components. One part to complete ASAP (Step 0 to Step 4 below, to be completed mostly today in Section or as soon as possible afterwards) and one graded part that is due by the end of next Friday, Oct. 8th 2021. One week is the typical time period for lab assignments. In each lab starting with next week (10/08), you should make sure as a team that you have completed all lab deliverables from the previous week. 

<div class="grade" markdown="1">

**Graded**: (20 pts) You earn these points if/only if:
* your group reached **Milestone 1** described below in Step 2, on top of which every member branched the team repo and did a pull request to submit a file named after themselves in the teams folder from their own branch, and the team together created a NORMS.md file.
This is the goal for Section today. 

Over the coming week: 

**Graded**: (20 pts) You earn these points if/only if:
* your group logged your first Scrum meetings (including `lab01.md` and `lec03.md`) in the `sprint00` subfolder. 
* you took accurate attendance, accounting for all members of your group
   (See the [teams page]({{'/teams_page/' | relative_url }}) for a list of group members)
* the meeting notes the scribe took are added to the above files. For future meetings, you will replace `lab01` with the respective meeting time denominator (e.g. `lec05` or `01-17-2pm`)

**Graded**: (20 pts) You earn these points if/only if:
* your group produced a problem scenario in the form of a github file './team/problem_scenario.md', and 
* a user journey documentation in the format of your choice. Summarize what you came up with in a file './team/user_journey.md'

**Graded (lab01-I)**: (20 pts) towards (lab01-I) is your individual grade for lab01.  Your mentor will check with each of the team members to see if they got a `Hello World` app running. These reviews can be as simple as pointing the mentor to a deployed heroku web app, or it could involve the team member demoing an app to the mentor via Zoom. Your TA or instructor will then do an independent assessment, informed by the mentors review, and assign a grade. If you are unsure about your code/project following good practice, you are encouraged to complete it early and meet with your mentor, your TA, or another mentor/TA during arranged meeting time or office hours to go over it in advance.
The components of this grade are listed below. These points cover the basic functionality and code of your Hello World app on the basis of the app review.  The remaining points cover mechanics of the release process (issues, version control, deployment/demos).

**Graded (lab01-T)**: (20 pts) (lab01-T) is your Team grade for lab01.  As part of this grade, each team member should have contributed to a hello world assignment as an individual or as part of a group by the due date/time of this lab, i.e.  ({{page.due |  date: "%a, %b %d at %l:%M%p"}})

For teams of 5, this part of your grade is 6 points per team member. For teams of 4, it is 7.5 points.  Those points are all or nothing; if you've made a reasonable attempt, even if you didn't earn 100% on lab01, your team will earn 6 or 7.5 points for your contribution towards the whole.

This component of your team grade is designed to encourage each team member to reach out to all the other members of the team, and be aware of the progress they are making towards the goal of having every team member complete a hello world assignment as an individual or as part of a pair. The most important learning goal of the course is to learn to work as a team, supporting one another.

</div>



## Step 0: Find your assigned seat and meet your mentors

Seating charts are here:

| Row | 11am | 12pm |
|-----|-----|-----|
|1 | **t01-sbrideshare** (Vincent, Alan)     &     **t02-clubrush** (Nagarjun, Zechen) | **t06-campusmaps** (Bryan, Zechen) |
|2 | **t07-musictaste** (Alan, Vincent)	     &     **t08-servedup** (Vincent, Alan) | **t09-studygroup** (Nagarjun, Zechen) |
|3 | **t03-fitnessguru** (Zechen, Alan) | **t10-animelist** (Bryan, Tobias) |
|RT Window | **t04-youtubevoice** (Bryan, Nagarjun) | **t11-typingtest** (Tobias, Vincent)	|
|RT Door | **t05-recipefinder** (Alan, Vincent)	|  | 
{:.table .table-sm .table-striped .table-bordered}


## Step 1: Create a CoE account if you don't have one already

You could do all the necessary work this quarter on your own computer, but very likely it will be convenient for you to test things with your team on a computer in one of the Computer Science Labs. 

To log on to the machines in the Computer Science labs, or to connect
remotely, you will need a **College of Engineering account**. You can create an account online at
<https://accounts.engr.ucsb.edu/create>.

If you are enrolled in <i>any</i> CoE course this quarter (including CS148), you
should be able to create your account immediately.

If you are not able to do so, you will need to contact the ECI Help Desk at <a href="mailto:help@engineering.ucsb.edu">help@engineering.ucsb.edu</a>.

## Step 2: Get setup with github and add yourself to our organization

We will be using github.com in this course. We have created an
organization called {{github_org_name}} on github.com where you can
create repositories (repos) for your assignments in this course.

The advantage of creating private repos under this organization is
that the course staff (your instructors and TAs) will be able to see
your code and provide you with help, without you having to do anything
special.

To join this organization, you need to do three things.

1. If you don't already have a github.com account, create one on the
"free" plan. Visit [https://github.com/](https://github.com/)

2. If you don't already have your @umail.ucsb.edu email address
associated with your github.com account. go to "settings", add that
email, and confirm that email address.

3. Visit our Github Sign Up Tool at <{{page.signup_app}}>.   Navigate to <{{page.signup_app}}>.  Login with your github.com account. Click "Home", find this course ({{site.course}}, {{site.qtr}}), and click the "Join course button".   That will automatically send you an invitation to join the course organization on github.

4. There should be a link to the invitation for the GitHub organization for this course (<https://github.com/{{site.github_org}}>). Click on the invitation link and accept it. You can also go straight to <https://github.com/{{site.github_org}}> and see the invitation there (if you're logged in). Accept the invitation that appears in your browser (from step 3) or log into your account on [https://github.com/](https://github.com/) to accept the invitation.

**Milestone 1**: Once all your team members have successfully joined the organization, send a message in your Slack team channel that states "Milestone 1 completed!". This is important, because we will run a program to automatically create GitHub repositories for your teams once all the teams in this Section have completed this milestone. 

### Step 2a: Decide where you will work

Your first step here is to decide whether you are going to work:
* on your own laptop/desktop system
* by ssh'ing into CSIL

Here are some of the pros and cons:

| Location | Pros | Cons |
|----------|------|------|
| Your own machine | Less likely to run out of disk space | Must install software |
| CSIL | No need to install software | May run out of disk space, especially for Next.js | 
{:.table .table-sm .table-striped .table-bordered}

Notes for running locally
* Installing software on your own machine is typically straightforward.  We can try to assist during course staff office hours.   Please know. however, that we cannot necessarily provide detailed tech support for every possible operating system version.   You will ultimately be resposible for dealing with any OS specific issues.

Note for running on CSIL
* On CSIL, disk space has typically not been an issue for Spring Boot.  However, next.js does typically take up quite a bit of disk space for dependencies and it is easy to blow past your disk quota.  This article describes some techniques for dealing with disk quota issue on CSIL: [CSIL: Disk Quota and File Quota issues](https://ucsb-cs48.github.io/topics/csil_disk_quota/)
* When running on CSIL, a web server running on `localhost` will not be accessible in your local browser unless you take
  special steps to make it accessible, such as setting up ssh port forwarding.  That process is described here: [CSIL: SSH Port Forwarding](https://ucsb-cs148.github.io/topics/csil_ssh_port_forwarding/)


### Step 2b: Install Git

Skip this step if you are working on CSIL; git comes pre-installed.

If you decide to work locally, you'll need at least git on your local machine. 

* For MacOS, open a terminal prompt and type `git --version` at the prompt.  If `git` is not installed, you'll be prompted to
  install the Command Line Tools part of XCode.   Proceed with the install, and afterwards you should have `git`
* For Windows, we recommend this installation: <https://git-scm.com/download/win>
  * This also provides the "git bash shell", which is a handy tool to have at your disposal.
* For Linux, it is likely that `git` comes pre-installed, but if not, consult the documentation for your distribution.
  * For distributions that use `apt`, it is likely `sudo apt update; sudo apt install git`
  * For distributions that use `yum`, it is likely: `sudo yum install git`

When you can type `git --version` at the command prompt on your system, and it shows a version rather than an error such as `command not found`, you are ready to proceed.

### Step 2c: Configure git

You may skip this step if you've already configured git on the machine where you are working.

### Step 2d: Configure name and email

When you use `git` to add commits to a project, it attaches your name and email to the commit as part of the metadata.

To configure this, type the following commands, substituting in your name in place of `Your Name` and your email in place of `you@example.com`.

```
git config --global user.name "Your Name"
git config --global user.email you@example.com
```

### Step 2e: Configure ssh keys

Configuring ssh keys for GitHub allows us to allows us to avoid having to type in our git password many times per session.  So while not strictly required, it is highly recommended.   All further instructions in the course will assume you have done this step; if you don't, you'll need to adjust the instructions to use `https` based urls instead of the SSH based ones that start with `git@github.com:`.

To configure your SSH keys for GitHub, follow these instructions.  

* <https://ucsb-cs148.github.io/topics/github_ssh_keys/>

Notes: 
* You should generate the keys on the system where you plan to work: generate the keys on CSIL if you plan to work on CSIL, and on your laptop if you plan to work on your laptop.
* If the `ssh-keygen` command is not available on your system, do a web search to try to determine how to install it for your platform.)

### Step 2f: Clone your repo

For this step, please wait until you get the ok from the instructors that your project group repos have been generated.

Then, on your computer of choice, `cd` in the directory where you plan to do your work for this course (e.g. perhaps `~/cs148`), type this command to clone your empty repo into that directory.   In place of `repo-url-goes-here`, copy the URL for the new repo you created.  That will be, for example: `git@github.com:ucsb-cs148-f21/cgaucho_lab00.git` but with `cgaucho` replaced with your GitHub id.

```
git clone repo-url-goes-here
```

That should create a new empty directory (well, almost empty) called `lab00-cgaucho`.  Use `cd lab00-gaucho` to put yourself in that directory.

If you then type `ls -a` you'll see that the directory is not completely empty. It contains a `.git` subdirectory, which is how you know that this is a git repo rather than an ordinary directory.

## Step 3: Each of you INDIVIDUALLY now makes a branch of the repo

The next step is done as an individual

* Clone the repo and make a branch of the repo that matches your name, e.g.
   ```
   cd repo-name-goes-here
   git checkout -b yourname
   ```


### Step 3a: Inside your branch of the repo, create a file called `team/your_first_name.md`

In your branch, NOT on the master branch of the main repo, please do the following:

Make a directory called `team`. Inside this, create a markdown file named `your_first_name.md` containing a brief description of you and of your ideas for the project. 

* NOTE: Not literally `team/your-first-name.md`, but something like `team/chris.md` or `team/taylor.md`

Each team member should do this individually. Note that this will be publicly displayed on the course site.
   
### Step 3b: Do a pull request from your branch that has your file called `team/your_first_name.md`.

Do a pull request from your branch to the master branch of the repo.  Each team member should have done at least
one pull request from their github id.
   
## Step 4: Create your team/NORMS.md file

This is a list of ideal team behaviors, e.g. everyone arrives to meetings on time or everyone starts things tasks early. You should write this as a team.  Only one student needs to submit a pull request containing this file, however it is ok
if there are multiple pull requests for this file.   You should be careful, however to avoid merge conflicts!

The `team/NORMS.md` file should contain all of the team norms.  It is ok to "suggest" team norms in your individual team/first-name.md files, but the team, ultimately, should consolidate all of these into one `team/NORMS.md` file.

<div class="grade" markdown="1">

**Graded**: (20 pts) You earn these points if/only if:
* your group reached **Milestone 1** described below in Step 2, on top of which every member branched the team repo and did a pull request to submit a file named after themselves in the teams folder from their own branch, and the team together created a NORMS.md file.

</div>

# To be completed over the coming week: 

## Step 5: Document your meetings

During [lec03]({{'/lec/lec03/' | relative_url }}), you have first practiced logging meetings in GitHub. Make sure to log today's meeting as well, and capture it as `lab01.md` in the `sprint01` folder you created in lecture. Reminder: In your github repository, you structure the documentation of your meetings into 'sprints' (which are week-long unless you as a team decide on a different interval). 

<div class="grade" markdown="1">

**Graded**: (20) You earn these points if/only if:
* your group logged `lec03.md` and `lab01.md` meetings in the `sprint01` subfolder. 
* you took accurate attendance, accounting for all members of your group
   (See the [teams page]({{'/teams_page/' | relative_url }}) for a list of group members)
* the meeting notes the scribe took are added to the above files. For future meetings, you will replace `lab01` with the respective meeting time denominator (e.g. `lec05` or `01-17-2pm`)
</div>

From now on, please document all your meetings in the github repository in this way.


## Step 6: Discuss the User Journey

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

**Graded**: (20) You earn these points if/only if:
* your group produced a problem scenario in the form of a github file './team/problem_scenario.md', and 
* a user journey documentation in the format of your choice. Summarize what you came up with in a file './team/user_journey.md'
</div>

## Step 7: Move towards minimum viable product (MVP)

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



## Development deliverables for lab01

As the Agile Methodology strives to get to a working live software as quickly as possible (to be improved constantly thereupon), it is now also time to experiment with potential technology stacks, so that your team has a good basis for choosing a particular implementation platform and framework in an informed fashion! 

By the due date of this assignment (i.e. {{page.due |  date: "%a, %b %d at %l:%M%p"}}), every team member (either individually or as part of a group of team members all following the same steps on their own host computers) should have created a simple running  `Hello World` app on a platform and with a technology stack of each person's choice. Variety among your team members w.r.t. the tried technologies will help you gather valuable information about the pros and cons of different choices, but it is not required that you all do something different. It is also ok to do this as a group experience or in breakout groups of 2 or 3 people. 

A `Hello World` app demonstration includes all of the following:
* Each team member has participated either as a solo programmer, or as part of a group (but with their own deployed demo), in producing a "Hello World" type app for a
   framework you are exploring for your project.  You will get two grades for this: one as part of your team grade, and another as
   an individual grade, as explained below.
* As a team, you've settled on the work you are going to do after the Hello World phase to move towards your minimum viable product (MVP).

More on this below, and on how we'll be assessing this for both a team and an individual grade.

<div class="grade" markdown="1">

**Graded (lab01-I)**: (30) towards (lab01-I) is your individual grade for lab01.  Your mentor will check with each of the team members to see if they got a `Hello World` app running. These reviews can be as simple as pointing the mentor to a deployed heroku web app, or it could involve the team member demoing an app to the mentor via Zoom. Your TA or instructor will then do an independent assessment, informed by the mentors review, and assign a grade. If you are unsure about your code/project following good practice, you are encouraged to complete it early and meet with your mentor, your TA, or another mentor/TA during arranged meeting time or office hours to go over it in advance.
The components of this grade are listed below. These points cover the basic functionality and code of your Hello World app on the basis of the app review.  The remaining points cover mechanics of the release process (issues, version control, deployment/demos).

**Graded (lab01-T)**: (30) (lab01-T) is your Team grade for lab01.  As part of this grade, each team member should have contributed to a hello world assignment as an individual or as part of a group by the due date/time of this lab, i.e.  ({{page.due |  date: "%a, %b %d at %l:%M%p"}})

For teams of 5, this part of your grade is 6 points per team member. For teams of 4, it is 7.5 points.  Those points are all or nothing; if you've made a reasonable attempt, even if you didn't earn 100% on lab01, your team will earn 6 or 7.5 points for your contribution towards the whole.

This component of your team grade is designed to encourage each team member to reach out to all the other members of the team, and be aware of the progress they are making towards the goal of having every team member complete a hello world assignment as an individual or as part of a pair. The most important learning goal of the course is to learn to work as a team, supporting one another.

</div>  


## What *each* "Hello World" branch/pull-request must contain for full credit.
   
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
the demonstration BEFORE the lab next Friday. The TAs hold 
office hours and you can arrange meeting times with your mentors during which you can schedule this demo.   The last opportunity to do this demo
is right after or just before lab on the due date for this assignment, if you can grab your mentor or TA, but it may not be possible to fit all of those in, and in that case, regrettably, you may lose the opportunity to do so (and earn the points.)  Please coordinate with your team to
get as many of these demos done *before* lab on the due date of this assignment.

If working in a pair/sub-group, *each* member of the pair should demo the app, to show that they understand how to run it.

NOTE: If you cannot schedule with your own mentor, you may coordinate on slack between your mentor and another mentor/TA holding open lab hours that better fit your schedule.  Please use the slack to coordinate this.  

## Some starting points for selected platforms: 

Vincent Tieu has put together [a Github repository with starter code for React and Google Authentication ](https://github.com/vincentktieu101/ReactGoogleAuthStarter) The README.md and [an accompanying YouTube video](https://www.youtube.com/watch?v=XZceEXlYC1w&amp;ab_channel=VincentTieu)  also cover how to use the Google Developer Console and how to host the application on Heroku. 

If you are using Heroku for hosting a web app, you may also find [these instructions from CS48 some time ago](https://ucsb-cs48.github.io/s20/lab/lab01/) helpful. 


