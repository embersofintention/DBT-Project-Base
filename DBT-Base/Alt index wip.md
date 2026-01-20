








```dataview
table without id 
	embed(link(meta(sketch).path)) as "sketch",
	date as "date",
	topic as Title
where sketch!= null
```

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
    ).path, "100")), "![](" + img + ")") AS EmbededCoverImg


```



.