---
title: "Communication Styles in Microservices" # Title of the blog post.
date: 2023-07-13T08:39:03+04:00 # Date of post creation.
tags:
  - microservices
  - communication styles
  - rest
  - rabbitmq
  - message queue
# comment: false # Disable comment if false.
---

There are two communication styles in distributed systems:
1. Direct, a.k.a. synchronous
2. Indirect, a.k.a asynchronous

**Direct communication** is used when a service wants to send a command to another, or when it wants to orchestrate a 
sequence of behaviors by multiple services, or when it needs to get an immediate response for its request. **The 
upside** of using direct communication is that it's easier to do, compared to indirect communication. **The 
downside** of 
direct communication is the tight coupling and the single point of failure. **Using REST** is an example of direct 
communication.

On the other hand, **indirect communication** is used when a service wants to notify one or more services of something, 
and 
when an immediate response is not needed. **The upside** of using this style is the loose coupling and the 
elimination of 
the single point of failure we get with direct communication. **The downside** of it is the added complexity to set up 
indirect communication. **Using a message queue like RabbitMQ** is an example of indirect communication.
