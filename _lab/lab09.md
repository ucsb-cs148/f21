---
layout: lab
num: lab09
ready: true
desc: "Final Code Release"
assigned: 2021-06-04 13:00
due: 2021-06-10 23:59
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

<div class="grade" markdown="1">

**Graded**: ({{page.num}}-T) (50 pts) Final Code Release and Deployment (Heroku or pointer to platform binaries) by **Fri, 06/04, 23:59:59**.

**Graded**: ({{page.num}}-I) (30 pts) Team (coordinating on one response or by submitting individual commentary) documents team roles and github contributions.

**Graded**: ({{page.num}}-I) (10 pts) Every student lists at least one insight in `#lessons_learned` Slack channel. 

**Graded**: ({{page.num}}-I) (10 pts) Every student submits their favorite 3 projects in the audience choice awards voting (to be released on **Wednesday, 06/09**). 

</div>


# Final Code Release and Deployment

Look back on [Lab04 MVP Tag/Release instructions](https://ucsb-cs148.github.io/s21/lab/lab04/) to remind yourselves on how to do a tag and release and do a "Project Demo" Tag and numbered Release for your Code Freeze by **Fri, 06/04, 23:59:59**.

By the same deadline, add a `#Deployment` section at the bottom of your README.md, which points to a live testable version of your project, either on Heroku (or other cloud service), or to platform binaries (e.g. hosted on Google Drive). 

The deadline for your Manual and for the Design Document, s well as for your 10-minute final Demonstration Video is  the coming **Tuesday, 06/08, 23:59:59**.

# Team Roles and Github Contributions

We ask every team to comment on the code contributions that every team member made. You already documented leadership roles within the team management (in team/LEADERSHIP.md), and now we ask you to document the roles the team members played in the code development effort. In your github team folder, please create a `contributions` subfolder. 

By **Tue, 06/08 23:59:59**: write brief commentary on team member code contributions: 
*each team member* should initially write their own section.    
  - Suggestion: each team member should initially create a draft of their part in `contrib_Alice.md`, `contrib_Bob.md`, `contrib_Carol.md`, `contrib_Danny.md`
  - Then: the person writing the overall report can copy/paste those separate files into one unified CONTRIBS.md file.
* Today: Review the `/graphs/contributors` report for your project repo.    
  - You can find it by clicking "insights" then "contributors".
  
## Is the `Contributors` graph accurate?

Note that there can be big disparities between the contributors graph and ground truth.

One source is "misattributed commits".  As an example, see this page:

* <https://github.com/ucsb-cs48-s20/project-idea-reviewer/commits/master?after=e37a193735918fa2f25c9af93ad1e129caec2946+69>

Note that:
* *some* of the commits that Phill Conrad did on this page are attributed to his GitHub account, `pconrad`, and have his avatar (the icon/photo) next to his commit.
* but *other* commits are *not* attributed to that account, and just say "Phillip Conrad", and have a generic grey icon.

The difference has to do with whether the machine on which the commits were performed was configured to connect to a GitHub account or not. This is a lesson learned for the future!  

It's too late to fix the commits, but it's NOT too late to offer an explanation in part 3 of your report.
* We are going to look at the data on the `/graphs/contributors` for your repo, but
* We are going to look *more* at your explanation of that data.

If the data and the explanation match, it's all good.

If you have a team member that you suspect has made lots of commits that are not being attributed to them, 
scroll through your commit log and see if you can find a few examples.

If the commits look ok, but don't tell the full story (e.g. a team member may have just contributed very few, but very important commits), you can bring that out in your commentary, too. 

Even distribution of the coding effort among all team members is definitely not expected, but highly uneven contributions, especially when paired with potential team dissatisfaction expressed through the catme.org surveys may be grounds for individual weighting of the project grade component among team members.   


# Lessons Learned 

Every student will post at least one "I wish I had known it when I started" lesson learned in our #lessons_learned Slack channel. 
Examples: 
* During a rebase, *just rebase*.  Don't make changes (i.e. fix bugs, add features) during a rebase.  Only focus on 
  fixing merge conflicts.    Make your changes to fix bugs or add features before the rebase, or after the rebase,
  but *not during*.
* Making sure to listen to your team mates and give everyone a chance to feel like they are a part of the team, because the internal team work and how everyone contributes is crucial to the   
  team's effectiveness and success. 
* The `git bisect` tool [can help you figure out](https://git-scm.com/docs/git-bisect) with what commit you introduced a crucial change in your repository. 


# Participation in Audience Choice Award

On **Wednesday, 06/09**, you will be invited to a Google Form that points to all the final videos of your projects. You can follow all project demonstrations and interactive Q&A during our final slot project presentation session on **Thu, 06/10, 4pm-7pm** and submit the Google Form after that, or, if you really can't make it to other presentations but your own (in that one your presence is required!), then you can peruse the links to get an idea of the other projects before you vote. In any case, in order to receive the last individual 10 lab points, your vote needs to be submitted by **Thu, 06/10, 23:59:59**.  