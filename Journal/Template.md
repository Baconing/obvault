# << <% tp.date.now("YYYY-MM-DD") %> >>
#### << [[<% tp.date.now("YYYY-MM-DD", -1) %>]] | [[<% tp.date.now("YYYY-MM-DD", 1) %>]] >>

---
### Accomplishments
#### Tasks completed
<% tp.file.cursor %>

#### Tasks intended to be completed.

---
### Reflection

---
### Statistics
#### Notes created today
```dataview
List FROM "" WHERE file.cday = date("<%tp.date.now("YYYY-MM-DD")%>") SORT file.ctime asc
```