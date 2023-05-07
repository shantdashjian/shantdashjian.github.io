---
title: "Code Reviews and APIs" # Title of the blog post.
date: 2023-04-23T10:39:06+04:00 # Date of post creation.
tags:
  - code review
  - api
# comment: false # Disable comment if false.
---

## Code Reviews
Yesterday I completed the code reviews module. Key learnings:
1. How to perform Scrim-based over the shoulder code reviews. I performed my first real code review of a solo 
   project for a student. I have nine more to go. I plan on doing one per day for the next 2 days.
2. How to do PRs. You create an issue, create a branch, make changes, push changes, create a pull request, it gets 
   reviewed, and then merged to main. In case of merge conflicts, reslve merge conflicts, recommit, push, create 
   pull request, approve, and merge.

## APIs
I started a new module on APIs. This is great as it gets path closer to fullstack development. The key learning is: 

<pre>fetch("url")
    .then(res => res.json())
    .then(data => element.textContent = data.message)
</pre>

