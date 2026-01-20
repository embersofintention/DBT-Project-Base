







Edit this one:

```dataview
TABLE WITHOUT ID 

created_date as "ⁿⁿⁿⁿⁿDate⁰⁰⁰⁰⁰",
link(created_time, 
date(created_time)) AS "time",
  
contentment as "peace/ comfort",
sorrow-grieving as "sorrow/ grief",
guilt-shame as "guilt/ shame",
anger-resentment as "anger/ scorn",
anxiety-fear as "panic/ fear",
link(file.name) AS "⁶⁹⁴²⁰FileLink⁸⁰⁰⁸⁵"


  

  
FROM
  #diary-card AND!#exclude AND !"_Templates"

WHERE created_date != null 
SORT entry_time

FLATTEN created_date as "date"




```

---
dateformat(dateOfPurchase, "yyyy-LLL-dd")

```dataview 

TABLE without id

dateformat(created_date, "LLL dd, yyyy") as "Date",
link(created_time, date(created_time)) AS "Time of Entry",

   
   contentment AS "peace/ comfort",
   sorrow-grieving AS "sorrow/ grief",
   guilt-shame AS "guilt/ shame",
   anger-resentment AS "anger/ scorn",
   anxiety-fear AS "panic/ fear",
   link(file.link) AS "file name"
   
   


FROM
   #diary-card AND !#exclude AND !"_Templates"
WHERE 
   created_time != null
   
   

SORT
   created_date DESC, created_time DESC

```










__f
_



.