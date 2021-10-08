---
assigned: 2020-10-08 11:00
desc: Kanban Boards towards MVP Demo Video
due: 2021-10-15 14:00
due_2_weeks: 2021-10-22 14:00
layout: lab
num: lab02
ready: true
github_org: ucsb-cs148-f21
---

<div style="display:none">
https://ucsb-cs148.github.io/f21/lab/lab02/
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
<br>



lab02 is a team-based grade for several check points towards the MVP demo.

 * Make sure your README.md contains a paragraph about the tech stack you are planning to use, as well as mention user roles (see [this description](https://ucsb-cs148.github.io/s21/lab/lab02-addendum))
 * Kanban board: 
    * There should be a Kanban board (a Github Project associated with your repo) for your team
    * That Kanban board should have a complete set of user stories on it, that, when complete, results in a minium viable product for
   your app; one that clearly delivers value to the user.   User stories should be plain old "cards" on the Kanban board.
    *  There should be a complete set of issues for each of those user stories; a set of issues that are specific TODO's that a individual, pair, or 
   sub-group of your project team can pick up and start coding from.  Each of those issues should have a clear set of criteria for
   what it means to be "done" with that issue.
    * As a team, you've settled on the work you are going to do after the Hello World phase to move towards your minimum viable product (MVP), and you've put user stories and issues in your In-Progress column for each team member.
 * You checked and updated the links in Project Spreadsheet for your team (creating and linking the files LEADERSHIP.md, LEARNING.md according to information from [lect05](https://ucsb-cs148.github.io/s21/lectures/lect05/)) 

<div class="grade" markdown="1">
 
**Graded: ({{page.num}}-I)**: (20 pts) You earn these points if/when you, within one week from the start of this assignment (i.e. by {{page.due |  date: "%a, %b %d at %l:%M%p"}}):

* are assigned to an issue that has been moved from To-Do to In-Progress to Done on the Kanban board, tracking the progress of your issue from start to finish.

Note that each time an issue is moved or assigned, the date/time is tracked; so for full credit, this should be done "in real time" as you work on the issue, not "after the fact".   We'll assess this to encourage you to get in the habit of doing it in real time as you work; doing it that way has benefit to the team.   When you do it in real time, the Kanban board reflects the state of the project, and gives the team a way to visualize the status of what's going on.

But doing it "after the fact" is better than not doing it at all; if nothing else, it helps you learn the mechanics to that you can know better how to do it next time.  So if you forget to do it as you work, go back and do it, going through the motions.  This will earn you partial credit, which is better than getting a zero for this part.

**Graded (lab02-T)**: is your Team grade for {{page.num}}.  As part of this grade:

* (20 pts) Your README.md file is updated with information about your technology stack and approach, as well as listing user roles (see [this description](https://ucsb-cs148.github.io/f21/lab/lab02-addendum))  
* (10 pts) There should be at least one user story in the In-Progress or Done column for your team. If there is more than one in the In-Progress column at any given time, it is because the issues for the first one are insufficient to keep the team making progress, and it was necessary to bring over a second one to have enough issues to work on.
* (10 pts) There should be at least one issue under each user story that supports implementing that user story.
* (20 pts) Each user on the team should have been assigned to at least one issue in the in-progress column.   
   For teams of 5, this part of your grade is 4 points per team member.  For teams of 4, it is 5 points per team member, for teams of 6 it is 3.17 points. 

This component of your team grade is designed to encourage each team member to reach out to all the other members of the team, and be aware of the progress they are making towards the goal of having every team member be making a contribution to the project.  The most important learning goal of the course is to learn to work as a team, supporting one another.

</div>

# About assigning issues to team members

It is possible to assign multiple users to an issue.

You may work on issues either:
* as an individual
* as a pair
* as a "mob" (like pair programming, but with more than one person)

However, if you are working as a pair or a mob, you should *really* be
working as a pair or a mob.  That is, you should plan times to get
together, ideally in person, but at least via screen sharing, and work
together on the code.

What we don't encourage is for Alice and Bob to be assigned to the
issue, and then Alice and Bob take turns "solo programming" on the
issue.  That's a way of working but not the one we are encouraging you
to pursue.

# About limiting work in progress

Throughout the rest of the course, up until we wrap things up with the final project delivery, you are encouraged to:
* ensure that each team member, at all times, is assigned to at least one in-progress issue
* limit the number of in-progress issues.  

Being assigned to more than one in-progress issue is occasionally unavoidable, but typically not ideal.  An example of a case where you may be tempted to do it is when you are blocked on an issue (e.g. waiting for someone else to finish something you need). In that case, you might decide to start another issue so that you are assigned to two in-progress issues at a time.  

But the experience of most teams is that it's best to try not to do this too often.  

Context switching among issues has a cost, and having lots of work in progress can slow a team down further and complicate the delivery of working software that adds value for the user.

# Finally: Choose a leader for next week's retrospective

Choose a leader for next week's sprint retrospective.  That sprint retrospective will take the entire lab period next week.  Attendance at that 
lab is therefore particularly important.  

* Put the name of that leader in a card in the "TODO" column of your Kanban board, e.g. "Chris will lead team in first Retro"

Note, for full course credit, each of you needs to take a turn taking a leadership role in some activity.  
   * If you don't lead a retro, you can be product owner, scrum master, or make a class presentation at some point.
   * So you are encouraged to volunteer.  
   * Once you've led one retro, you'll have fulfilled your duty to exercise leadership at least once. You will likely be able to hold 3, or perhaps 4 retrospectives in total. 
   
<div class="grade" markdown="1">
**Graded ({{page.num}}-T)**: towards the team part of your grade for {{page.num}}.  

This part of the team grade is for the mechanics of:
* (10 pts) naming a retro leader for the [lect06](https://ucsb-cs148.github.io/f21/lectures/lect06/)) retro and record their name in your new LEADERSHIP.md file (described in [lect05](https://ucsb-cs148.github.io/f21/lectures/lect05/)). Also list there the leaders for previous and scheduled Sprint planning meetings, and other major coordination meetings. 
* (10 pts) your LEARNING.md file (described in [lect05](https://ucsb-cs148.github.io/f21/lectures/lect05/)) is filled with information about your tech stack background and learning trajectory.  
</div>  

# MVP Demo, due {{page.due_2_weeks}}

The YouTube video <https://youtu.be/k0Je8ASh4jo>
explains how you can create an MVP demo video using Zoom and YouTube:

<iframe width="560" height="315" src="https://www.youtube.com/embed/k0Je8ASh4jo" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

The [link on Gauchospace]({{page.gauchospace}}) is where you upload the link to your demo when it is complete.   The video may be public, or "unlisted", as you see fit.
Links to videos will be shared with the class, but the class is asked not to share links to non-public videos (unlisted videos)
with people other than enrolled students and course staff.

Your video should be no longer than 5 minutes and should follow the instructions given in <https://ucsb-cs148.github.io/f21/lectures/lect12/>,
which are repeated here:

## Demo of your production app

Your demo should be from your production app (e.g. `prod` on Heroku), not from a version deployed on `localhost`.

Students in the class, as well as Instructors/TAs/LAs should be able to visit your production link and try out the app after watching your video.

So, make every effort to have your production version ready to go with a stable MVP for the deadline lab section.

## Additional notes about the MVP demo

1. **Features beyond MVP are fine**  Note that if you have moved your production version on master "beyond" your MVP, 
   that's fine; as long as it contains all of the MVP functions.   If you are time restricted, you can focus the demo
   just on the MVP features and "save" the rest for later.
   
2. **Broken `master` is a problem.  You can fix with a `temp-prod` branch**.   
   If your `master` branch is currently "broken" in 
   some way that makes it impossible to do a decent demo from your `prod` Heroku app, then here's a quick fix:
   
   - (a) find an earlier commit that isn't broken 
   - (b) give that commit a branch name `temp-prod` for example 
     - use: `git checkout -b temp-prod` 
     - then `git reset --hard a1b2c3d4` where `a1b2c3d4` 
       is the sha of the commit that's good; 
     - then `git push origin temp-prod -f` 
   - (c) redeploy your prod app using `temp-prod` instead of the master branch.
   
   If you do this, please disclose that you are demoing from `temp-prod` and not master in your lab02 submission 
   so that we aren't confused when evaluating your MVP.  
   
   It's not ideal, but it won't be a major deduction.  It's better than demoing a broken `master` branch.
   
3. **A demo from `localhost` is better than nothing, but isn't really an MVP demo**.   If you absolutely 
   *cannot* do a meaningful demo from your production app, then you may demo from `localhost` as a last resort, rather
   than offering no demo at all.   However, that will result in a lower grade; 
   a localhost app isn't really "viable" in the sense that you can't put it in the hands of customers.   
