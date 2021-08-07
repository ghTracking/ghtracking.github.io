---
layout: default
categories: programming
---
- General note: the .yml file is key. This is where "site." variables are created. "site.pages" is a list of all pages which contain front matter.
Example of front matter:
```
---
layout: post
title: Title of this post!
---
```

- assign creates a new named variable. 

- One may also have a collection. If, such as in my example, I introduce a named collection in _config.yml as "A_Courses" and create a folder named "_A_Courses", these are accessed via "site.A_Courses".
- To add collection URLs, use the following in the config:
```
collections:
  A_Courses:
    output: true
    permalink: /A_Courses/:path/
```