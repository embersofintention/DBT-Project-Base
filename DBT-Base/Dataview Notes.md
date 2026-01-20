
To display a YAML property as a clickable link in a Dataview table, you can use the `link()` function in your query. For example, you can format your query like this: `TABLE link(yourProperty) AS "Your Link" FROM "yourFolder"` to create clickable links to the files associated with that property.  forum.obsidian.md](https://forum.obsidian.md/t/creating-links-from-dataview-table-results/65801)

---

A table to display frontmatter properties as a table in a note:  (to use, just copypaste the insides)

```

```dataviewjs
const frontmatter = Object.entries(dv.current().file.frontmatter).map((obj) => {
obj[0] = obj[0][0].toUpperCase() + obj[0].substr(1);
return obj;
}).filter(obj => obj[0] != "Tags");
dv.table(frontmatter.keys(), frontmatter);
```
```

```





s
BACKUP THINGs

```dataview

TABLE WITHOUT ID 
EmbededCoverImg as "Preview", 
link(file.name) + " | " + tagline as "About"




FROM "SketchPages" AND !"_Templates" AND !"index"
SORT date-sketched

WHERE file.name != this.file.name AND is_about
FLATTEN choice(typeof(img)="link",
    embed(link(meta(
        choice(
            typeof(img)="link",
                img, this.file.link
        )
    ).path, "250")), "![](" + img + ")") AS EmbededCoverImg

```



---



```dataview




```
