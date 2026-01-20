1

```dataview
TABLE WITHOUT ID
   
  dateformat(file.ctime, "LLL dd, yy") as "★date",
   created_time AS "Time",
  
  
  blood-pressure as "blood pressure",
  pulse as "pulse rate",
  bp-context as "context",
  light-headed as "light headed?",
  dizzy as "dizzy?",
  file.link as "⁰⁰⁰⁰⁰link⁰⁰⁰⁰⁰"
  

  
FROM
  !#exclude 
  AND !"_Templates"
  
WHERE created != null 
 AND blood-pressure != null
 AND blood-pressure != " / "
 AND blood-pressure != " "

  


SORT created DESC

  
```
.


2
1

```dataview
TABLE
   
   dateformat(file.ctime, "LLL dd, yy") as "★date",
   created_time AS "Time",
   tags
  
  
  

  

FROM #homework 
SORT created DESC
LIMIT 10 
  
```

```dataview
TABLE WITHOUT ID





```


















.
















.