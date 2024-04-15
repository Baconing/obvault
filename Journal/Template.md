---
tasksCompleted: 1
tasksLeft: 1
excercised: 
intended: true
---
<% moment(tp.file.title,'YYYY-MM-DD').format("dddd, MMMM DD, YYYY") %>
<< [[<% fileDate = moment(tp.file.title, 'YYYY-MM-DD-dddd').subtract(1, 'd').format('YYYY-MM-DD-dddd') %>|Yesterday]] | [[<% fileDate = moment(tp.file.title, 'YYYY-MM-DD-dddd').add(1, 'd').format('YYYY-MM-DD-dddd') %>|Tomorrow]] >>
#### Tasks Completed
- 

#### Tasks Uncompleted
- 

#### Reflection