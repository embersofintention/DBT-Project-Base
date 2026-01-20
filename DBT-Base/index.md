---
cssclasses:
  - hide-title
  - cards
publish: true
sticker: emoji//2660-fe0f
---
(Last updated:  `$=dv.current().file.mtime`)

Click an image below to enlarge, or subject link to view its post (some may have thoughts included)

## ✏️
I gotta add the rest of the sketch pages ok but enjoy these for now yay



# The Visual Metaphors Used 
The concepts and ideas that are used throughout these pages to visually depict much of this overall mental process.

```dataview

TABLE WITHOUT ID 
EmbededCoverImg as "Thumbnail", 
link(file.name) + " | " + tagline as "About"



//do not include templates or index page in results
FROM !"_Templates" AND !"index" 
SORT file.name ASC

WHERE file.name != this.file.name 
	AND contains(is_about, "Characterizing-Concepts")
	AND publish = true


FLATTEN choice(typeof(img)="link",
    embed(link(meta(
        choice(
            typeof(img)="link",
                img, this.file.link
        )
    ).path, "200")), "![](" + img + ")") AS EmbededCoverImg

LIMIT 10

```




# All Sketch Pages....

```dataview

TABLE WITHOUT ID 
EmbededCoverImg as "Preview", 
link(file.name) as "Date",
tagline as "Tagline",
tags as "Touches on..."




FROM "SketchPages" AND !"_Templates" AND !"index" AND !#exclude
SORT date-sketched ASC

FLATTEN choice(typeof(img)="link",
    embed(link(meta(
        choice(
            typeof(img)="link",
                img, this.file.link
        )
    ).path, "100")), "![](" + img + ")") AS EmbededCoverImg



```





![[Pasted image 20251004171414.png]]


---
## Other fun links...
* Coming soon


---
