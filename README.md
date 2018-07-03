Dear Software Development instructor,

A lot of times, we inherit course materials from another instructor, yet it is not usually clear why certain elements of the course are the way they are.
I hope that this document will help demystify some of the CS121 course components, provide a bit of history and motivation for them, and help you improve your own course.

I put a lot of work into these materials, and I would be delighted if you find them useful and decide to adopt them for your own course.
If you do, I ask that you fork this repo and when making the changes, please, leave the ["Copyright and Licensing"](#copyright-and-licensing) section intact.

Thank you, and good luck!

~K


<!-- TOC depthFrom:1 depthTo:6 withLinks:1 updateOnSave:0 orderedList:0 -->

- [Introduction](#introduction)
	- [Previous course changes](#previous-course-changes)
	- [Changes I implemented during Spring 2017](#changes-i-implemented-during-spring-2017)
	- [Changes for Fall 2017 and their relationship to Clinic](#changes-for-fall-2017-and-their-relationship-to-clinic)
	- [Spring 2018 focus](#spring-2018-focus)
- [Syllabus](#syllabus)
- [Course Objectives](#course-objectives)
  - [Group Project](#group-project)
    - [Goal: Gain experience on a big\* software project](#goal-gain-experience-on-a-big-software-project)
    	- [Self-organized teams of four.](#self-organized-teams-of-four)
    	- [External clients.](#external-clients)
    - [Goal: Gain experience as a project manager (PM) and working with a shared code base](#goal-gain-experience-as-a-project-manager-pm-and-working-with-a-shared-code-base)
    - [Goal: Gain experience estimating productivity and managing their time](#goal-gain-experience-estimating-productivity-and-managing-their-time)
    - [Goal: Gain experience with software engineering tools](#goal-gain-experience-with-software-engineering-tools)
    - [Goal: Gain experience working with a new development environment and set of libraries](#goal-gain-experience-working-with-a-new-development-environment-and-set-of-libraries)
  - [Presentations and Communication](#presentations-and-communication)
    - [Goal: Gain experience communicating technical information](#goal-gain-experience-communicating-technical-information)
- [Schedule](#schedule)
- [Copyright and Licensing](#copyright-and-licensing)

<!-- /TOC -->



#### Introduction
As I embarked on redesigning CS121 at Harvey Mudd, I interviewed all faculty in the department to figure out where the course fits in the curriculum and what its learning outcomes should be.

One of my main questions was: "Is this course supposed to be about **software** development or software **development**?"
If it was the former, my goal would have been on the specific tools and exercises that ensure that students get practice with various technologies and create a software product.
Since the faculty agreed that it was the latter, the course became about the **process** of development, and as such, the structure of _how_ students develop a project becomes more important than the knowledge of a specific language or a software tool.


Additionally, since CS121 is a prerequisite for students' capstone experience in  [Clinic](http://www.cs.hmc.edu/clinic), the faculty supported my desire to change the course to align it with what students will need in order to succeed during Clinic (e.g., skills, templates, resources).


After talking with the four instructors who had taught this course before, I learned that CS121 has gone through several changes in structure/focus.

###### Previous course changes
* Introducing an iOS app development at the beginning of the semester (using a toy app example)
* Having all students in the section use the same platform (e.g., all iOS or all Android) versus using different platforms during the same semester (examples included iOS, Android, Node.js, Unity)
  * I found out that while having multiple platforms in the course allows for a greater selection of the projects, troubleshooting and managing them is a pain
  * providing assignment instructions (e.g., for Architecture report) becomes a nightmare when there are multiple platforms in use in the course -- inevitably students end up complaining that assignments are irrelevant, because the instructions don't apply to their project (e.g., a web-based project needing to document UML classes, which they don't have in their product)
* Having student-proposed semester-long group projects versus inviting technical or non-technical external clients to provide semester-long group projects
  * instructors warned me that having students work on their own projects can be problematic, because they tend to run out of steam or become disinterested.
* Varying group sizes from 3 to 5
  * If there are three or fewer students, then it gets harder to motivate the need for collaborative project management tools: students tend to think of them as an unnecessary overhead, since it can be easier to coordinate tasks without them.
  * If there are five or more students, then it can become challenging to ensure that everyone on the team can make a substantial contribution. Additionally, managing group dynamics can become trickier as the group gets larger.
  * Four students per team seems to be best.
* Having a single PM versus having all students rotate as PM
  * Given that one of the main objectives for the course is to prepare students for Clinic, it is reasonable to give each student a chance to experience this role.


I decided to first focus on the structural changes of the course before making any substantial changes to the course content.

###### Changes I implemented during Spring 2017
* **Issue**: students' culture / stigma / attitudes about the course
* **My Solution**: make 121 unrecognizable (change its schedule and format, development platform, etc.)
  * instead of starting on their respective projects at the beginning of the semester, the first part of the course (about 6 weeks) focused on providing concepts and fundamentals along with some time to explore the new development platform (Rails)
  * students still had four phases to work on their projects, except that now there were just two weeks per phase
  * everyone got to use Ruby on Rails 5
    * almost everyone was new to this development framework: students who had lots of previous experience could still learn something new for them, while the less experienced students felt a bit less intimidated, since nobody was "an expert"
    * Rails is a beginner-friendly framework that allows one to have something up and running in less than an hour
    * Rails allowed students to create web apps, which is something that they don't get to do in other courses
    * having a standardized platform allowed me to share more focused resources, write clearer assignments, simplify debugging, and allow students to ask each-other for troubleshooting tips


* **Issue**: assignments (that focus on planning or documentation) are
seen as busywork that takes away from development time
* **My Solution**:
  - provide examples / templates
  - introduce peer-review of each assignment draft


* **Issue**: lecture material is seen as not relevant to projects
* **My Solution**:
  - one lecture on each topic directly relevant to projects
  - lots of hands-on practice (teamwork using whiteboards)
  - status reports are submitted using a written document (instead of as a quiz on Canvas)
  - PM presentations explain the phases of the project (+ reflect on the video of their presentation)

* **Bonus**: get to know students by scheduling 15 min interviews + "Getting acquainted" survey
  * My first meetings were scheduled using Google Calendar's appointment system; in subsequent semesters, I switched to a great tool called [Calendly](https://calendly.com/) (yay for automatic 5 min breaks between the meetings!).
  * The [Introduction survey](https://goo.gl/forms/X0fkxkW7xcFxKhej2) initially included my answers to the questions to serve as examples. However, since I saved the filled-out student forms as PDFs (to use as a guide during our meetings), I got tired of removing the first two pages, which contained my answers, so I excluded it from the subsequent forms;
  the linked survey from Fall 2017 also has additional prompts, e.g., for the preferred gender pronouns.

###### Changes for Fall 2017 and their relationship to Clinic
* Create a portfolio using the materials submitted for the course
(teamwork/interests survey, progress logs, reflections, final write-up)
* Ask the faculty in the department to emphasize to students the benefits of this course, e.g., how this course is going to help them with open-ended projects
* Add a quick reminder of CS121 concepts to one of the Clinic Tuesday sessions
* Begin generating resources that would help students during Clinic;
Areas of focus are
  * Time management (try a premium trial of KanbanFlow)
  * Team dynamics (update phase evaluations, match the Clinic rubric)
  * Presentation (update the rubrics, include reflection)
  * Writing (incorporate LaTeX)

###### Spring 2018 focus
* Provide more practice using git/GitHub
  * help students understand the open-source workflow
  * provide several tutorials to practice git/GitHub concepts
* Provide more practice writing in LaTeX using Overleaf
  * start with the first document they submit as a group
  * provide templates for all group assignments (e.g., phase plan, chapters of the final report)
* Improve presentation and poster guidelines
* Add more reflection opportunities for PMs in their reports (e.g., what can you do better, dev ratings and assessment)



This repository is a collection of materials from the Spring 2018 version of the course, with some additional materials from previous semesters.

### Syllabus

[Google Doc version](https://docs.google.com/document/d/1mjoCNHRznlpP5Z4dQvKB9Wgj4cRoTExARePnLazdBto/edit?usp=sharing) (depending on the browser, it does not paginate in the same way as in the [PDF version](https://drive.google.com/open?id=1xdE6-9VgQBRGdkbT6y_2BBqwPCT3-gI4))

**Notes**:
I worked with Yi Luo on restructuring the syllabus to make it more streamlined.
A lot of sections can still be improved (e.g., "Tips for Success") but at least we have a good start.

I recommend reviewing the "Late Policy" and clarifying whether 20% are rounded up or truncated. Grutors definitely need to know this info.

The three (3) excused absences should probably be moved to the "Class Participation" section.  It is currently challenging to accommodate this calculation through the rubric on Canvas, since the participation-tracking mechanism on Canvas doesn't allow a student's absence to not count against the grade.
This consideration is one of the reasons for the warning in the "Dispute of Grade Policy" section (while another reason for that warning can stem from the fact that some grades might not be released to students, e.g., due to a delay in grading).

---

### Course Objectives
Below are the goals for some class elements, which are listed on the syllabus.

#### Group Project
##### Goal: Gain experience on a big\* software project

\* _for some definition of "big"_

* Students will self-organize into (or be assigned to) project teams of four (with some teams of three depending on class size).
* Project teams will complete a group project for an external client.

###### Self-organized teams of four.
I let students select who their teammates will be - I am not involved in any way (this way they cannot blame me for putting them on a "bad" team).
Such self-organization does lead to a per-college separation: since off-campus students might not know others, they tend to form teams with students from their home college.
A team with students from different campuses usually runs into difficulties scheduling in-person meetings and coordinating their work -> help them be cognizant of this potential issue from the start.

Groups of four seem to be ideal.
See the section ["Previous course changes"](#previous-course-changes) to read more about the team size consideration.
Having four people on the team lends itself nicely to the current four-phase structure of the course (see the next goal).

###### External clients.
The clients for the projects are typically people from the community who I happened to know personally or who came to me with a problem that they hoped we could solve.
I learned the hard way that the instructor should _not_ be the client: students can end up being more on-guard, since they don't know when they are being evaluated and might feel less comfortable coming to you for help.
I had great success with students (who are not taking the course) proposing a project.
Usually, it's best when there exists a prototype or when the client has a strong vision for the final product.
I like when students are exposed to non-technical clients, however, it poses challenges with calibrating expectations.
If a client is unaware of what is possible and/or really happy with _whatever_ students deliver, it seems to take away the team's motivation to strive to improve (because it doesn't seem to matter how well they do) and leads to general dissatisfaction with the project.


##### Goal: Gain experience as a project manager (PM) and working with a shared code base
* Each team member will serve as project manager for one phase (approximately two weeks).
* Each team member will serve as software engineer for three phases (they’ll do much more than code though).

Sometimes, the class size does not evenly divide into teams of four students.
In those cases, I try to create teams of five, letting students to decide in which phase they want to have two PMs.

Students tend to like that they get to be a PM;
they might not necessarily like the experience with their team/project or learn that they don't ever want to be a PM, but they seem to value that they got to have this experience.

When students decide who gets to be a PM for each phase, I give them the following rough guidelines:
* the first PM should be very comfortable with uncertainty and ambiguity, since there will be plenty of it as the team is starting out
* the second PM is usually in charge of making sure that the initial design and plan are gaining traction
* the PM for Phase 3 is usually leading one of the most stressful phases as the team is potentially pivoting their project and/or trying to merge their changes and add final features in preparation for the wrap-up in the final phase
* the last PM's focus is mainly on writing to make sure that the team provides a complete and well-documented project; if the project hasn't been on track, this person is also responsible for managing the addition and/or merging of the final features


##### Goal: Gain experience estimating productivity and managing their time
* Each team member will maintain a work log and submit weekly status updates.

[Status report template](https://docs.google.com/document/d/1C1y2t1av2OlrO08fGWFlhN4-7265dw4SbYS0Q9_gYls/edit?usp=sharing)


This goal is one of the most challenging aspects of the class for both, students and the instructor(s).
For most students, this is their first time planning and keeping track of their work, and they dislike how much it challenges the way they tend to work.
Most of them, instead of planning their week in advance and then keeping track of their efforts, end up writing their log at the end of the week, trying to remember what they've done.
Others, having developed their own successful workflow, find the provided system cumbersome and unneeded (no matter what that system actually is).

Additionally, the eight-hour weekly work limit (with up to two extra hours counted for points) ends up being a source of much of their complaints:
- for some students, 8 hours is not enough time, since they end up working more (either because they are making a lot of progress or they just naturally are slower than the assumed pace);
- for others, 8 hours/week is too much time and they don't know what to fill it with.

Grading status reports that were written as a continuous log made it easy to see students' progress.
However, providing feedback, especially, in a timely manner was still difficult:
currently, Canvas does not notify students about the received feedback - they have to actively check for it.
If someone submits their status report late, grutors don't tend to go back to grade things that haven't been graded, plus, the student misses out on a chance to get feedback that they probably really need (having two meetings per week with the grutors might help solve this issue).


##### Goal: Gain experience with software engineering tools
* Students will work in teams to practice aspects of the software engineering process.
* Project teams will submit software engineering products like user stories, project writeups, etc.

##### Goal: Gain experience working with a new development environment and set of libraries
* Students will complete development tutorials.



#### Presentations and Communication

##### Goal: Gain experience communicating technical information
* Students will develop and refine a software project.
* Students will provide feedback on their classmates' project.
* Students (while serving as the project manager) will present their team's progress.
* Students will provide feedback on all individual and group presentations.
* Students will summarize their weekly progress at a level appropriate for a non-technical manager in weekly status reports.

Technical communication through formal writing needs to be added to the bullet points.
* Students will produce technical reports that document their work on various project components.

* Students will communicate their progress, accomplishments, and setbacks to their client and course staff.

* Students will produce a poster and present their work at a Poster Session at the end of the semester.

---
## Schedule

Schedule as well ways to present it to the class has undergone many changes.

To be continued...

---

## Copyright and Licensing
<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a>

This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>.
This license lets others remix, tweak, and build upon this work non-commercially, as long as they credit this work and license their new creations under the identical terms. Read more about the <a href="https://creativecommons.org/licenses/">available licenses</a>.

These materials build on the resources shared by Harvey Mudd College's CS121 instructors and the HMC Clinic staff.

Original GitHub course link: https://github.com/hmc-cs121-admin/hmc-cs121-s2018 (created by Yekaterina Kharitonova)
