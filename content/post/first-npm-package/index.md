---
title: "First NPM Package" # Title of the blog post.
date: 2023-07-03T05:59:16+04:00 # Date of post creation.
tags:
  - npm
  - project
  - armenian-names
# comment: false # Disable comment if false.
---

Yesterday I developed and published my first NPM package, the [armenian-names package](https://www.npmjs.com/package/armenian-names).
This package provides the following useful functions:
<pre>
getMaleNames()
getFemaleNames()
getAllNames()
getRandomMaleName()
getRandomFemaleName()
getRandomName()
</pre>

### Who Would Benefit from `armenian-names`?
People developing applications that need to incorporate Armenian given names, whether boy or girl names, as part of 
their data can 
benefit 
from 
importing this package into their project.

### Why I Built It
1. I wanted to build something fun that I'm interested in. I'm ethnically Armenian and preserving my ethnic identity 
   is something I value. I also find picking names for babies to be a fun thing to do.
2. I wanted to learn a new technology. Learning how to build and publish an NPM package was always something I 
   had in the back burner and finally got to do.
3. I wanted to add something to the incredibly vast universe of resources available for developers that is the 
   Internet. This is one contribution I made, giving back to this mind-blowing ecosystem. 
4. This is a project I could showcase in a future job interview or technical talk. 

### What I Learned
1. Building an NPM package is a very easy process. The steps are:
   1. `mkdir <your-npm-package-name>`.
   2. `cd <your-npm-package-name>`.
   3. `git init`.
   4. `npm init`.
   5. Create an `index.js`. 
   6. In `index.js`, you provide data and export function(s) to make that data available to the end user in someway(s).
   7. `npm link` to make it globally available on your machine for testing.
   8. Create another project to test it.
   9. `npm link <your-npm-package-name>` to add it as a dependency and use it in that test project.
   10. When ready, `npm login` and then `npm publish`.
2. There are currently **2,459,633** packages on [npm](https://www.npmjs.com/). My [armenian-names package](https://www.npmjs.com/package/armenian-names) is one of those **2,459,633** packages.
