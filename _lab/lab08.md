---
layout: lab
num: lab08
ready: false
desc: "Group Peer Eval, Two weeks to Code Freeze (but Thanksgiving in between)"
assigned: 2021-11-19 11:00
due: 2021-11-22 12:00
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

**Graded**: ({{page.num}}-T) (30 pts) Team has provided access to its own repo and `-DEPLOY-FEEDBACK` repo to members of the other team in timely fashion.

**Graded**: ({{page.num}}-T) (70 pts) Team members worked together to complete the review of the other team's products, according to instructions, by the deadline for this assignment.

Note: "In a timely fashion" in the items above means "during the lecture or section in which this assignment is made, or within a few hours afterwards"; this is based
on the fact that time will be given during class to complete these tasks.

</div>


# Ops Review

In [lab06](https://ucsb-cs148.github.io/f21/lab/lab06-ops/) you prepared written instructions (and perhaps a video for your team's project) that 
described how to start with only your team's source code repo, and finish with an production ready instance of the application
up and running on supported platform(s).

In this lab:
* The 4-5 people on your team will work together to try out the written instructions (and potentially videos) of the other team you got assigned from your discussion section, and provide feedback to them.
* Each team will also test the current state of the deployed product. NOTE: the performance of your product today has absolutely no grade consequences. It is merely a chance for constructive feedback that you can take into account in your week towards code freeze!  
* In return, you'll be receiving feedback from one of the other teams in your discussion section on your own deployment instructions and product.

The following table lists the review pairings for all teams: 

| Your Team  | will review team | and will be reviewed by team |
|---|---|---|
| t1-  | t3-  | t2-  |
| t2-	  | t1-  | t3-  |
| t3-	 | t2-  |  t1- |
| t5- | t8-  | t7- |
| t7-  | t5-  |  t8- |
| t8-	  | t7-  |  t5- |
| t4-  | t6-  | t11-  |
| t6-  | t9-  | t4-  |
| t9-  | t10-  | t6-  |
| t10-  | t11-  | t9-  |
| t11-  | t4-  | t10-  |

# Step 1: Prepare FEEDBACK Repo and grant access to your reviewers

As a team, you will be preparing a new private Github Repo in which the team that evaluates your work will collect their feedback for you. 
This repo should have the name of your main team repo, followed by `DEPLOY_FEEDBACK`.

For instance:

* t3-11am-course-recommender-DEPLOY-FEEDBACK
* t5-12pm-we-connect-DEPLOY-FEEDBACK
* etc.  

This new repo is private.   You will need to:
* grant write access to your team's `-DEPLOY-FEEDBACK` repo to all members from the other team in your section that is reviewing your repo
* obtain write access to the other team's repos for each person on your team that is participating in a review

Here is a [table with the slack display names of all team members](https://docs.google.com/spreadsheets/d/1BnGP-2nbP-HI3eNsd3Nc8gkpL8mAMNjratRvxIAI-gs/edit?usp=sharing).

To grant access you'll need the github id's of the folks from the other team (which you can obtain
using the `/whois @ScreenName` command on the course Slack.)   

Please communicate with the other team through Slack. Contact persons for each team will be listed [in this table](https://docs.google.com/spreadsheets/d/1rGk06L3xZ08sWqDN3o_FKx8b-mQrxYGO_mrf6XcW0vA/edit?usp=sharing) and you can Slack DM with them to coordinate. 

To grant access, you visit the `Settings` Page of the repo, then `Manage Access` (url is `/settings/access`).

# Step 2: Create Stub for your Feedback

To make these instructions concrete: 
* assuming you are Chris from team `1pm-t1-ride-share`
* you have been assigned to provide deploy feedback for team `1pm-t3-restaurant-reviews`.

1. Go to the `-DEPLOY-FEEDBACK` repo for the team you are supposed to provide feedback for (e.g. `1pm-t3-restaurant-reviews-DEPLOY-FEEDBACK`)
2. Create a file with the name of your own team and name (e.g. `1pm-t1-ride-share-chris.md`) in the root of the repo.  You can just do this directly in the web ui on the master branch.
3. In this file, put the following template (substituting in your name and team name):

   ```
   # Feedback from team 1pm-t1-ride-share.md

   Review by Chris
   
   (Review in progress--leave this line here until review is final)
   
   TODO: Insert review here
   
   ```
   
# Step 3: Actually try deploying the app

Each of you should then try deploying the app from the other team assigned to you.  

If there are naming possibilities for deployments (e.g. Heroku apps), call your app: `cs148-s21-t1-chris-tries-t3, where:
* `t1-chris` is your team's number and your name (which comes before `-tries-`)
* `t3` is the team number of the code your are trying out (which comes after `-tries-`)

You may need to create Auth0 or Google credentials, MongoDB credentials, other API credentials, etc. Ideally, the creation of those will be sufficiently described in your deployment instructions, but for the purpose of successfully completing this peer review, feel free to share throwaway credentials with the reviewing team!   

As you do, follow the instructions provided in the deployment instructions and/or video.

As you run into issues and/or problems, document these, and also work with the other team through Slack to try to resolve them.

As you edit, leave this line as the top of your review until the final step of the lab:

```
   (Review in progress--leave this line here until review is final)
```

# Step 4: Finish your review
 
When you are done, provide a brief writeup in which you provide:

* A link to the running application (or your attempt at bringing up a running application). This can be a heroku deployment or a Google Drive link to an executable or zip file. 
* Suggestions for the team on improving their deploy instructions

Then, turn to some comments about the app itself.  Please address the following questions, plus
anything else you think would be helpful for the team that is working on the app:

- What do you like about the app?
- What, if anything, did you find confusing about the app? 
- What bugs did you find (if any?)
- What suggestions do you have for improvements or new features?
- Would you use this app?  Why or why not?

# Step 5: Notify the other team that your review is finished via Slack.

When your review is finished remove the line:

```
(Review in progress--leave this line here until review is final)
```

And replace it with:

```
Review Complete
```

Then notify the team whose deploy instructions and app you were reviewing, via Slack, that your review is complete.

# One Week to Code Freeze 

For the rest of this lab week, your team will work towards the code freeze deadline, Fri., 12/03/21, 11:59. No lab points are assigned to this portion of the work, but clearly, the work that you will put in will pay off in the final evaluations of your product and documentation! 