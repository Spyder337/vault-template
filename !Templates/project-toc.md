---
created: <% tp.file.creation_date("DD-MM-YYYY") %>
modified: <% tp.file.last_modified_date("DD-MM-YYYY HH:mm") %>
title: <% tp.file.title %>
tags:
  - projects
  - project/<%
  - tp.file.title
  - "%>"
project: "[[<% tp.file.title %>]]"
project_type: Programming
active: "false"
git: '""'
---
# <% tp.file.title %>
## Why?
What does the project aim to address or what is it's primary reason to exist.
# How?
How will the project be implemented or what are the steps to complete the project.
## Notes
```dataview
LIST
FROM #project/<% tp.file.title %>
WHERE title != "<%tp.file.title%>"
SORT created
```
# Resources
Sources used in order to plan the project. Also any research materials go here, such as, blog posts, YouTube videos, etc.
