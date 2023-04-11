---
title: "Responsive Design and React Basics" # Title of the blog post.
date: 2023-04-11T09:56:34+04:00 # Date of post creation.
tags:
  - responsive design
  - react
# comment: false # Disable comment if false.
---

## Responsive Design
1. Using `em` works fine for margin and padding as it is based on the font size of the element itself. On the other 
   hand, it is not recommended to use `em` for font size because that is based on the font size of the parent which 
   leads to a compounding effect that is better off being avoided. A better, recommended approach for font size is 
   to use `rem`, i.e. `root em`, which as the name implies, is based on the font size of the root, i.e. `16px` by 
   default.
2. For `line-height`, it is recommended to use unitless values, as it makes it based on the font size of the 
   root/browser, unless the element itself has a font size set. A good recommended value for `line-height` is `1.5`.

## React Basics
1. I reviewed components and composing them of other components.
2. I also looked at `className` for styling.
3. In addition, I looked at organizing components into separate files using `export` and `import`.
