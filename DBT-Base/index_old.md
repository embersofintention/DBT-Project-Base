---
publish: false
cssclasses:
---

# ✏️🖍️hi✒️🖍️
Click an image below to view, or just hover over it to preview the page.  

(Content posted and managed directly from my phone. Pretty handy!)



```dataview

TABLE WITHOUT ID EmbededCoverImg as "Sketch", link(file.link) + " (" + date + ")" as "subject"
FROM #sketches AND !"_Templates"

WHERE file.name != this.file.name
FLATTEN choice(typeof(img)="link",
    embed(link(meta(
        choice(
            typeof(img)="link",
                img, this.file.link
        )
    ).path, "250")), "![](" + img + ")") AS EmbededCoverImg


```







---





---
```dataview

TABLE WITHOUT ID EmbededCoverImg as "Sketch", link(file.link) as "Thing", Today as "Date"
FROM #journal AND !"_Templates"

WHERE file.name != this.file.name
FLATTEN choice(typeof(img)="link",
    embed(link(meta(
        choice(
            typeof(img)="link",
                img, this.file.link
        )
    ).path, "50")), "![](" + img + ")") AS EmbededCoverImg


```



---
