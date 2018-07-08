---
title: The First Connection
tags:
  - socket
categories:
  - one
slug: 2-first-connection
---

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
