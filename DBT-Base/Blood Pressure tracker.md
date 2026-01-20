---
tags:
  - homework
  - blood-pressure
tagline: (empty)
publish: false
date:
---

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
WHERE 
  created_date != null 
  AND blood-pressure != null
  
SORT entry_time ASC
GROUP BY
  created_date
SORT key DESC

  
```



---



### 19:57 - speaking with on call person 




### 19:29 - info for on call provider 

* Surprised by situation: I've been far more healthy with my habits over the past five or so weeks, yet BP seems to have gotten significantly higher 
	* Been in RI hospital partial program trauma track

> [!question] **Chlorthalidone**, 12.5mg:  question for nurse
> Would it be safe / recommended to take an extra dose tonight and or tomorrow???
> * just started taking this for BP, 
> * took first dose this evening
> Ask when she calls back

 




---
