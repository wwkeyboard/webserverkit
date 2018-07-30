---
title: Start Parsing the Request
tags:
  - parse
  - header
categories:
  - four
slug: 4-parse-uri.md
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

A request coming from the curl utility will look something like this.

``` bash
Request: GET / HTTP/1.1
Host: localhost:8080
User-Agent: curl/7.58.0
Accept: */*
```

Starting on the first line you'll notice the HTTP verb of this request
`GET` and the path that's requested `/`. If you change the options to
curl you'll notice this line change. We'll start by parsing out this
line.

At this point your adventure is going to take a bit of a turn based on
what language and programming style you're using. Many of you will be
doing some sort of Object Oriented or procedural programming. In this
case you'll probably want an object or stuct to represent the request
and the information about that request you've parsed out. If you want
to use a different form of programming, you'll still need some
internal representation of the request in your codebase. Be as
creative as you feel necessary for this project!

# outcome

* representation of the request in code
* Extract the path and verb from the request
