---
desc: "Production pipeline. Feature-branch/pull request workflow"
lecture_date: 2021-10-18
num: lect06
ready: true
---
 
# Announcements
* h05 is (uncharacteristically!) due on Friday. We set the deadline to be 2pm, but will accept submissions until 11:59pm. h06 will be posted on Friday, and will be due the next Friday. 
* catme.org peer reviews are due Wed. Night. You get a lot of lab03 points for it, so please don't miss it! **Let us know if you didn't get an email (to your umail account!) last Fri/Sat**


# Sprint Planning
* [Sprint Planning](https://www.agilealliance.org/glossary/sprint-planning), can be combined with [Story Time](https://switchingtoscrum.wordpress.com/2012/11/28/what-are-story-time-meetings-for/)...

# Continuous Integration / Continuous Delivery (CI/CD) 

* **Continuous Delivery**: Software development process that aims to build software that is *always* ready to be deployed into production
* **Continuous Integration**: Technique where every developer on a project should integrate their work daily with every other developer

# Feature Branch / Pull Request Workflow

When making a change to your team's repo, you should typically NOT be making changes on the `master` branch

* At many companies, the `master` branch is a "protected" branch.
* There is "process and ceremony" around when/where changes to `master` are pushed.
  * Certain things may have to be done first (code reviews, testing, etc.)
  * Sometimes only certain members of the team do it
 
Reasonable exceptions: small changes to documentation only (not touching code).

## So what do you do instead?

* Make a feature branch
* Work on the feature branch
* When done, make a Pull Request

## Whoa, whoa getting ahead of ourselves: issue first.

WAIT.

Before you start working on a branch:
* There should be an issue on the Kanban board.  If there isn't, make one.
* Be sure the issue has clear acceptance criteria, formatted as a checklist:

  ```
  - [ ] There is a menu item called `Users`
  - [ ] The menu item `Users` only appears when logged in as an Admin
  - [ ] The menu item `Users` leads to an page that lists users
  - [ ] The column headings for the users list is First, Last, and Email
  etc.
  ```
  
* Assign yourself to the issue and drag the issue into the "In Progress" column.
* Assign any pair partners working with you to the issue also.

Once your team is in steady state, you should always be assigned to at least one in-progress issue
on the Kanban board.

## Ok, got an issue.  How do you make a feature branch?

Like this.  Always start with a fresh copy of master:

```
git checkout master
git pull origin master
git checkout -b thAddMenuItem
```

The `th` are your initials (the person making the branch).   The rest is camel-cased and summarizes the purpose of the branch.

You could also come up with a different branch name convention, one that works better for your team.

The important thing is to have one.
* You should use the branch naming convention described above *unless* your entire team comes to a team consensus
  on a different convention, and a rationale for why that process is better.
* If you decide on a different convention, document it in a file `team/CONVENTIONS.md`

## Working on a feature branch

You may need, periodically, to push your changes to GitHub.  Use the branch name in place of `master`:

* `git push origin thAddMenuItem` 


## Rebasing on master

You may need, from time to time, to rebase your branch on master.

This is to say, replay all of the changes on your branch on top of a *fresh* copy of master.

To do this, type:

```
git pull --rebase origin master
```

You may have merge conflicts.  If so, you may find that you have to resolve these merge conflicts *one commit at a time*.

If all else fails, you can always type `git rebase --abort` to abort the mission and start over.

But if you stay focused, you can get through it:

* Step through the commits carefully, and read the instructions on the screen carefully.  
* At each step, use `git status` to see where you are and what the next step is.
* Files marked in red as `both changed` are the ones that you need to look for merge conflicts in
* You resolve those by editing the file, and then doing a `git add` so that it turns green in the `git status` output.
* You may have to do multiple commits and then `git rebase --continue`
* At some steps, you may also find you need to do `git rebase --skip` to get to the next commit.


Eventually, you'll have a new version of your branch, at which point you'll want to:

* test to make sure that everything still works.
* then "force push" to update GitHub with the new branch history for your branch (your changes "rebased" on the newest version of `master`).

```
git push --force origin thAddMenuItem
```
## Creating a Pull Request

When you create a pull request, which you can easily do through the github web interface, you have to select a *base* branch and a *compare* branch.

* The "base" branch is typically `master`; it's where the "old code" lives
* The "compare" branch is typically your feature branch; it's where the "new code" lives.

You are requesting that the admins of the repo pull commits from the compare branch into the base branch.

Once you create a Pull Request, you should:

* Link the issue you were working on to the Pull Request
* Ask for members of your team to review the Pull Request (through the GitHub Web UI)
* Consider posting a link to the PR on your team's Slack channel (there are ways to automate this, but let's not get ahead of ourselves.)
* Drag the issue you are working on from the "In Progress" column into the "In Review" column.

## Reviewing a PR

If you are asked to review a PR, please do so promptly.

Diplomacy is good... it's better to ask questions than make statements.

```
I wonder if this code would be clearer if we factored out both the long if
part and the long else part into separate functions?   Choosing
some good names for those and some good parameter values might make this
code easier to understand.  What do you think?
```

vs.

```
This code is a convoluted mess---so complicated that no-one could
possibly make sense of it.  You need to totally rewrite this!
```

Both of these might be honest and understandable reactions to 
the same code.  But one is much more likely to result in good
team relations and team productivity. :-)

# Today:

* Standup
* If not done yet: Sprint planning for MVP! 
* Practice branches and pull requests (PR)
* Work towards MVP code freeze a week from today. See also [lab03](https://ucsb-cs148.github.io/f21/lab/lab03/)
