---
layout: page
title: "Static web server"
github-url: https://github.com/lierluis/static-web-server
---

This project was a multithreaded static web server written purely in Ruby, which
was developed to learn about the HTTP protocol and the underpinnings of the
Ruby on Rails framework.

Creating a connection through sockets, the server reads and parses HTTP
requests from a client, performs a series of operations, and returns an HTTP
response with the appropriate status code and resource (if applicable).
The project lasted from February to April 2016.

[Web server workflow (PDF)]({{ site.url }}{% link assets/file/web-server-workflow.pdf %})

**Concepts:**
* Hypertext Transfer Protocol (HTTP)
* Client-server architecture

**Technologies:**
* Ruby, HTML

**See more:**
* [View on Github]({{ page.github-url }})
* [Original documentation](https://goo.gl/0d0PWk)
