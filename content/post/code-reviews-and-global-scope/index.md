---
title: "Code Reviews and Global Scope" # Title of the blog post.
date: 2023-04-27T10:53:58+04:00 # Date of post creation.
tags:
  - code review
  - fetch
  - global scope
# comment: false # Disable comment if false.
---

## Code Reviews
Yesterday I completed another code review, adding up to 5 total. Things are going well on that front, as I follow my 
daily process of reviewing material and providing code reviews for students. I plan to do another 3.

## My Solo Project
I also completed and submitting my own solo project for review. It's part of the APIs module, practicing `fetch`. I 
also used the `color` and `select` HTML input field types. In addition, I came across an issue trying to hook a 
function to `onclick` attribute in HTML. Because I imported my JavaScript as a `type="module"`, its functions are in 
a local module scope. The fix was to put the function under the `window` object, making it in the global scope, thus 
accessible for `onclick`. I made good use of `ChatGPT` as a peer to figure that out. 
