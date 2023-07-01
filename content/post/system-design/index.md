---
title: "System Design" # Title of the blog post.
date: 2023-07-02T01:42:18+04:00 # Date of post creation.
tags:
  - system design
  - interview
# comment: false # Disable comment if false.
---

Yesterday I watched a system design mock interview about designing Netflix. Key learnings:
1. Start by asking clarifying questions to define the requirements and defining the scope.
2. Take notes in real time on the screen in the same tool you'll use to design the system.
3. Extract the concepts which will be the data model.
4. Ask about the number of the users and the size and amount of data used.
5. Decide to go with SQL or NoSQL. You'll use a SQL database when you'd have complex queries. You'd use NoSQL for 
   unstructured data and when prioritizing availability over consistency. For example use PostgreSQL.
6. Always discuss the trade-offs and defend your decisions.
7. Always check with the interviewer making sure they are fine with the steps you take along the way.
8. The design started with adding boxes for the data, i.e. BLOB file store and then databases, the API.
9. Add in-memory cache for faster requests. For example use Redis.
10. You'd need to make calculations on the fly for the size of the data, using units like K(3), M(6), G(9), T(12), P 
    (15) bytes.

Like other skills, it takes daily practice to master the system design interviews. 


