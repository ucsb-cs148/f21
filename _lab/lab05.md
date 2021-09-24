---
layout: lab
num: lab05
ready: true
desc: "Second Retrospective, Product Improvement, Additional Testing"
assigned: 2021-05-07 13:00
due: 2021-05-14 14:00
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


# Grading for Second Retro

<div class="grade" markdown="1">

**Graded**: ({{page.num}}-I) (20 pts) You earn these points for submitting feedback on overall team performance via a second CATME.org form survey that you got email invitations for.

**Graded**: ({{page.num}}-T) (20 pts) You earn these team points based on the attendance/participation in your retrospective; 4 per team member for teams of five, 5 points per team member for teams of four.

**Graded**: ({{page.num}}-T) (10 pts) You earn these team points when the content in `team/RETROS.md` is updated per the instructions.

</div>


# Today: Second Retrospective

You already know the goal and procedure for Retrospectives from your RETRO_01. This Retrospective allows you to discuss things that 

* We'll put you in breakout groups.
* When you are finished, just leave.
  * No need to come back to main room, unless you have questions
* Staff will be dropping in to observe.

# Deliverable

* In your team's repo, under `team` directory
  `team/RETROS.md`

* Add a section:

  ```
  # Retro #2 05/06/21 or 05/07/21

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

  All Team members: Fill out peer eval survey (on email from CATME.org)
  
  Retro leader: add a file `RETRO_02.md` to `team/retrospectives`
  
  ```
  ## Retro Assessment

  * A brief description of what retro outline or process you used.
  * A brief assessment of how it went.
  * What advice would you give to the next person leading a retro
    based on what you learned today?
  ```

# Grading for new Development / Testing 

Over the next week, please focus predominantly on **new/improved functionality/robustness/user experience** for your product, using your momentum and ideas from the MVP effort and discussion. 

Again, every team member should be assigned (and complete at least one) new issue towards this goal. Make sure that your issues have clear acceptance criteria in Github Projects and that you have a process for completing and assigning issues (e.g. feature branches or your own "Continuous Delivery" rules). It should be possible at any point in time to deploy your product with new improvements over time! 

So, while focus should be on your product growing/improving, we want you to experiment more with Test-Driven-Development (TDD). This could be a great week to fully embrace TDD, and we think you would get many benefits from it in the long term. It is, however, an investment in the short term, so if you don't think that you are ready to completely switch over to TDD, then at the very least you'lll have to select a tool for component testing (a type of integration or end-to-end testing) and implement **at least one** component test **or** other integration **or** end-to-end test in your source code. Use of a Behavior-Driven Development (BDD) framework would also check this box.  

Teams working with React could use the [React Testing Library](https://testing-library.com/docs/react-testing-library/intro/) or [Enzyme](https://enzymejs.github.io/enzyme/) or [Storybook](https://ucsb-cs148.github.io/jstopics/react_storybook/). Python backends could for example be tested with [TestProject](https://testproject.io/) or the BDD frameworks [Behave](https://behave.readthedocs.io/) or [Lettuce](http://lettuce.it/).

<div class="grade" markdown="1">

**Graded**: ({{page.num}}-T) (10 pts) You earn these team points for ensuring that each team member was again assigned at least one issue that was moved to the Done column of your Kanban board with tested acceptance criteria over the next week **ending on 05/14/21, 14:00:00 PDT**.

**Graded**: ({{page.num}}-T) (20 pts) You earn these team points if your team integrated a higher-level (not just unit tests) testing framework with your project

**Graded**: ({{page.num}}-T) (20 pts) You earn these team points if your team implemented and demonstrated successful execution of **at least one** component test **or** other integration **or** end-to-end test (e.g. BDD) in your project. 


</div>
 