#### [[<% tp.date.now("YYYY-MM-DD", -1) %>]] | [[<% tp.date.now("YYYY-MM-DD", 1) %>]]

---
### Accomplishments
#### Tasks
- [ ] <% tp.file.cursor %>
---
### Reflection

---
### Statistics
#### Notes created today
```dataview
List FROM "" WHERE file.cday = date("<%tp.date.now("YYYY-MM-DD")%>") SORT file.ctime asc
```