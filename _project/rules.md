---
layout: default
title: Rules
ready: true
desc: "Rules governing group formation, project selection, and project completion"
---

# Group formation

This quarter the instructional staff will assist and partly direct the formation of groups.

We will try to minimize the number of groups, subject to the restriction that no group may
have more than 6 nor fewer than 4 members.

Attendance is always important, but it is mandatory during the first week of lectures and
at your first discussion section.  Otherwise, you cannot be assigned to a group, and will
need to drop the course and take it next time it is offered.

All remaining rules apply after the groups are formed.

# Type of project to choose

CS 48 is mostly about analyzing problems and designing systems. It is not primarily
about programming, at least not programming at the method or even class level.
Therefore, what we are looking for in projects are problem domains that
are "interesting" - i.e., have

* around two dozen key concepts, and
* interesting relationships between these concepts.

<style>
.good-choice { background-color: lightgreen; }
.poor-choice { background-color: #ff8070; }
.highlighted-course-rule { background-color: lightyellow }
</style>

Suppose you have a choice between two projects, A and B.

<div class="row">
  <div class="col-sm-6">
    <div class="card">
      <div class="card-body good-choice">
	<h5 class="card-title">Project A: Good Choice</h5>
	<p class="card-text">
	  Has many concepts with complex relationships between them,
	  but each resulting class is simple to implement.
	</p>
      </div>
    </div>
  </div>
  <div class="col-sm-6">
    <div class="card">
      <div class="card-body poor-choice">
	<h5 class="card-title poor-choice">Project B: Poor Choice</h5>
	<p class="card-text poor-choice">
	  Has fewer concepts, and classes are difficult to
	  implement due to tricky algorithms and/or fancy graphics.
	</p>	    
      </div>
    </div>
  </div>
</div>


For CS 48, project A is a *much* better choice. A key goal is for you
to learn how to analyze and design, and thus a major portion of your
work on the project should be in that area.

# *Almost* any type of project you want

Good news! You may choose *almost* any type of project you
want&mdash;subject to some limitations:

The first is that you must create **something that someone will actually use**.
* If it's a game, it should be a game people will actually play, and enjoy playing
* If it's a tool, it should be a tool people will actually use.

As an example of something that you could build, but that would NOT be
acceptable: supposed you built a better interface for a ride sharing
service such as Lyft or Uber.  That's clearly useful to someone.  But
no-one is actually going to use it, unless you *actually have* a bunch of willing
drivers ready to start driving people around using *your app*.

Another example: an airline reservations systems.  Unless *you own
planes*, and have airport slots, and cleararance from the FAA, etc, you
aren't going to be able to actually have anyone try out *your system*
for *real*.

# Why do we need real users?

We are concentrating on the Agile software design methodology.

* Involving actual users in the design of the software is essential to Agile
* If there are no *real* users, there is no *real* Agile.

You get plenty of practice writing code that no "real" user will ever
use in CS8, CS16, CS24, CS32, CS64 CS130A, CS160, CS170, and many more
courses.  There are very few courses in the curriculum where you have
the opportunity to write code for real users: those being CS48, parts
of CS56, and capstone (CS189A/B) if you take it.

So concentrate on something that people can actually use.

# Programming language and other source code requirements

As CMPSC 32 is a pre-requisite for this course, every enrolled student is assumed to possess
sufficient C++ programming knowlege to be an effective team member if the project is mostly written
in that language.

CMPSC 56 is another required course for CS majors, many students have
or are gaining experience with the Java programming language and
related libraries.   If all of your team members are comfortable with Java, that's an acceptable choice.

Another object-oriented language may only be used with explicit permission, and only if there is a compelling
justification for using that language in contradistinction to C++ or Java.

For webapps, client side code may be written in JavaScript, but it should be
well-structured, well-organized and well-tested JavaScript.

</div><!-- card-text -->
</div><!-- card-body -->
</div><!-- card -->

# Additional Requirments.


## C++ specific:

* Should conform to the [Google C++ Style Guide](https://google.github.io/styleguide/cppguide.html)

## Java Specific

* Should conform to the [Google Java Style Guide](https://google.github.io/styleguide/javaguide.html)

## Python Specific

* Should conform to the [Google Python Style Guide](https://github.com/google/styleguide/blob/gh-pages/pyguide.md)

## JavaScript Specific

* Should conform to the [Google JavaScript Style Guide](https://google.github.io/styleguide/jsguide.html)

# Originality Requirements

* The code for which you receive credit must be *original*&mdash;written by **your group** during
  *this quarter* for *this course*.

   * Of course, your source may use any parts of the standard libraries, but consult with your
     TA/mentor before incorporating third-party libraries.

* **Note:**  your system design must be original too, or it must be properly
    credited. See the special note about plagiarism below.

<div class="card">
<div class="card-body highlighted-course-rule">
<h5 class="card-title" >
About technical expertise
</h5>
<div class="card-text" markdown="1">

The instructor and TAs will *not* assume responsibility for teaching you how to accomplish every
possible programming task you need to learn - whether or not we are familiar with these tasks
ourselves. A large part of a developer's job is to learn how to do things they have not been
trained to do. You must research any techniques that are novel to you: find examples in books
or by searching the Internet.


</div><!-- card-text -->
</div><!-- card-body -->
</div><!-- card -->


# Grading guidelines

The group grade is based on your final system demo and final code review.

All project team members in good standing will receive the same grade
for this portion of the project.   To remain in good standing, you should have
* an acceptable level of attendance/participation in standup meetings
* an acceptable level of attendance/participation in group discussions
* an acceptable level of contribution to the teams progess.

# Good Standing on your Team

The initial determination as to what an acceptable level of participation is will
be defined by consensus of each group during the "team norming" activity
at the start of the quarter.

For example, a team might define "acceptable attendance/participation at standups meetings" with some combination of norms like the following:
* A team member should not normally miss a standup 
* The team may occasionally excuse a member from standup attendance by unanimous consensus when there is a legitimate reason to miss it.
* If it is necessarily to miss a standup, the team member should communicate with the team as soon as possible; in advance if possible, or as soon as possible afterwards when not.
* A team member that misses more than k consecutive standups is not in good standing.
* A team member that misses more than n during a quarter is not in good standing.

Course staff will take attendance at standups, but it is up to teams themselves to hold each other accountable to their team norms.  If a team member is not in good standing, or is in danger of not being in good standing, it is the responsibility of the team to reach out to course staff---mentors, TAs, and instructors---early, and often---for help in resolving the situation.  You can't just "vote someone off the island" on the last day of the course.  You have a responsibility to make every effort to resolve the situation early, and successfully, to document your efforts to do so, and to involve staff in those efforts as early as possible.

Ultimately, the decision about whether a team member is in good standing lies with the instructor.  However, the instructor will use the norms, and communication processes established by the team, as well as its own documented efforts to resolve the matter, in making a final determination.

A team member that is not in good standing with their team will
receive a reduced grade, or a zero for the project portion of their
final grade.  Note that a zero on the project portion guarantees a
failing grade in the course.

# A special note about plagiarism:

All work that you submit must be entirely your own, or its origin must
be properly credited. In other words, it is okay to borrow an idea
from somewhere, but only if you tell us so. (Of course, if you borrow
a substantial part of your design, your grade may be affected.)

Plagiarism is a very serious offense, and we are obligated to spend
some effort trying to find it. If we detect it, the offending group's
grade will be reduced by at least 40 percent even for minor
infractions. For anything other than a minor infraction, the grade
will be zero, and the students' behavior will be reported to the
appropriate university authorities. According to university
guidelines, "any act of academic dishonesty ... is unacceptable and
will be met with disciplinary action".


Credits:
* Updated December 27, 2018, P. Conrad.
* Based on previous CS48 course material from  provided by C. Michael Costanzo and Chandra Krinz.

