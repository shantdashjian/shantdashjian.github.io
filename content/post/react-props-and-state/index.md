---
title: "React Props and State" # Title of the blog post.
date: 2023-05-15T11:03:29+04:00 # Date of post creation.
tags:
  - react
  - props
  - state
# comment: false # Disable comment if false.
---

## React Props and State
Yesterday I explored the difference between props and state:
- **Props:** is data sent to the component from the outside, from a "parent" component, as config, as parameters, to 
  be used by the component but are immutable.
- **State:** is data that lives inside the component, as local variables, that are meant to be changed and displayed. 
  It's the data the React **reacts** to. As in, when that data changes, React will re-render that 
  component to reflect the changes in state. In a sense, React's reaction to state change is the core feature of 
  React as a framework. 
