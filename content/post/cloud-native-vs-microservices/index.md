---
title: "Cloud Native vs Microservices" # Title of the blog post.
date: 2023-08-24T14:10:27+04:00 # Date of post creation.
tags:
  - cloud native
  - microservices
  - architecture
  - system design
  - cloud
# comment: false # Disable comment if false.
---

Many software developers and even authoritative voices in the software industry use the terms **cloud native** and 
**microservices** interchangeably. While studying with the excellent book [Cloud Native Spring](https://www.manning.com/books/cloud-native-spring-in-action?experiment=B), I decided to dig deeper into the differences between those two 
approaches.

The experienced [Thomas Vitale](https://www.linkedin.com/in/vitalethomas/) emphasizes that the book is about building 
cloud native 
applications, and not necessarily about microservices. He points out that he adopts a **service-based** architectural 
style. He explains that this allows for services of any size: small, big, and everything in between. I inferred from 
it that a system built using 
the microservices-based architectural style must consist of all small/micro services.

I decided to give the matter further thought to further understand the differences, going beyond just the size of services difference. Here is what I concluded:

1. A **cloud native** system consists of one or more services of any size. It could be a monolith that is modular, 
   many small/micro services, or anything in between. **Microservices** must consist of many small/micro services, each 
   loosely coupled and highly cohesive, each separate and doing one thing.
2. A **cloud native** system must leverage the cloud. It's in the name. **Microservices** don't have to. They can be 
   hosted fully on premise.
3. A **cloud native** system leverages elasticity, i.e. auto-scaling that comes with using the cloud as the platform. 
   **Microservices** don't have to.

The cloud enabled more systems to go the microservices path, but it doesn't require systems to do that in order to 
leverage the benefits of the cloud, i.e. become cloud native. Going cloud native is more that just the size of 
each service. It's about achieving the goal of better scalability, better resilience, higher speed to market, and lower 
costs,
using the cloud as 
the platform, and utilizing the practices of automation, continuous delivery, and DevOps.


