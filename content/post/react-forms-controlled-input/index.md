---
title: "React Forms and Controlled Input" # Title of the blog post.
date: 2023-05-17T08:01:42+04:00 # Date of post creation.
tags:
  - react
  - forms
  - controlled input
# comment: false # Disable comment if false.
---

## React Basics Continued
Yesterday I continued studying React basics. I went through forms and how to add two properties to an `input` 
element such that it becomes controlled:
1. `value={state}`: This ensures the value of the input displayed is changed whenever state changes from inside the 
   component, 
   by code.
2. `onChange={() => handleChange(e)}`: This ensures state changes whenever the value of the input is changed by the 
   user.
