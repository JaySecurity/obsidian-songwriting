<%*
	let folder = tp.file.folder()
	let title = tp.file.title
	if (folder != "Daily/"){
		await tp.file.move("Daily/"+title)
	}
	tR += "---"
%>
creation date: <% tp.file.creation_date() %>
tags:
Mood:
---
# Habit Tracking

- [ ] Meditation
- [ ] Workout
- [ ] Walk Dog

# Thoughts






