---
title: Start the Project
tags:
  - project
categories:
  - one
slug: 1-start-project
---

# Start Your Project

In this segment we'll set up the initial structure of the
application. I recommend you don't start trying to pick a framework,
listing design patterns, or drawing UML. Instead let's start
simple. First let's start with a `hello word` application, something
that compiles(if you need to compile), and runs.

Once you have this we'll need to start with a command line
argument. This will be the port our server will listen on. I recommend
you convert this to an integer and print it to the screen.

At this point if you haven't start source control now would be a
great time. Initialize the repo of your favorite SCM and add the
application. At this point you'll have enough of the build created to
know what temporary or generated files come out of the
language. You'll want to mask those out early so as to keep the
repository small(er).

This process of discovering how a build is structured in your language
can take some time. It's often complicated and there can be large
differences between hello-world applications and real world build
systems. If you intend to learn a build system it's fine to experiment
with one, however getting bogged down with the details and caveats of
a build can slow down your exploration of a new language. At this
stage it's okay to use a shell script, a makefile, or even copy-paste
from a notes file. It's your project and you can do what you want!
However, if you are familiar with the language you're working in now
would be a great time to learn how it's preferred build system is
configured.

# Outcome

At the end of this step you should have:

* A directory for the project
* Source control for the project
* "hello world" that takes an argument from the command line
* Enough build to run the "hello world"

# Googleable Words

* { language } hello world
* { language } build process
* github new project
