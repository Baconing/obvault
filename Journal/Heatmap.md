```dataviewjs
dv.span("**Tasks Completed**")
const calanderData = {
	entries: []
}

for (let page of dv.pages('Journal/2024').where(p => p.tasksCompleted)) {
	calanderData.entries.push({
		date: page.file.name,
		intensity: page.tasksCompleted,
	})
}

renderHeatmapCalendar(this.container, calanderData)
```
