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
