---
created: <% tp.file.creation_date("DD-MM-YYYY") %>
modified: <% tp.file.last_modified_date("DD-MM-YYYY HH:mm") %>
title: <% tp.date.now("MMMM-DD-YYYY") %>
tags: [ "daily_note" ]
---
# <% tp.date.now("dddd - MMMM, DD, YYYY") %>
<< [[Daily Notes/<% tp.date.now("YYYY", -1)%>/<% tp.date.now("MM-MMMM", -1) %>/<% tp.date.now("DD", -1) %> |Previous]] | [[Daily Notes/<% tp.date.now("YYYY", 1)%>/<% tp.date.now("MM-MMMM", 1) %>/<% tp.date.now("DD", 1) %>|Next]] >>

# Notes Created
```dataview
List FROM "" WHERE created = date("<% tp.date.now("DD-MM-YYYY") %>") SORT file.mtime asc 
```
