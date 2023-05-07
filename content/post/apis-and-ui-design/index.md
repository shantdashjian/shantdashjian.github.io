---
title: "APIs and UI Design" # Title of the blog post.
date: 2023-05-07T08:53:29+04:00 # Date of post creation.
tags:
  - api
  - ui design
  - chrome extension
# comment: false # Disable comment if false.
---

## APIs
Yesterday I completed Module 9: Working with APIs. The last section was about building a Chrome extension. The key 
element added to an otherwise regular JavaScript code to turn it into a Chrome extension is the **manifest.json** file. 
Here's an example of one:
<pre>
{
    "manifest_version": 3,
    "name": "Personal Dashboard",
    "version": "1.0.0",
    "description": "Just for practicing async JS",
    "action": {
        "default_icon": "icon.png"
    },
    "chrome_url_overrides": {
        "newtab": "index.html"
    }
}
</pre>


## UI Design
I kicked off Module 10: UI Design. The key learning from it so far is that UI design is based on 7 fundamentals, 
acronymed WACS-TCH:
1. **Whitespace**: Use padding, margin, line-height.
2. **Alignment**: Use text-align, flex-box justify-content and align-items.
3. **Contrast**: Use WCAG 2 extension to reach a min of 4.5:1 ratio between foreground font color and background color.
4. **Size or Scale**: Use font-size.
5. **Typography**: Use 1 or two fonts max.
6. **Color**: Use less colors, from a color palette.
7. **Visual Hierarchy**: Use all previous 6 fundamentals to display levels of importance, ensure titles and 
   call-to-action buttons are made important.
