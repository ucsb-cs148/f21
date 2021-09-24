---
layout: lab
num: lab04
ready: true
desc: "MVP Release, MVP Review, Testing"
assigned: 2021-04-30 13:00
due: 2021-05-07 14:00
github_org: "ucsb-cs148-s21"
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


# Finalize MVP Materials ([lab03](https://ucsb-cs148.github.io/s21/lectures/lect06/) requirements) 

<div markdown="1">

**Graded**: (lab03-I) (5) You earn these individual points if you participated in the first retrospective.

**Graded**: (lab03-I) (20) You earn these points for submitting feedback on overall team performance via a CATME.org form survey that you got email invitations and possibly reminders for.

**Graded**: (lab03-T) (20) You earn these team points based on the attendance/participation in your retrospective; 4 per team member for teams of 5,  5 points per team member for teams of four.

**Graded**: (lab03-T) (20) You earn these team points when the content in `team/retrospectives/RETRO_01.md` is updated per the instructions from [lect06](https://ucsb-cs148.github.io/s21/lectures/lect06/).

New since [lect06](https://ucsb-cs148.github.io/s21/lectures/lect06/): 

**Graded**: (lab03-T) (10) You earn these team points when you recorded the outcome of (one of) your Retro experiments in `team/retrospectives/RETRO_01.md` by the due date of the MVP. 

**Graded**: (lab03-T) (10) When MVP Sprint Planning meeting took place and was documented in your team/sprint0?/ folder (question mark for number of current sprint).

**Graded**: (lab03-I) (5) You earn these individual points if you gave a 'thumbs up' in Slack to at least one article you appreciated in one of the `..._articles` channels.

**Graded**: (lab03-T) (10) You earn these team points if your README.md is updated with complete installation instructions for your MVP and your MVP video link is announced in `team/MVP_DEMO.md`.  

</div>

## Finalizing your demo (MVP video)

* Plan a five minute presentation video
* Please prepare a 5 minute YouTube video (unlisted or public, your choice)
  - See the bottom of the [lab02](https://ucsb-cs148.github.io/s21/lab/lab02/) description for information about creating your MVP video.
  - Links to videos will be made available to (some of) the class for peer review, but will not be made public
* Present to an audience of **potential users**
  - Not to an audience of CS148 students, or the instructor or TAs.
  - Explain what problem the app solves, or what need it fulfills, as you demo the features of
    the app.
* Stay focused on user functionality.
  - Do not go into details of implementation, or team process.
  - There will be other presentations for that.
* Optionally, you may introduce with a powerpoint slide, and/or close with one, but the bulk
  of the time, you should be sharing your screen and showing us your app.
* At the end, tell us a bit about upcoming features planned for the next iteration.

At next week's Tuesday lecture [lect10](https://ucsb-cs148.github.io/s21/lectures/lect10/) you'll be asked to evaluate other teams' presentation(s), so plan to watch them and be ready to do some very brief writing after each one.

## Point us to your video 
*  **by 04/30/21, 23:59 PDT** create a file `team/MVP_DEMO.md` containing your MVP video link and any additional information you see fit that you think doesn't belong in the project's README.md  

## Add Installation instructions to your README.md 
*  **by 04/30/21, 23:59 PDT** (for details, see [lab03](https://ucsb-cs148.github.io/s21/lab/lab03/)) 

# Lab04 New Deliverables

<div class="grade" markdown="1">

**Graded**: ({{page.num}}-T) (10 pts) You earn these team points if your team has a github tagged release of your MVP timestamped **before 04/30/21, 23:59:59 PDT**

**Graded**: ({{page.num}}-I) (25 pts) You earn these individual points if you participate in the MVP review during [lec10](https://ucsb-cs148.github.io/s21/lectures/lect10/)  and submit an evaluation form to briefly review all other groups' MVPs by **Tue, 05/04/2021, 17:00 PDT**

**Graded**: ({{page.num}}-I) (25 pts) You earn these team points in the MVP review during [lec10](https://ucsb-cs148.github.io/s21/lectures/lect10/) on **Tue, 05/04/2021** if at least one member of your team asks a question after the video of one other team (the pairing will be announced before the class lecture) 

**Graded**: ({{page.num}}-T) (20 pts) You earn these team points for implementing and documenting at least one unit test in your code base by next week **05/07/21, 14:00 PDT**.

**Graded**: ({{page.num}}-T) (20 pts) You earn these team points for ensuring that each team member was assigned at least one issue that was moved to the Done column of your Kanban board with tested acceptance criteria over the next week **ending on 05/07/21, 14:00:00 PDT**.

</div>

## MVP Tag/Release in your GitHub repo
By the end of Friday, 04/30/21, tag and release your MVP project in your github. 
[This brief article](https://medium.com/@jameshamann/a-brief-guide-to-semantic-versioning-c6055d87c90e) gives some suggestions on versioning numbering.  

### To create a tag:
#### Option 1: Web UI
* You can use the web UI to create a tag, but it will only create the tag from the current version (most recent commit).
The tag is automatically created when you create a new release in the git UI.
* Skip directly to 'Create a Release'

#### Option 2: command line instructions. 
(Choose this option if you need to create a tag that is earlier than the most recent commit)

`git tag v1.0.0 <commit ID>`

note - v1.0.0 is the tag name, and commitID refers to the last commit in your MVP 

you can find the commit ID using `git log`, or using the history tab in the github web ui

if done correctly, you should see something like this in the git log
![image](https://user-images.githubusercontent.com/10558897/116512519-06006680-a87d-11eb-9ead-d6cbc0d633bd.png)

if you messed up, you can delete the tag using `git tag -d <tag_name>`

Verify that everything looks good, then `git push origin <tag_name>`

Your newly created tag should appear in your tags page on the web UI

### To create a release:

#### Option 1:
* If you want to create a release from the current, most recent commit
* On the right hand column, there should be a section labeled 'Releases'. Click on 'create a new release'
* Put v1.0.0 in the 'Tag Version' box, and fill out the rest of the boxes.
* Click `Publish Release' and the tag will automatically be created for you

#### Option 2:
* If you want to create a release from an existing tag
* On the right hand column, there should be a section labeled 'Releases'. Click on 'create a new release'
* There should be a toggle between Releases and Tabs right above the 'Tag Version' form. Click on Tabs to toggle over.
* Click on the  menu (with 3 dots) on the far right hand side of the tag, and select 'Create Release'
* Fill out the form, and `Publish Release`

## New Deliverable: Participate in the MVP review and review other groups' MVPs

In class **on Tue, 05/04/21, 15:30**, we will watch the videos all the groups have created, and provide feedback in a simple Google Form. You will get points towards lab04 for submitting these forms. 

## New Deliverable: Testing  

Over the next week, the following testing deliverables will give you points towards lab04: 

  * Make sure that every person on your team is assigned to at least one issue in the in-progress column of your Kanban board at all times. If you complete work on the lasst open issue you were assigned to (yay!) and you move it to the Done column, immediately assign this team member a new issue from the Sprint backlog and move it to the in-progress column. Make sure that all these issues have clear acceptance tests/criteria and that you verified these before calling the issue Done.   
  
  * Use a unit testing library / test runner of your choice (we recommend JEST for Javascript/React and PyUnit for Python (comes with the Python package)) to implement **at least one** unit test in your code. Mind you, *one* unit test will not really do you any good, apart from making you go through the motions. The benefit of unit testing, and test-driven software development in general comes from consistent use and embrace of it as a software engineering methodology, but for now we won't require fully instrumenting your code with tests, even though we encourage it as a matter of principle!   


 