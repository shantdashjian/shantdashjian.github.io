---
title: "WebSocket vs HTTP" # Title of the blog post.
date: 2023-07-06T06:37:47+04:00 # Date of post creation.
tags:
  - websocket
  - http
  - communications protocol
# comment: false # Disable comment if false.
---

Yesterday I learned more about the [WebSocket communication protocol](https://en.wikipedia.org/wiki/WebSocket). 
Compared to HTTP(s), WebSocket allows:
1. Server to communicate with client without client first sending a request.
2. Multiple messages going back and forth between client and server in a single connection.

WebSocket is thus a better fit for applications that need up-to-date ongoing data communication, for example:
1. Messaging
2. Gaming
3. Trading

On the other hand, WebSocket lacks the HTTP verbs and status codes, thus HTTP(s) is still king for building RESTful 
APIs.
