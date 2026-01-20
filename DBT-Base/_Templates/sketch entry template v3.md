---
tagline: (empty)
date-sketched: <% tp.file.creation_date("YYYY-MM-DD HH:mm") %>
tags:
  - sketches
is_about: general
publish: false
CW//: " "
---
```dataviewjs
// display the "tagline" YAML property as a header

let tagline = dv.current().tagline; 
if (tagline) {
	dv.header(1, tagline);
}


```


img:: pastehere



..