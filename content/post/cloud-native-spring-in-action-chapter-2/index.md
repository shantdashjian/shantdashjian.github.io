---
title: "Cloud Native Spring in Action: Chapter 2" # Title of the blog post.
date: 2023-11-15T17:25:06+04:00 # Date of post creation.
tags:
  - cloud native
  - spring boot
  - spring
  - system design
# comment: false # Disable comment if false.
---

**Chapter 3 had 3 main parts:**
1. The 15 factors for building cloud native applications.
2. The hands-on exercise to design, develop, and deploy the first service in the system, the `catalog-service`. 
3. The system requirements and architecture.
   - It then provided an overview of all the concepts and technologies that will be covered and used through the 
     rest of the book while building the bookshop.

**The core technologies that I will use:**
1. Design it using the C4 model on `diagrams.net`.
2. Develop it using Spring Boot on IntelliJ.
3. Deploy it by first packaging it using Cloud Native Buildpacks abstracting Docker. Then deploy it on K8s. The 
   delivery will be automated using GitHub Actions. Then the deployment will be automated using GitOps and ArgoCD.
4. The K8s cluster will be hosted on a cloud provider: Digital Ocean.
