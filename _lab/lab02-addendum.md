---
desc: Expand README.md 
layout: lab
num: lab02-addendum
ready: true
github_org: ucsb-cs148-f21
---


# A few things to add to your README.md:

1. In your README.md, add a line for which app type / tech stack you are using.
2. Add some more detail about the plan for your app to your README.md
   * Minimum, a single paragraph that expands on the one-sentence description
   * Better: Instead of, or in addition to that, a list of user roles (see below), and few things that
     people in each user role can accomplish in your app
   * Even Better: go beyond that, and talk about roles and permissions
     
   
## Add "Tech Stack" to your README.md

We've provided some information for you already, and lab01 gave you the opportunity of familiarizing yourselves with different tech stack possibilities.  So in most groups, there is likely to be a quick consensus on which tech stack to use.  But you should still discuss the pros/cons of each, and share your preferences with one another.

If you have questions, or need guidance, ask the course staff!

## A single paragraph

For the second item, focus *first* on writing *a single paragraph* in which you go into a bit more detail about what you plan for your project.

This is NOT intended to be a full specification of what you are going to build.  It is just an opportunity to *briefly* 
add a bit more detail that wouldn't fit into the one-sentence description.

## Then, consider user roles

How many different kinds of users are there, and what are their roles?

Examples: 
* A ride share app mvp has two kinds of users: those looking for rides, and those offering rides.  
  * A third kind of user role you might need is site admins, users that can have the power to delete anyone's posting.
* A game app might have only one kind of user: game player
* A Recipe sharer app might have two kinds:
  * Users that look up recipes, but can't add new data to the system
  * Admins that can upload new data to the system
  * Later, you might also allow user contributed content; in that case, you might want admins to have the ability to delete inappropriate content.

## Roles and Permissions

Think about the fact that your app will be available on the public internet.  If your app allows user contributed content of any kind, there is the potential for inappropriate content (spam, or worse) to be added.   One option is restrict your user base to folks with an `@ucsb.edu` login; we can provide some example code or point you towards resources that you can build on to add this feature to your app.

What will each different kind of user be able to do in your app?
* What are their goals in using their app?
* How does your app allow them to accomplish their goal?

## Team Homework: `.gitignore` and `LICENSE.md`

Before Thursday's lecture, as a team, please add a `.gitignore` and a `LICENSE.md` to your repo.

The `.gitignore` will depend on your tech stack choice.
* Create a file called `.gitignore` in the root of your repo
* For next.js, a good start is the `.gitignore` for Node, found here: <https://github.com/github/gitignore/blob/master/Node.gitignore>
* For a Spring Boot project, we would recommend the contents from this article: <https://ucsb-cs48.github.io/javatopics/gitignore_maven/>

For the `LICENSE.md`:
* Consult <https://choosealicense.com/>.
* The [MIT license](https://choosealicense.com/licenses/mit/) is a reasonable choice if you don't want to spend too much time troubling over this.
* Create a file called `LICENSE.md` in the root of your repo, and copy the license terms into that file.
