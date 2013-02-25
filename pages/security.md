---
layout: page
title: "Security"
description: ""
---
{% include JB/setup %}

Security should be remembered at all stages of development.  Ignore it until later and by then it may be too late!  Here's a few reminders about common web-related security pitfalls.


Be Wary of Clear Text
----------------------

Learn what it means to pass data around in 'clear text' and understand whether that's a security risk for you or not.  Passing sensitive information in clear text is wrong and should be swapped out immediately with a secure solution.  This usually means adding SSL certificates to web sites and redirecting from http to https versions of pages with forms on them, but also applies to working with APIs, databases and libraries that send and receive data between servers.


How to Store Secrets
--------------------

Secrets in this case refers to those bits of configuration - passwords, API keys, etc. that only your app needs to know about.  You need to store them somewhere because your application needs to know them (and your application lives on several servers).

What you shouldn't do is store them in a versioning system, like Git.  Even if you've got a private repository, you may eventually make it public, or you may forget to revoke read-access to it to an ex-employee or something might happen down the line where git's ability to never forget a repo's history will come back to bite you.  This also applies in the case where you were storing a password in a repo, you realised the error of your ways and removed it straight away - the history is not so easy to unpick, so that secret remains discoverable.

Heroku has a good system for managing secrets and general application configuration, which is to have the app read everything it needs from environment variables, which only live on the servers they're needed on.  The setting of these is all managed centrally, setting up all nodes with the required info.

Puppet similarly controls configuration centrally, effectively relinquishing the required secret information to the nodes that need it, through a system of authentication.  There's still a need to have a backup of that secret information somewhere, in the event that the centrally managed store of info goes down and it needs to be reset.