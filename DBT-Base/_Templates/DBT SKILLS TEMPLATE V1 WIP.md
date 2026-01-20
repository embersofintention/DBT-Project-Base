---
tags:
  - dbt
  - type/Mindfulness
  - type/Emotion_Regulation
  - type/Distress_Tolerance
  - type/Interpersonal_Effectiveness
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


(( editing the outline directly ))



# **Skill Name**
---

## Slides
1. pdf
2. ​individual page images
3. Space for personal notes (after each page)
4. Any other related handouts



## Project Art
* Dataview Table: **Related Sketches (gallery)**
	* ?


## Worksheets --Try it out!

1. PDF copy
2. Button to use worksheet
	- creates new page in a sub folder
	- applies a **template** to the page: fillable version, formatted for obsidian

### (Filled sheets)

* Dataview table
	* date
	* tagline
	* link to file





# More Info
---

* articles
* videos
* misc
* 



---



---
**Edit template:**
```button
name Edit DBT template
type link
action obsidian://open?vault=Sketch-Journal&file=_Templates%2FDBT%20SKILLS%20TEMPLATE%20V1%20WIP
```
^button-1dfh
---
