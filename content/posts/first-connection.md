---
title: The First Connection
tags:
  - socket
categories:
  - two
slug: 2-first-connection
---

# Open a Socket

At this point we have an application that reads a port number and
prints it to the screen. Great first step! But we need to get more
data into the server. To do this you'll need to open a socket and
listen to the given port. Once you have the socket listening you'll be
able to make a request with curl or a browser and see the actual HTTP!

The socket documentation for your language will probably start by
explaining how to connect to a server that's already running, you'll
need to find the part about binding to a socket address and listening
for connections. This should also explain the method for supplying a
port number along with other options. At this point you shouldn't need
to worry about the additional options, learn what the defaults are and
go with them until you have a specific reason to make a change. For a
production system, on the other hand, you'll want to review all of the
options to ensure they make sense for your needs.

Once you are listening to the socket you'll need to handle incoming
connections. For now read all the data from the connection and print
it to the screen. To test this start the application and make a
request to the port you specified. If it looks like curl or your
browser is spinning you may need to explicitly close the socket once
you've read data from it.

# Outcomes

* Open a socket on a given port
* Listen for connections on that socket
* Print the received data to the screen

# Googleable Words

* { language } socket listener
* { language } socket close
* { language } tcp server example
* curl http
