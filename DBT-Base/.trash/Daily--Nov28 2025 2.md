---
tags:
  - daily-notes
  - diary-card
  - homework
tagline: (empty)
publish: false
date:
created: 2025-11-28,  12:35
created_time: 12:35
created_date: 2025-11-28
---
.

# `=this.created_date`


---
# Seed Thoughts 🫘
---
Any stray, seemingly unimportant little thought could carry the potential to wind up growing into something so much more.  All thoughts deserve to have a place to go.
* .


---
# Intention 🌱
---

## Main Goals
*(A small, manageable list of things that I can plan out and make actionable)*

* .



---
# Reflection 🍁
---
## Pleasant Moments 
*(A place to reflect on nice things that happened)*
* .

## What went *well*?
* .

## What *didn't* go well?
*and what could I do differently next time?* 
* .

## What am I *proud* of?
* .

## What did I *learn*? 
* .



---

# Diary Card Entries of Today

```button
name 👍🏾Create New Diary Card Entry
type note(My New Note, tab) template
action Diary Card Template v4
color default
folder DBT/Diary Cards
```
^button-Add_DC

```dataview

TABLE without id

dateformat(created_date, "LLL dd, yy") as "date",
   created_time AS "Time",
   
   

   emotion-mind as "ₑₘₒₜᵢₒₙ Mɪɴᴅ",
   rational-mind as "Logic Mind",
   wise-mind as "Wise Mind",
   dissociation as "ᴰᶦˢˢᵒᶜᶦᵃᵗᶦᵒⁿ ⁽⁰⁻¹⁰⁰⁾",
   focus as "Focus",
   scattered-thoughts as "ˢᶜᵃᵗᵗᵉʳᵉᵈ ᵀʰᵒᵘᵍʰᵗˢ",
   
   
   link(file.link) AS "★⁰⁰⁰⁰File⁰⁰⁰⁰★",
      dc-context as "‹‹CONTEXT›› ᴹᵒʳᵉ:ᶜᵒⁿᵗᵉˣᵗ:ᵂᶦᵗʰᶦⁿ:ᵀʰᵃᵗ:ᴺᵒᵗᵉ:ᴸᶦⁿᵏ:;:;:;:;:;:;:;:!:!:;:;;:;::::::::::::::::::"
   
   
FROM
   #diary-card AND !#exclude AND !"_Templates"
   

WHERE 
   file.created_date = this.file.created_date


SORT 
   created DESC
   

```










.
```dataviewjs
// display the "tagline" YAML property as a header

let tagline = dv.current().tagline; 
if (tagline) {
	dv.header(1, tagline);
}


```




---
