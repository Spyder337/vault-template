---
created: <% tp.file.creation_date("DD-MM-YYYY") %>
modified: <% tp.file.last_modified_date("DD-MM-YYYY HH:mm") %>
title: <% tp.file.folder() %>/<% tp.file.title %>
tags:
  - projects
  - project/<% tp.file.folder() %>
project: "[[<% tp.file.folder() %>]]"
---
# <% tp.file.title %>
<% tp.file.cursor(1) %>