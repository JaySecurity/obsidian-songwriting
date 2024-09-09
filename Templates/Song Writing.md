<%*
	let folder = tp.file.folder()
	let title = tp.file.title
	if (title.startsWith("Untitled")){
		title = await tp.system.prompt("Title")
		await tp.file.rename(title)
		tp.file.title = title
	}
	if (folder != "Song Writing"){
		await tp.file.move("Song Writing/"+title)
	}
	tR += "---"
%>
working title: <%* tR += title %>
creation date: <% tp.file.creation_date() %>
tags: 
complete:
---
### Brain Dump / Map


### Hooks / Lines


## Melodies


`BUTTON[record-start]`


### Chord Progression / Melody
```chords
```


## Song Lyrics
