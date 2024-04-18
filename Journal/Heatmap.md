
```dataviewjs
dv.span("**Tasks**")
const calanderData = {
	entries: []
}

for (let page of dv.pages('"Journal/2024"')) {
	let tasksCompleted = page.file.tasks.length 
	let totalTasks = page.file.tasks.length

	calanderData.entries.push({
		date: page.file.name,
		intensity: tasksCompleted/totalTasks,
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
