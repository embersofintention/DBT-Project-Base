---
tags:
  - homework
  - indexes
tagline: DBT Skills Work Dashboard
publish: false
date:
created: 2025-11-22, 17:49
created_date: 2025 Saturday, November 22, 2025 5:49 PM
created_time: 17:49
---
.
```dataviewjs
// display the "tagline" YAML property as a header

let tagline = dv.current().tagline; 
if (tagline) {
	dv.header(1, tagline);
}


```
* [[_Daily notes dashboard v1]]
---



# Challenging Beliefs 
---
Start with a **distressing situation**, identify the **Belief** fueling the distress, and work through a process of **treating it with curiosity** 

> [!info] Add New Entry
> ```button
name ➕ challenge a new belief
type note(My New Note, tab) template
action Challenging Beliefs worksheet process
color default
folder DBT/-filled```

^button-AddChallengingBeliefs
```dataview

TABLE without id

	
	created AS "Created",
   
	"**Belief:** " + belief as "‹‹Belief Being Challenged›› :ᴹᵒʳᵉ:ᶜᵒⁿᵗᵉˣᵗ:ᵂᶦᵗʰᶦⁿ:ᵀʰᵃᵗ:ᴺᵒᵗᵉ:ᴸᶦⁿᵏ:_______",
	link(file.link) AS "⁰⁰⁰⁰⁰File⁰⁰⁰⁰⁰"
   
   
FROM
   #challenging-beliefs AND !#exclude AND !"_Templates"
   

WHERE 
   created_time != null
   

SORT 
   created DESC
   

```





# TRAP worksheet
---





.