---
publish: false
cssclasses:
date:
is_about:
  - Diary-card
  - Collection
---



# Diary Card Display


## Emotions 
```dataview
TABLE
   
  rows.entry_time as "time",
  rows.contentment as "peace/ comfort",
  rows.sorrow-grieving as "sorrow/ grief",
  rows.guilt-shame as "guilt/ shame",
  rows.anger-resentment as "anger/ scorn",
  rows.anxiety-fear as "panic/ fear",
  rows.file.link as "Link"
  

  
FROM
  #diary-card AND!#exclude AND !"_Templates"
  
SORT entry_time ASC
GROUP BY
  entry_date
SORT key DESC
LIMIT 5

```
---

## Struggles 
```dataview
TABLE 
   
  rows.entry_time as "time",
  rows.intrusive-thoughts as "intrusive thoughts",
  rows.memory-lapses as "memory issues",
  rows.brain-explosions as "🧠💥",
  rows.all-or-nothing-thinking as "all or nothing thinking",
  
  rows.file.link as "Link"
  
  
FROM
  #diary-card AND!#exclude AND !"_Templates"
  
SORT entry_time ASC
GROUP BY
  entry_date
SORT key DESC

```
---

## Self Care
```dataview
TABLE 
   
  rows.entry_time as "time",
  rows.breakfast as "breakfast",
  rows.lunch as "lunch",
  rows.dinner as "dinner",
  rows.cups-of-water as "🥤",
  rows.moist-chamber as "moist chamber",
  rows.file.link as "Link"
  
  FROM
  #diary-card AND!#exclude AND !"_Templates"
  
SORT entry_time ASC
GROUP BY
  entry_date
SORT key DESC
  
```
---
## Context
```dataview
TABLE 
   
  rows.entry_time as "time",
  rows.context as "context blargharbleruargfgfgararararara",
  
  rows.file.link as "Link"
  
  FROM
  #diary-card AND!#exclude AND !"_Templates"
  WHERE context != null
  
SORT entry_time ASC
GROUP BY
  entry_date
SORT key DESC
  
```








---

# Key

### Emotions
- contentment::
- sorrow-grieving::
- guilt-shame::
- anger-resentment::
- anxiety-fear::
### Struggles
- intrusive-thoughts::
- memory-lapses::
- brain-explosions::
- all-or-nothing-thinking::
### Habits
(yes or no)
* get-outside::
* moist-chamber::
#### Meals
* breakfast::
* lunch::
* dinner::
* cups-of-water::






# BACKUP




---
# Thought Entries 
```dataview

TABLE WITHOUT ID EmbededCoverImg as "Preview", link(file.link) + " (" + date + ")" as "Link"
FROM "DBT" AND !"_Templates" AND !"index"
SORT date-sketched, ASC

WHERE file.name != this.file.name AND publish = true
FLATTEN choice(typeof(img)="link",
    embed(link(meta(
        choice(
            typeof(img)="link",
                img, this.file.link
        )
    ).path, "250")), "![](" + img + ")") AS EmbededCoverImg


```



---






.