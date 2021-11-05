---
layout: lab
num: lab06-part2-ops
ready: true
desc: "Deployment Instructions"
assigned: 2021-11-05 11:01
due: 2021-11-19 23:59
github_org: "ucsb-cs148-f21"
---

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

<div class="grade" markdown="1">
**Graded**: ({{page.num}}-T) (30 pts) You earn these team points if your GitHub is updated with complete installation / deployment instructions in ./docs/DEPLOY.md, linked to from your README.md  
</div>

# Deployment Instructions
This part of the lab has a two-week performance period. 

One of the important aspects of Software Development that often gets overlooked in the academic curriculum is "operations".   

For your MVP, you already provided detailed deployment instructions in your GitHub README.md. In this lab, you will  

Operations refers to the things other than your code that are necessary to deploy a running application.  This includes:
* configuring the platform on which the software is deployed
* configuring external dependencies such as authorization servers, databases, API credentials, etc.
* configuring initial accounts (for example, accounts for admins, etc.)

Each of your production and QA applications has some "operations" that are necessary to get it deployed on Heroku.

This part of the assignment prepares an activity during [lab08](https://ucsb-cs148.github.io/f21/lab/lab08/). 

* In this lab, you'll prepare written deployment instructions and a video with deployment instructions.
* In [lab08](https://ucsb-cs148.github.io/f21/lab/lab08/), your team and another team in your section will swap instructions/videos, try them out, and provide feedback, both on the deploy instructions, and on the apps themselves.

## Part One: Written Deployment Instructions

Someone on your team should prepare a set of instructions with all of the steps necessary to start with nothing but "read only" access to your repo, and end with a running instance of your app on a platform (or multiple platforms) you support.  

While this is a team grade, it is likely that you'll assign one or more people from your team to focus on this, while other members of your team are working on fixing bugs or adding new features.  

So, please make `Deploy Instructions (lab06-ops)` a new story with at least one associated "issue" and track it on your Kanban board along with your other issues.  Ideally, whoever is working on these instructions is not *also* juggling working on a coding issue at the same time, so this is the only issue to which they are assigned while they are working on it.

### Share instructions, NOT credentials

The running instance that your instructions enable should be *entirely separate* from the running instances for your
own team.  That is:

* You should not share any database credentials
* You should not share any OAuth or Auth0 credentials
* You should not share any 3rd party API credentials (e.g. Firebase, Spotify, Google, etc.)
    
NOTE: If any of the 3rd party services require signing up with a credit card, please speak to the instructor.    
    
Instead of sharing the credentials, you should share *instructions for obtaining those credentials*,
and instructions for configuring those credentials for your application.

These instructions should be in Markdown format, and stored in a file called `/docs/DEPLOY.md` in your repo.
(It is ok to factor this out into separate pages also stored under `/docs` and linked to from `docs/DEPLOY.md`)
    
There should be a link to `./docs/DEPLOY.md` from your main `README.md` file of your repo, e.g.
    
```
* [Deployment Instructions](./docs/DEPLOY.md)
```

This replaces the `Installation Steps` Section you previously wrote in the README.MD file as per [lab04](https://ucsb-cs148.github.io/f21/lab/lab04/) instructions. 

## Part Two: Deployment Video (OPTIONAL)

<div class="card" style="width: 80%; margin-left:auto; margin-right:auto;">
<div class="card-body">
<h5 class="card-title">Note: This is optional</h5>
<h6 class="card-subtitle mb-2 text-muted">As such, I expect most teams may opt-out of doing it.</h6>
<p class="card-text">
So if it's optional, why am I even leaving this step in the lab?
</p>
<p class="card-text">
I've left this in, because if you
read though it, I think you'll see how making this as a video would kind of force you to make your written instructions
more clear and foolproof.   You'd definitely find any problems with the written instructions as you go through 
the steps to make the video.
</p>
<p class="card-text">
(For teams that DO do it, however, it will be taken into account in your final team evaluation as a plus.   
</p>
</div>
</div>


Working from your written deployment instructions, someone on your team should make a video where you follow the written deployment instructions yourselves,
step by step, and show what the deployment looks like.   

For guidance on making the video, you can again use the instructions [here](https://youtu.be/k0Je8ASh4jo) for advice on how to do this using Zoom and YouTube; you may also use another tool if you have access to one and prefer it.

If in the course of making that video, you end up showing
values of secrets (e.g. database passwords, OAuth tokens, etc.) you should go back and *invalidate* those tokens before
releasing the video.
    
Today, I suggest that you create a story on your Kanban board for the creation of the deployment video, and put it 
wherever you keep stories that are not ready to start yet; you will eventually assign that story to someone, but
you aren't ready to start it until you have the written instructions done.   

Ideally, the person that makes the video
should be different from the person that wrote the instructions.  That makes it more
likely that if there are any ambiguities, errors, or omissions in the instructions, you'll find them before the video
is finished.  But, this is a recommendation, not a requirement.
    
# Grading:

Team Grade: 30 points for successfully completing the instructions.
