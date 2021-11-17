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

**Graded**: ({{page.num}}-T) (30 pts) Team has provided access to its own repo and Feedback Google Doc to members of the other team in timely fashion.

**Graded**: ({{page.num}}-T) (70 pts) Team members worked together to complete the review of the other team's products, according to instructions, by noon on Monday, 11/22.

Note: "In a timely fashion" in the items above means "during the Section in which this assignment is made, allowing the revieewing team to put Section time fully towards the evaluation"; this is based
on the fact that time will be given during Section to complete these tasks.

</div>


# Ops Review

In [lab06](https://ucsb-cs148.github.io/f21/lab/lab06-ops/) you prepared written instructions (and perhaps a video for your team's project) that 
described how to start with only your team's source code repo, and finish with an production ready instance of the application
up and running on supported platform(s).

In this lab:
* The 4-6 people on your team will work together to each try out the written instructions (and potentially videos) of the other team you got assigned from your discussion section, and provide feedback to them.
* Each team will also test the current state of the deployed product. NOTE: the performance of your product today has absolutely no grade consequences. It is merely a chance for constructive feedback that you can take into account in your week towards code freeze!  
* In return, you'll be receiving feedback from one of the other teams in your discussion section on your own deployment instructions and product.

The following table lists the review pairings for all teams: 

| Your Team  | will review team | and will be reviewed by team |
|---|---|---|
| t01-11am-sbrideshare  | t03-11am-fitnessguru  | t02-11am-clubrush  |
| t02-11am-clubrush	  | t01-11am-sbrideshare  | t03-11am-fitnessguru  |
| t03-11am-fitnessguru	 | t02-11am-clubrush  |  t01-11am-sbrideshare |
| t05-11am-recipefinder | t08-11am-servedup  | t07-11am-musictaste |
| t07-11am-musictaste  | t05-11am-recipefinder  |  t08-11am-servedup |
| t08-11am-servedup	  | t07-11am-musictaste  |  t05-11am-recipefinder |
| t04-12pm-youtubevoice  | t06-12pm-campusmaps  | t11-12pm-typingtest  |
| t06-12pm-campusmaps  | t09-12pm-studygroup  | t04-12pm-youtubevoice  |
| t09-12pm-studygroup  | t10-12pm-animelist  | t06-12pm-campusmaps  |
| t10-12pm-animelist  | t11-12pm-typingtest  | t09-12pm-studygroup  |
| t11-12pm-typingtest  | t04-12pm-youtubevoice  | t10-12pm-animelist  |

# Step 1: Set up FEEDBACK Document and grant access to your reviewers

As a team, you will create a Google Doc to capture the feedback from the team that is reviewing your product. 
The document should start as follows: 

```
   **Deployment and Product Feedback for Team <your team name>**

   (Review in progress--leave this line here until review is final)
```

Please list the link to that document in your team folder as team/DEPLOY_FEEDBACK.md and, as the first action item of today's lab section, communicate that link to the reviewing team. 

Please communicate with the other team through Slack. Contact persons for each team will be listed [in this table](https://docs.google.com/spreadsheets/d/1rGk06L3xZ08sWqDN3o_FKx8b-mQrxYGO_mrf6XcW0vA/edit?usp=sharing) and you can Slack DM with them to coordinate. 


# Step 2: Create Stub for your Feedback

To make these instructions concrete. Assuming: 
* you are Chris from team `1pm-t1-ride-share`
* you have been assigned to provide deploy feedback for team `1pm-t3-restaurant-reviews`.

1. Go to the Google Doc for the team you are supposed to provide feedback for (`1pm-t3-restaurant-reviews`), the link should have been communicated to you via Slack. If NOT, please prod the team for it! 
2. In this file, put the following template (substituting in your name and team name):

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

# Two Weeks to Code Freeze 

Over the next two weeks, your team will work towards the code freeze deadline, Fri., 12/03/21, 11:59. 
The work that you will put in will pay off in the final evaluations of your product and documentation! 

There will be one more Lab (lab09), but it will officially start after the Thanksgiving holiday, on Monday, 11/29. It will be discussed in class next week, however. 