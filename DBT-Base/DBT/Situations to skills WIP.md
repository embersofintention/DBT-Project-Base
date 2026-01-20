---
tags:
  - homework
tagline: What skills fit which situations??
publish: false
date:
---

```dataviewjs
// display the "tagline" YAML property as a header

let tagline = dv.current().tagline; 
if (tagline) {
	dv.header(1, tagline);
}


```




---
