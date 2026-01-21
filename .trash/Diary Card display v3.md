---
tags:
  - homework
  - diary-card
tagline: (empty)
publish: false
date:
---


# Diary Card Display


## Emotions (backing up working edits)
.
```dataview
TABLE WITHOUT ID 

created_date as "Date",


link(file.name) AS "File Link", 
(created_time) AS "time",
  
contentment as "peace/ comfort",
sorrow-grieving as "sorrow/ grief",
guilt-shame as "guilt/ shame",
anger-resentment as "anger/ scorn",
anxiety-fear as "panic/ fear"

  

  
FROM
  #diary-card AND!#exclude AND !"_Templates"
  
SORT entry_time



WHERE created_date != null 

```







---











## Struggles 
```dataview
TABLE 
   
  rows.created_time as "time",
  rows.intrusive-thoughts as "intrusive thoughts",
  rows.memory-lapses as "memory issues",
  rows.brain-explosions as "🧠💥",
  rows.all-or-nothing-thinking as "all or nothing thinking",
  
  rows.file.link as "Link"
  
  
FROM
  #diary-card AND!#exclude AND !"_Templates"
  
SORT entry_time ASC
GROUP BY
  created_date
SORT key DESC
WHERE created_date!= null

```
---

## Self Care (edit this)
```dataview
TABLE 

dateformat(created_date, "LLL dd, yyyy") as "Date",
link(created_time, date(created_time)) AS "Time of Entry",
   
  rows.created_time as "time",
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
  created_date
SORT key DESC
WHERE created_date!= null
  
```
---
## Context (see notes)
```dataview
TABLE WITHOUT ID
   
   created_date as "date",
  created_time as "time",
  file.link as "link (Full Context)",
  context as "short version blargharbleruargfgfgararararara"
  

  
  FROM
  #diary-card AND!#exclude AND !"_Templates"
  WHERE context != null
  
SORT entry_time ASC

  
```

## Blood Pressure Stuff
```dataview
TABLE 
   
  rows.created_time as "time",
  rows.blood-pressure as "blood pressure",
  rows.pulse as "pulse rate",
  rows.light-headed as "light headed?",
  rows.dizzy as "dizzy?",
  rows.file.link as "⁰⁰⁰⁰⁰⁰⁰⁰link⁰⁰⁰⁰⁰⁰⁰⁰"
  

  
FROM
  (#diary-card OR #blood-pressure) AND!#exclude AND !"_Templates"
WHERE created_date != null AND blood-pressure != null
  
SORT entry_time ASC
GROUP BY
  created_date
SORT key DESC

  
```
.