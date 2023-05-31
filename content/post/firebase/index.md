---
title: "Firebase" # Title of the blog post.
date: 2023-05-31T16:04:23+04:00 # Date of post creation.
tags:
  - firebase
  - fullstack
# comment: false # Disable comment if false.
---

## Firebase Realtime Database
Yesterday I completed the newly added section on building a progressive web app that looks like a mobile app, using the 
core frontend trifecta, 
HTML, CSS, and JavaScript, hooked to a Firebase Realtime Database backend. Throughout the course I built a basic Add 
to Cart/todo list app. At the end I built the solo project **[We are the Champions](https://we-are-the-champions-shant.netlify.app/)**.  

The key strength of the Firebase Realtime Database is its `onValue` function, which enables your app to get a 
snapshot of the data, i.e. realtime READ, anytime something changes, whether it's a `push`, i.e. CREATE, `update`, or 
`remove`. The list 
of constants and functions I learned and used include:
1. `appSettings`, in which you include the `databaseURL`
2. `initialiseApp()`
3. `getDatabase()`
4. `ref()`
5. `push()`
6. `onValue()`
7. `remove()`
8. `update()`
9. `snapshot.exists()`
10. `snapshot.val()`
11. `Object.values()`
12. `Object.keys()`
13. `Object.entries()`
