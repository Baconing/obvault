
```dataviewjs
dv.span("**Tasks Completed**")
const calanderData = {
	entries: []
}

for (let page of dv.pages('"Journal/2024"').where(p => p.tasksCompleted)) {
	calanderData.entries.push({
		date: page.file.name,
		intensity: page.tasksCompleted,
	})
}

renderHeatmapCalendar(this.container, calanderData)
```
```dataviewjs
dv.span("**Tasks Left**")
const calanderData = {
	entries: []
}

for (let page of dv.pages('"Journal/2024"').where(p => p.tasksLeft)) {
	calanderData.entries.push({
		date: page.file.name,
		intensity: page.tasksLeft,
	})
}

renderHeatmapCalendar(this.container, calanderData)
```
```dataviewjs
dv.span("**Excercise**")
const calanderData = {
	entries: []
}

for (let page of dv.pages('"Journal/2024"').where(p => p.excercised)) {
	calanderData.entries.push({
		date: page.file.name,
		intensity: page.excercised,
	})
}

renderHeatmapCalendar(this.container, calanderData)
```
```dataviewjs
dv.span("**Tasks Left**")
const calanderData = {
	entries: []
}

for (let page of dv.pages('"Journal/2024"').where(p => p.tasksLeft)) {
	calanderData.entries.push({
		date: page.file.name,
		intensity: page.tasksLeft,
	})
}

renderHeatmapCalendar(this.container, calanderData)
```
