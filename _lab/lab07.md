---
layout: lab
num: lab07
ready: true
desc: "User Flow, Start Manual, Continue Design Document, Retro 3"
assigned: 2021-11-12 11:00
due: 2021-11-19 11:59
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

**Graded**: ({{page.num}}-T) (40 pts) You earn these team points if you a) expanded the Design Document by summarizing important team decisions referring to meetings logged in your GitHub repo, and b) created a new Section in your Design Document talking about your User Experience (UX) considerations. A high-level task/user flow (see below) might be the first thing to document there, and it will also be helpful for determining the structure of your manual (see next bullet).

**Graded**: ({{page.num}}-T) (40 pts) You earn these team points if you started a user manual document that you link to in your Github ./docs/MANUAL.md and that contains at the very least a description of the product purpose, lists the intended user audience, and has section headings (which are allowed to change later on) with placeholder information (could even be [Lorem Ipsum text](https://www.lipsum.com/) for now) that in the future should document the various features of your product and how to operate them (with plenty of screenshots).  

**Graded**: ({{page.num}}-T) (20 pts) You earn these team points based on the attendance/participation in your third and last retrospective on Wed, 11/17 (or whenever your team opts to hold it); 3.34 per team member for teams of 6, 4 per team member for teams of five, 5 points per team member for teams of four.

</div>


# User Flow 
A high-level overview (diagram and associated explanation) of your product's 
[Task/User Flow](https://careerfoundry.com/en/blog/ux-design/what-are-user-flows/) can be used as the starting point for the UX section in your Design Document and also for planning/structuring your user manual.


# Updated Design Document
The exact structure of the Design Document that you started during the last lab is left to your team to determine, but to get you started, we recommend at least the following set of sections in some form and order: 
* Opening/Overview section with high-level system architecture overview diagram for your project, with associated explanations of all parts in some text paragraphs accompanying it.
* More Detailed SW Architecture Design: Describe the main modules in your SW Design in more detail
* Design Process Documentation Section: This is where you can satisfy the point a) from the first grading bullet above: Document your design process by summarizing important team decisions referring to specific meetings logged in your GitHub repo.
* User Interface and User Experience (UX) considerations. Your high-level task/user flow (see above) might be the first thing to document here.

# Start User Manual Document
Start a User Manual Document (as a Google Doc or another `living document` format of your choice) and link to it in a new ./docs/MANUAL.md file in your GitHub. 
It should start with a paragraph explaining the purpose and intended user audience for the product (it can share some of this information with your README.MD, but the manual should be entirely oriented towards end users and should make no mention of implementation details that are not relevant to the end user experience).   


# Third (and last) Retrospective 

You will get time on Wed, 11/17, to hold your third and last team Scrum Retrospective, but you can move the time of this meeting to whatever time within this lab period your team prefers, including right this lab session (Nov. 12). Note though that lab08 (Nov. 19) will be taken up by team pear review of your deployment procedures and apps. 

Make sure you have a Retro leader assigned (should be the case since it was part of the Leadership review last lab).

You already know the goal and procedure for Retrospectives from your RETRO_01 and RETRO_02. This Retrospective allows you to discuss things that are relevant on your final stretch to product deployment, documentation, and presentation.


* In your team's repo, under `team/retrospectives` directory, add a file `RETRO_03.md` capturing the following:

  ```
  # Retro #3 <date>

  * Led by: name-goes-here
  * Present: name1, name2, ... , nameN
  * Absent: name1, name2, ...

  ## Action item

  * a goal: identify something the team wants to get better at
  * a change: identify one thing that the team will change about how it works together
  * a measurement: identify at least one way to measure whether the change helped the team acheive the goal, or move closer to it.

  ## Optional

  * Record anything else you think the team might want to remember from this retro

  ```

* After the Retro
  
  Retro leader: add the following Section to `RETRO_03.md`:
  
  ```
  ## Retro Assessment

  * A brief description of what retro outline or process you used.
  * A brief assessment of how it went.
  * A brief statement on how much any of the Retros changed the way you worked as a team (no correct answer here. 
    Teams could be happy with the way they started operating from the get-go and Retrospectives would just be quick 
    confirmations then, or teams could have tried a lot of different things based on their retro reviews. We just would like to know!)
  ```
 
   

# Carry-over from Lab06: Deployment Manual

Remember that there also was a [second part](https://ucsb-cs148.github.io/f21/lab/lab06-ops/) to lab06, which needs to be completed by next Friday, 11/19, BEFORE your section start 11:00am, or 12:00pm!  
