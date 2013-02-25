---
layout: page
title: "Project Management"
description: ""
---
{% include JB/setup %}


We stick pretty firmly to the Agile SCRUM software development methodology.  I won't go into great detail about what that means, but here's the way we work:

Sprints
-------

We have a two-week 'sprint', which is a block of time dedicated to working on a set of tasks laid out at the beginning that won't change in the middle.

Planning
--------

Good planning takes time.  Sorry bosses, but it has to be that way or the actual sprint will suffer.  During planning, bite-sized tasks are pulled out of a backlog of features, refined until everyone understands what it's about, estimated and added to the sprint.

Estimations
-----------

The whole team are involved in estimating each task.  This way, the experience of many are used to cover all bases - the established team members know about legacy code in the application and the new team members might bring new ways to solve a certain problem.  A consensus is agreed upon that is realistic, which is vital for understanding what's possible to achieve during a sprint.  With each sprint down, the estimations of individual tasks and the backlog features overall get more and more accurate, especially if the team is made up of the same developers each time.

Daily Standup
-------------

We hold a daily stand-up meeting at 10am.  It should last no longer than 10 minutes, involves the whole team and everyone has to tell the others:

* What they did yesterday
* What they're working on today
* Any blockers they might have

It's not a way to keep tabs on people and know whether they're skiving off or not!  The main reasons to have it are so that the team has a good understanding of where everyone is at and what it is we're all working on.  More importantly is the result that blockers are caught early on and help given (in whatever the best form for that is), which will be arranged for a time after the meeting.

>*Don't be late for standup!*


Demos
-----

It's important during planning to define what the team expects to see as deliverables at the end of the sprint.  These are the tangible end results of your hard work, which you then get to demo to the whole team at the end of a successful iteration.

Make sure to get ready for a demo before you give the demo.  The law of Sod indicates that your demo will not go well and will take ages of everyone's time if you don't have it ready.


Retrospective
-------------

It's important to spend a little time looking back at each sprint, in order to fix any process that was broken for the next one.  And to do more of what was done well!


More on Tasks
-----

> We use [Asana](https://app.asana.com/) for managing the tasks we're working on.  It holds all the information needed for each task, as well as who's doing what and what has been completed to date.

Tasks are entered in a simplistic form, along with the agreed estimation.  There may be more details inside a task, or there may not.  They're positioned in priority order, though take a pragmatic approach to deciding what the next task you do is, depending on whether you're waiting for other tasks to get done beforehand.

When you've got nothing to do, simply grab the next task off the list by assigning it to yourself.  Also, we use a ToDo/In-Progress/On-Hold/Waiting for Sign-off system to denote what stage each task is at.

We also have a physical board with copies of all the tasks on it, which is a much easier way of looking at the whole sprint and how it's progressing.  Make sure that when you alter the status of a task in Asana, you also update the board.  This will be necessary until such time as we build a robot that will automatically keep the board in sync with Asana.

### Make sure you know what you're building

Even if you think you know exactly what you're about to attempt when grabbing a new task off the pile, it's always a good idea to double-check with whoever created the task in the first place that you'll be delivering what's expected.  If deliverables are clearly defined, they indicate to you exactly what it is you'll be demoing to the team at the end of a sprint, which means there will be no last-minute rush to change it all around because you forgot to add this or that.

If a task doesn't put a specific deliverable in your mind, don't be afraid to ask for clarification.

### Asana's github Hook

Once you've set it up right, if you add a '#' and then the number of an Asana task ID to one of your git commits, when pushed up to github Asana will add a commit message into your task.  Handy!

<!-- TODO: How to set it up right. -->