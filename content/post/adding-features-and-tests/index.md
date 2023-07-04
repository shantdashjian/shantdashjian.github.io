---
title: "Adding Features and Tests" # Title of the blog post.
date: 2023-07-04T16:38:10+04:00 # Date of post creation.
tags:
  - npm package
  - adding features
  - testing
  - jest
  - tdd
  - refactor
  - armenian-names
# comment: false # Disable comment if false.
---

Yesterday I worked further on my [armenian-names NPM package](https://www.npmjs.com/package/armenian-names). 
1. I added new features to enable users to get random names for boys and girls that start with a certain letter or 
   letters. This was in response to requests from people I spoke with who said they'd like to see that feature in 
   the package.
2. I also added tests written in [Jest](https://jestjs.io/) for existing functionality. I then used TDD to add the 
   new functionality and refactor my code for maintainability.
3. I also extracted data into a separate file for better separation of concerns.

As of now, I'm at version 2.2.0 and have 161 downloads in 2 days since I published the package. This is already an 
awesome accomplishment.
