---
tags:
  - homework
tagline: (empty)
publish: false
date:
created: <% tp.file.creation_date("YYYY-MM-DD, HH:mm") %>
created_date: <% tp.file.creation_date("YYYY LLLL") %>
created_time: <% tp.file.creation_date("HH:mm") %>
---

```dataviewjs
// display the "tagline" YAML property as a header

let tagline = dv.current().tagline; 
if (tagline) {
	dv.header(1, tagline);
}


```







---
# Planning template out...

Things needed:
* header: name of skill
* slides
	1. pdf
	2. ​individual page images
	3. Space for personal notes (after each page)
* handouts
* worksheets
	1. PDF
	2. Button to use worksheet
		- creates new page in a sub folder
		- applies a **template** to the page: fillable version, formatted for obsidian
* Dataview table: **filled worksheets**
	* date
	* tagline
	* link to file

* Dataview Table: **Related Sketches (gallery)**
	* ?





---
