---
title: Return Something
tags:
  - response
  - header
categories:
  - three
slug: 3-return-something.md
---

Now that we can get something from the browser we should send something back. You can see what an HTTP response looks like by passing the `-v` option to curl. If you `curl -v google.com` you'll notice lines prepended with `>`, these contain the data sent to the server. It should look a lot like the requests you observed in the previous step! There are also lines prepended with `<`, these contain the headers of the response from the server.

In the case of google.com, and most major sites, the first line will start with `HTTP/1.1 301 Moved Permanently`. This is called the Status Line; the first part says the protocal is `HTTP/1.1`, and next is the response code followed by a text description of that code. Most major sites will respond with `302` redirecting you to either a `www.whatever` subdomain, or will send you to an https version of the site. This is appropriate behaviour, but beyond what we'll cover at this step.

For now we're interested in the structure of the response, and if you notice the html at the bottom. After the status line is a number of headers. The headers are of the form `Header-Name: header value`. For example `Date: Tue, 31 Jul 2018 02:00:53 GMT`. There is some debate about what headers are prudent to send, but most clients are able to deal with a response that has no headers. So we'll start with that. 

You should build a response in a string that has a status line followed by some "hello world" html. The response can look like this.

```
HTTP/1.1 200 OK
<HTML><BODY>hello world!</BODY></HTML>
```

Hard code that response and send it back through the socket after an incoming connection is made. Once this is running use your web browser to make a request to the running server.