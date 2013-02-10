---
layout: page
title: "Testing"
description: ""
---
{% include JB/setup %}

Test Everything!
----------------

Every new bit of code you write should be proved to be doing the job you wanted it to in some sort of repeatable, automated test.  If it's not tested then it doesn't go in.



Jenkins
---------

We use Jenkins as our continuous integration server.  He sits there waiting for any code changes before he goes and runs all of the tests to give the green light on new releases.

### Add new projects to Jenkins from the start

When a new repo is created, add it to Jenkins.  We track the master and develop branches so that we can see the whole picture on development before knowing for certain that the code is at least ready for a release.

It doesn't matter if there are no tests or if it's not set up right.  As soon as it's in there, everyone can have visibility that these things need to be done.

### How to add a new repo or branch to Jenkins

TODO: Explain how to add to the jenkins templates
TODO: Explain jenkins.sh

### Add your feature branch if development is long-running

For big features, it can help for Jenkins to track the feature branch and show the status of all its tests.  It's easy to do and provides visibility to everyone immediately.



Top-Down or Bottoms-Up?
-----------------------


Mocking
--------




