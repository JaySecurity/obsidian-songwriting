<%*
	let folder = tp.file.folder()
	let title = tp.file.title
	if (title.startsWith("Untitled")){
		title = await tp.system.prompt("Title")
		await tp.file.rename(title)
		tp.file.title = title
	}
	let artist = await tp.system.prompt("Artist")
	await tp.file.move("Music/"+artist+"/"+title)
	tR += "---"
%>
artist:  <% artist %>
title:  <% title %>
creation date: <% tp.file.creation_date() %>
tags: 
complete:
---

## Song

```chords


```