---
title: "React Reusability and Performance" # Title of the blog post.
date: 2023-05-29T05:45:38+04:00 # Date of post creation.
tags:
  - react
  - reusability
  - performance
# comment: false # Disable comment if false.
---

## React Reusability
In order to DRY, 4 design patterns have emerged in React:
1. Components with props
2. Children
3. Higher Order Components
4. Render props

## React Performance
In order to prevent React from rendering the entire tree when a branch doesn't have its props and state changed, 
React has 3 ways:
1. `shouldComponentUpdate()`: The oldest, replaced by `PureComponent`
2. `PureComponent`: For class components
3. `memo()`: for functional components

*Avoid premature optimization*.
