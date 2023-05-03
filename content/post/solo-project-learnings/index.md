---
title: "Solo Project Learnings" # Title of the blog post.
date: 2023-05-03T22:20:15+04:00 # Date of post creation.
tags:
  - solo project
  - html
  - css
  - javascript
# comment: false # Disable comment if false.
---

## Solo Project Learnings
Yesterday I submitted my Movie Watchlist solo project for review. Here are things I learned working on the project:
1. Add `charset` to the `<script>` tag in your HTML, in order to ensure the HTML rendered using JS doesn't replace 
   characters like the apostrophe `'` with some weird characters.
2. Use `utils.js` to include utility functions.
3. Use `window.location.href.includes()` to check which HTML page you are on.
4. Add an event listener for `keydown` to check if `Enter` was pressed.
5. Use comments to organize your CSS.
6. Use `::before` to add opacity to your background image.
7. Use `text-overflow: ellipsis` to replace last three characters in an overflowing text with `...`.
