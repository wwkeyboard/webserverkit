---
title: The First Connection
tags:
  - socket
categories:
  - one
slug: 1-first-connection
---

# Start Your Project

In this segment we'll set up the initial structure of the
application. I recommend you don't start trying to pick a framework or
listing out design patterns. Instead let's start simple. The first
step I pick is a `hello word` application, something that compiles(if
you need to compile), and runs.

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

# Open a Socket

At this point we have an application that reads a port number and
prints it to the screen. Great first step! But we need to get more
data into the server. To do this you'll need to open a socket and
listen to the given port. The socket documentation will provide the
manner for supplying the port along with other options. At this point
you shouldn't need to worry about them, learn what the defaults are
and go with them until you have a specific reason to make a
change. For a production system you'll want to review all of the
options to ensure they make sense for your needs.
