---
assigned: 2021-10-01 11:00
desc: Getting Started
due: 2021-10-08 23:59
layout: lab
num: lab01
ready: false
signup_app: https://ucsb-cs-github-linker.herokuapp.com/
slack_url: https://ucsb-cs148-f21.slack.com
github_org_name: ucsb-cs148-f21

---

## Announcements 

* COVID-19
* Making sure teams are all 4-6 students, accommodating students without groups
* Possibility to switch (as the whole team) from 11am to 12pm Lab Section
* TA will go over today's lab work (do be done in team groups) 


## Step 0: Find your assigned seat and meet your mentors

Seating charts are here:

| Row | 11am | 12pm |
|-----|-----|-----|
|1 | **t01-sbrideshare** (Vincent, Alan)     &     **t02-clubrush** (Nagarjun, Zechen) | **t06-campusmaps** (Bryan, Zechen) |
|2 | **t07-musictaste** (Alan, Vincent)	     &     **t08-servedup** (Vincent, Alan) | **t09-studygroup** (Nagarjun, Zechen) |
|3 | **t03-fitnessguru** (Zechen, Alan) | **t10-animelist** (Bryan, Tobias) |
|RT Window | **t04-youtubevoice** (Bryan, Nagarjun) | **t11-typingtest** (Tobias, Vincent)	|
|RT Door | **t05-recipefinder** (Alan, Vincent)	|  | 
{:.table .table-sm .table-striped .table-bordered}


# Step 1: Create a CoE account if you don't have one already

You could do all the necessary work this quarter on your own computer, but very likely it will be convenient for you to test things with your team on a computer in one of the Computer Science Labs. 

To log on to the machines in the Computer Science labs, or to connect
remotely, you will need a **College of Engineering account**. You can create an account online at
<https://accounts.engr.ucsb.edu/create>.

If you are enrolled in <i>any</i> CoE course this quarter (including CS148), you
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

**Milestone 1**: Once all your team members have successfully joined the organization, send a message in your Slack team channel that states "Milestone 1 completed!". This is important, because we will run a program to automatically create GitHub repositories for your teams once all the teams in this Section have completed this milestone. 

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
  special steps to make it accessible, such as setting up ssh port forwarding.  That process is described here: [CSIL: SSH Port Forwarding](https://ucsb-cs148.github.io/topics/csil_ssh_port_forwarding/)


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

* <https://ucsb-cs148.github.io/topics/github_ssh_keys/>

Notes: 
* You should generate the keys on the system where you plan to work: generate the keys on CSIL if you plan to work on CSIL, and on your laptop if you plan to work on your laptop.
* If the `ssh-keygen` command is not available on your system, do a web search to try to determine how to install it for your platform.)

## Step 2f: Clone your repo

Now, `cd` in the directory where you plan to do your work for this course (e.g. perhaps `~/cs148`), type this command to clone your empty repo into that directory.   In place of `repo-url-goes-here`, copy the URL for the new repo you created.  That will be, for example: `git@github.com:ucsb-cs148-f21/cgaucho_lab00.git` but with `cgaucho` replaced with your GitHub id.

```
git clone repo-url-goes-here
```

That should create a new empty directory (well, almost empty) called `lab00-cgaucho`.  Use `cd lab00-gaucho` to put yourself in that directory.

If you then type `ls -a` you'll see that the directory is not completely empty. It contains a `.git` subdirectory, which is how you know that this is a git repo rather than an ordinary directory.