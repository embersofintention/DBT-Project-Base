# Thing Name 
---
Add a **description** here, using bold and italics for emphasis. 


> [!info] Add New Entry
> ```button
name ➕ (use worksheet)
type note(My New Note, tab) template
action Add DC entry
color default
folder DBT/-filled```

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






---

---
---


Delete me



.