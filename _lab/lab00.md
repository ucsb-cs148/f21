---
assigned: 2021-04-02 13:00
desc: Getting Started
due: 2021-04-09 23:59
layout: lab
num: lab00
ready: true
signup_app: https://ucsb-cs-github-linker.herokuapp.com/
slack_url: https://ucsb-cs148-s21.slack.com

---


If you find typos or problems with the lab instructions, please report
them on Slack


## Announcements 

* Webpage updates
* Possibility to switch (as the whole team) to a secondary Lab Section (Fri, 8pm?, Fri, 8am?)
* TA will go over today's lab work (do be done in breakout groups) 
* Making sure teams are all 4-5 students, accommodating students without groups 

# Step 0: Find your Breakout Room and associated mentor: 

Current teams and their initial mentors are listed here:

| Team # | Team Name | Mentor | Breakout Room |
|-----|-----|-----|-----|
|T1|rec-center	|Jayleen	|1	|
|T2|food-bank	|Shiran/Sabrina	|2	|
|T3|course-recommender	|Vincent	|3	|
|T4|community-based-map	|Jayleen|4 |
|T5|we-connect	|Paul |5 |
|T6|ucsb-poll |Paul |6 |
|T7|file-transfer|Shiran/Sabrina |7 | 
|T8|potential-new-group|Vincent |8 | 
{:.table .table-sm .table-striped .table-bordered}


# Step 1: Create a CoE account if you don't have one already

We encourage you to complete all programming assignments by logging in
to the machines in the Computer Science labs, or to connect
remotely. To do this you will need a **College of Engineering
account**. You can create an account online at
<https://accounts.engr.ucsb.edu/create>.

If you are enrolled in <i>any</i> CoE course this quarter (including CS48), you
should be able to create your account immediately.

If you are not able to do so, you will need to contact the ECI Help Desk at <a href="mailto:help@engineering.ucsb.edu">help@engineering.ucsb.edu</a>.

# Step 2: Get setup with github and add yourself to our organization

We will be using github.com in this course. We have created an
organization called {{github_org_name}} on github.com where you can
create repositories (repos) for your assignments in this course.

The advantage of creating private repos under this organization is
that the course staff (your instructors and TAs) will be able to see
your code and provide you with help, without you having to do anything
special.

To join this organization, you need to do three things.

1. If you don't already have a github.com account, create one on the
"free" plan. Visit [https://github.com/](https://github.com/)

2. If you don't already have your @umail.ucsb.edu email address
associated with your github.com account. go to "settings", add that
email, and confirm that email address.

3. Visit our Github Sign Up Tool at <{{page.signup_app}}>.   Navigate to <{{page.signup_app}}>.  Login with your github.com account. Click "Home", find this course ({{site.course}}, {{site.qtr}}), and click the "Join course button".   That will automatically send you an invitation to join the course organization on github.

4. There should be a link to the invitation for the GitHub organization for this course (<https://github.com/{{site.github_org}}>). Click on the invitation link and accept it. You can also go straight to <https://github.com/{{site.github_org}}> and see the invitation there (if you're logged in). Accept the invitation that appears in your browser (from step 3) or log into your account on [https://github.com/](https://github.com/) to accept the invitation.

## Step 2a: Decide where you will work

Your first step here is to decide whether you are going to work:
* on your own laptop/desktop system
* by ssh'ing into CSIL

Here are some of the pros and cons:

| Location | Pros | Cons |
|----------|------|------|
| Your own machine | Less likely to run out of disk space | Must install software |
| CSIL | No need to install software | May run out of disk space, especially for Next.js | 
{:.table .table-sm .table-striped .table-bordered}

Notes for running locally
* Installing software on your own machine is typically straightforward.  We can try to assist during course staff office hours.   Please know. however, that we cannot necessarily provide detailed tech support for every possible operating system version.   You will ultimately be resposible for dealing with any OS specific issues.

Note for running on CSIL
* On CSIL, disk space has typically not been an issue for Spring Boot.  However, next.js does typically take up quite a bit of disk space for dependencies and it is easy to blow past your disk quota.  This article describes some techniques for dealing with disk quota issue on CSIL: [CSIL: Disk Quota and File Quota issues](https://ucsb-cs48.github.io/topics/csil_disk_quota/)
* When running on CSIL, a web server running on `localhost` will not be accessible in your local browser unless you take
  special steps to make it accessible, such as setting up ssh port forwarding.  That process is described here: [CSIL: SSH Port Forwarding](https://ucsb-cs48.github.io/topics/csil_ssh_port_forwarding/)


## Step 2b: Install Git

Skip this step if you are working on CSIL; git comes pre-installed.

If you decide to work locally, you'll need at least git on your local machine. 

* For MacOS, open a terminal prompt and type `git --version` at the prompt.  If `git` is not installed, you'll be prompted to
  install the Command Line Tools part of XCode.   Proceed with the install, and afterwards you should have `git`
* For Windows, we recommend this installation: <https://git-scm.com/download/win>
  * This also provides the "git bash shell", which is a handy tool to have at your disposal.
* For Linux, it is likely that `git` comes pre-installed, but if not, consult the documentation for your distribution.
  * For distributions that use `apt`, it is likely `sudo apt update; sudo apt install git`
  * For distributions that use `yum`, it is likely: `sudo yum install git`

When you can type `git --version` at the command prompt on your system, and it shows a version rather than an error such as `command not found`, you are ready to proceed.

## Step 2c: Configure git

You may skip this step if you've already configured git on the machine where you are working.

## Step 2d: Configure name and email

When you use `git` to add commits to a project, it attaches your name and email to the commit as part of the metadata.

To configure this, type the following commands, substituting in your name in place of `Your Name` and your email in place of `you@example.com`.

```
git config --global user.name "Your Name"
git config --global user.email you@example.com
```

## Step 2e: Configure ssh keys

Configuring ssh keys for GitHub allows us to allows us to avoid having to type in our git password many times per session.  So while not strictly required, it is highly recommended.   All further instructions in the course will assume you have done this step; if you don't, you'll need to adjust the instructions to use `https` based urls instead of the SSH based ones that start with `git@github.com:`.

To configure your SSH keys for GitHub, follow these instructions.  

* <https://ucsb-cs48.github.io/topics/github_ssh_keys/>

Notes: 
* You should generate the keys on the system where you plan to work: generate the keys on CSIL if you plan to work on CSIL, and on your laptop if you plan to work on your laptop.
* If the `ssh-keygen` command is not available on your system, do a web search to try to determine how to install it for your platform.)

## Step 2f: Clone your repo

Now, `cd` in the directory where you plan to do your work for this course (e.g. perhaps `~/cs48`), type this command to clone your empty repo into that directory.   In place of `repo-url-goes-here`, copy the URL for the new repo you created.  That will be, for example: `git@github.com:ucsb-cs48-s20/cgaucho_lab00.git` but with `cgaucho` replaced with your GitHub id.

```
git clone repo-url-goes-here
```

That should create a new empty directory (well, almost empty) called `lab00-cgaucho`.  Use `cd lab00-gaucho` to put yourself i that directory.

If you then type `ls -a` you'll see that the directory is not completely empty. It contains a `.git` subdirectory, which is how you know that this is a git repo rather than an ordinary directory.


# Step 3: Slack channel for your team

Find your mentor.  The team list is here, and it will tell you who your mentor is:

* [teams_page]({{ '/teams_page/' | relative_url }})

Then, ask them to add you to the Slack for the course which is:

* <{{site.slack_url}}>

There should be a channel there for your team.   Find that channel and join it.

# Step 4: Ask your mentor to create a repo for your team

First, your team must decide what language you want to use, so your mentor can choose the correct .gitignore. This choice isn't permanent. Once you've communicated your choice to your mentor, they should create a repo under the organization:

* <{{site.github_org_url}}>

Settings for repo:
* Public or private (your team decides)
* `.gitignore` for whatever language your team decides
* By default, MIT License, unless your team chooses a different one
* The repo name should be the same as the slack channel name.  


Your mentor should then add one team member with admin permission, who will then add all the other team members with admin permission.


# Step 5: Each of you INDIVIDUALLY now makes either a fork or branch of the repo

The next step is done as an individual

You can either:

* Clone the repo and make a branch of the repo that matches your name, e.g.
   ```
   git clone repo-url-goes-here
   cd repo-name-goes-here
   git checkout -b yourname
   ```
OR

* Fork the repo to your own github id

## Step 6a: Inside your fork/branch of the repo, create a file called `team/your_first_name.md`

In your fork or branch, NOT on the master branch of the main repo, please do the following:

Make a directory called `team`. Inside this, create a markdown file named `your_first_name.md` containing a brief description of you and of your ideas for the project. 

* NOTE: Not literally `team/your-first-name.md`, but something like `team/chris.md` or `team/taylor.md`

Each team member should do this individually. Note that this will be publicly displayed on the course site.
   
## Step 6b: Do a pull request from your fork/branch that has your file called `team/your_first_name.md`.

Do a pull request from your fork or branch to the master branch of the repo.  Each team member should have done at least
one pull request from their github id.
   
# Step 7: Create your team/NORMS.md file

This is a list of ideal team behaviors, e.g. everyone arrives to meetings on time or everyone starts things tasks early. You should write this as a team.  Only one student needs to submit a pull request containing this file, however it is ok
if there are multiple pull requests for this file.   You should be careful, however to avoid merge conflicts!

The `team/NORMS.md` file should contain all of the team norms.  It is ok to "suggest" team norms in your individual team/first-name.md files, but the team, ultimately, should consolidate all of these into one `team/NORMS.md` file.

# GRADING

This is a group grade.  Everyone on the team gets the same grade.  HOWEVER, some components of the grade required individual action.   It it suggested that you work together as a team to help and encourage one other to get each part of this done. 

* (60 pts): 
   Points are awarded for each team member that has successfully created their `team/name.md` file, and has done a
   pull request, per the instructions above.   For each team member that does this, points are awarded:
   * For teams with six members, 10 points per team member 
   * For teams with five members, 12 points per team member 
   * For teams with four members, 15 points per team member 
* (30 pts): Completion of the `/team/norms.md` file.
* (10 pts): Ten points for the team when each member of the team has contributed an idea on the Slack channel
   * This "idea" may be an idea about the project, about team norms, or really about anything that is course related.
   * The main point of this item is that we want to make sure that each team member 
      actually knows how to say something on the slack channel.  The content is sort of important, but mainly it's 
      a check on the mechanics.



