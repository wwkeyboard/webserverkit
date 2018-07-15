---
title: Start Parsing the Request
tags:
  - parse
  - header
categories:
  - three
slug: 3-parse-uri.md
---

# Start Parsing the Request

At this point the server is accepting connections, reading the request
from the socket, then printing it to the screen. The next step is
parsing information out of that request. These requests can get quite
complex, especially when they come from a browser. Modern browsers
advertise their willingness to accept a number of optimizations as
well as report a bunch of information to the server. If this is your
first time digging through an HTTP request it can be a little alarming
just how much information you offer just to see if the server will
give you some HTML.



# Outcome

* Representation of the request in code
* Extract the path and verb from the request
