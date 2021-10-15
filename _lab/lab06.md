---
layout: lab
num: lab06-part1
ready: false
desc: "Retro2 Outcome Logging / Review and Plan Leadership Roles / Start Design Document "
assigned: 2021-11-12 11:00
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
**Graded**: ({{page.num}}-T) (15 pts) You earn these team points if you have logged the result of your Retro 2 Experiment

**Graded**: ({{page.num}}-T) (15 pts) You earn these team points if you have planned future team leadership roles and logged them in your GitHub ./team/LEADERSHIP.md as per instructions below 

**Graded**: ({{page.num}}-T) (40 pts) You earn these team points if you started a design document that you link to in your Github ./docs/DESIGN.md and that contains at the very least an overview system architecture diagram and associated explanation.  
</div>


# Retro 2 Outcome Logging
* For the experiment you decided upon in your second retrospective, use the metric that you had planned on using to decide if the change brought positive results or not. Log the outcome in the following way 
  
  **Retro 2 leader**: add Section to `team/retrospectives/RETRO_02.md`
  
  ```
  ## Retro Outcome Assessment

  * A brief description of what your retro 2 experiment was 
  * A brief recap of the metric you planned on using 
  * The outcome according to the metric now that the next Sprint is done (maybe already for a while).
  * Your conclusions based on this outcome. You can decide to cement this change going forward, to modify it (start a new experiment), or to discard it and go back to previous procedures.    
  ```

# Review and Plan Leadership Roles
 Visiting your ./team/LEADERSHIP.md file, remind yourselves who took on previous leadership roles for your team, and log anything that may have fallen by the wayside.  

For example (if applicable): 
    * Initial Product Owner 
    * First Retro Leader 
    * Second Retro Leader 
    * MVP Peer Eval Leader                

Then, discuss the list of roles below and assign one team member to each of the roles.

Several people will clearly be assigned to more than one role. That's fine, but follow these rules:

    * The product owner and the scrum master *may not* be the same person at any time, and
    * The retro leaders for each of the three retros in the quarter should be different people.
    * No one should take on three roles unless/until each team member has already taken on two.

&nbsp;
If you have a situation where it is impossible to satisfy all of these rules, check with your mentor;
they are permitted to authorize exceptions where there is a legitimate need to do so.

Also, whoever is chosen below as the "Design Document Coordinator" will be responsible for copying these roles from your discussion into ./team/LEADERSHIP.md.

**Roles to assign**

* **Product Owner**.  Together with Scrum Master, leads the Sprint Planning meeting(s) to come
      Responsible for making sure that the team comes up with a set of **user stories**
      for the "final" product that your team will deliver, and marking those stories with a label "final" (just
      like the label `MVP` that you used previously).  
* **Scrum Master**.   Together with Product Owner, leads the sprint planing meeting(s) still to come.
      Responsible for making sure that the team comes up with a set of **issues**
      for the "final" product that your team will deliver, each tied to one of the user stories.
      and marking those stories with a label "final" (just like the label `MVP` that you used previously).
      Also responsible for holding the team accountable for keeping the issues moving through the Kanban board.
* **Testing/QA Coordinator**. 
      Ultimately, responsible for making sure that user stories and issues have acceptance criteria, and that
      these are met before pull requests are accepted into master. If you are doing any sort of TDD or BDD, this person will also mainly coordinate that effort. 
* **Retro 3 leader**.  This person will lead the third retro during week 9.
* **UX Coordinator**.  Responsible for the look and feel of the product, and the way that the user interacts with the
      product. By next week, will have a set of pointers and recommendations for the UI/UX of your products...
* **Design Document Coordinator**.  This person is responsible for the design process documentation started in this lab, chiefly the document pointed to by ./docs/DESIGN.md.
      By next week (lab07), they should ensure that there is a first version, and will be responsible for updating it throughout the rest of the quarter.
* **Deployment Document Coordinator**.  This person is responsible for the deployment documentation refactored in this lab, chiefly the document pointed to by ./docs/DEPLOY.md.
      By next week (lab07), they should ensure that there is a first version, and will be responsible for updating it throughout the rest of the quarter.
* **User Manual Coordinator**.  This person is responsible for the user manual part of the documentation. More detail will be given in lab07, and the person in charge will be responsible for updating it
      throughout the rest of the quarter.
* **Final presentation leader (week 9/10)**.  This person will be in charge coordinating the final class presentation video during week 9/10. The presentation itself will likely have multiple presenters, but the leader ensures everyone is prepared and everything goes smoothly with demos and setup.
  


# Start Design Document
Start a Design Document (as a Google Doc or another `living document` format of your choice) and link to it in a new ./docs/DESIGN.md file in your GitHub. 
It should contain, for starters, a high-level system architecture overview diagram for your project, with associated explanations of all parts in some text paragraphs accompanying it.   

For examples that might stir your creativity, you can check out, e.g., the Requirement Documents in [UCSB Capstone projects](https://capstone.cs.ucsb.edu/past20.html)   

You can use any diagramming tool of your choice. Please post in Slack if you like a tool beyond the ones in the list below, but here are some options:   
   * Google Slides
   * LibreOffice (Impress, Draw)
   * Microsoft Powerpoint or Visio (if you have access to MS Office) 

Or some web-based solutions: 
   * [diagrams.net](https://www.diagrams.net)
   * [Gliffy](https://www.gliffy.com/)
   * [graphviz](https://graphviz.org)

Multi-Platform: 
   * [drawio - see also diagrams.net above](https://github.com/jgraph/drawio-desktop/releases/tag/v14.6.13)
   
Or on Mac/IOS:     
   * [Flowchart Designer 3](https://apps.apple.com/app/flowchart-designer-3/id1512570906) 
   

# Part II: Deployment Manual

There is a [second part](https://ucsb-cs148.github.io/s21/lab/lab06-ops/) to this lab, which has a two-week performance period. 
