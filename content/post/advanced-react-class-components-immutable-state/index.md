---
title: "Advanced React: Class Components and Immutable State" # Title of the blog post.
date: 2023-05-27T06:36:30+04:00 # Date of post creation.
tags:
  - react
  - class components
  - immutable state
# comment: false # Disable comment if false.
---

## Class Components
Yesterday I completed the first section of the advanced React module. This went through using "old" React with class 
components as 
opposed to function components and hooks. It also went through "old" React lifecycle methods like `render`, 
`componentDidMount`, `componentDidUpdate`, and `componentWillUnmount` as opposed to using `useEffect`.

## Immutable State
The [React docs](https://react.dev/learn/updating-objects-in-state) recommend treating state as immutable, a 
snapshot, and only update it using `setState`. They say you 
probably could get away with it but shouldn't do it for a number of reasons that include easier debugging, 
compatability with future features, and performance. 
