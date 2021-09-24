---
desc: Mentor instructions for lab00
github_org: ucsb-cs148-s21
layout: lab
mentor_due: 2021-04-02 23:59
num: lab00_mentors
ready: false
ta_due: 2021-04-15 23:59

---

<div style="display:none">
https://ucsb-cs148.github.io/s21/lab/lab00_mentors/
</div>

# These instructions are for mentors/TAs only

Students, you are welcome to read them; there are no secrets here.   But there are probably better uses of your time. :-)


# Creating Feedback repos (overview)

The task is to create feedback repos for the individual students.  These are the places where we'll record information
about their grades for various items in the course.

(Note that it would be *so much nicer* if we had an app to do this. Phill Conrad is on it, but for now we'll just continue to do it by hand, and it'll get done fast since we are spreading the work over 8 mentors.)

# Create a team level FEEDBACK repo for each of your teams

First thing: go to <https://github.com/ucsb-cs148-s21> and create a new **private* repo with your team's name followed by the suffix `_FEEDBACK`

| For team | create repo |
|----------|-------------|
| `4pm-stock-trading` | `4pm-stock-trading_FEEDBACK` |
| `5pm-pet-life` | `5pm-pet-life_FEEDBACK` |

etc...

Create it as follows:
* private
* with a `README.md`
* no `.gitignore` and no `LICENSE`  needed

Then, add each of the team members to that repo as collaborators, by their github id, with READ ONLY permission.


# Create individual team member FEEDBACK repos

Now, for each team member, on each of your teams:

Create a new **private* repo with the prefix of the team name, then `_FEEDBACK` then `_` then the individual's github id.

For example, 

| For team | with member with github id | create repo |
|----------|----------------------------|--------------|
| `5pm-pet-life` | `cgaucho78`  | `5pm-pet-life_FEEDBACK_cgaucho78` |
| `5pm-pet-life` | `bondjamesbond`  | `5pm-pet-life_FEEDBACK_bondjamesbond` |
| `5pm-pet-life` | `haskellkween`  | `5pm-pet-life_FEEDBACK_haskellkween` |

etc...

Create it as follows:
* private
* with a `README.md`
* no `.gitignore` and no `LICENSE`  needed

Then, for each of these, only that individual student  as collaborators, by their github id, with READ ONLY permission.

Next, we'll put some information in the team repos as feedback on lab00 so that the TAs can start grading it.


# Mentor Review of lab00

Due {{page.mentor_due}}

The evaluation of lab00 is entirely at the team level, and will be completed in a file called `lab00.md` in the team `_FEEDBACK` repos.  

The repo <https://github.com/{{page.github_org}}/FEEDBACK_TEMPLATES> contains templates for feedback for various assignemnts that we'll
give throughout the quarter.  In that repo, locate the file:

* <https://github.com/{{page.github_org}}/FEEDBACK_TEMPLATES/blob/master/lab00.md>

You can copy the contents of that file into each of your feedback repos, and then fill in the template provided.

# TA Review/Grading of lab00

Due {{page.ta_due}}
