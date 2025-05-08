---
ContentDependencies:
  - "[[Core Foundations Overview|Core Foundations]]"
tags:
  - Overview
  - CoreItems
aliases:
  - Core Items
SectionEdition: 1.0.0
---
***Dependencies:*** `=this.ContentDependencies`
***Edition:*** `=this.SectionEdition`
***Description:***

Core Items implements wearable and carriable [[Item]] Objects for [[Creature|Creatures]] to use. In addition, it adds a relatively basic inventory system. See the [[Using Items]] page for the basics of this section. These pair well with weapons from the [[Core Combat Overview|Core Combat]] section. 


***Content Pages:***
```dataview
TABLE WITHOUT ID Tags, map(rows, (r) => link(r.file.link, r.title)) AS Pages
FROM #CoreItems 
FLATTEN file.tags as Tags 
SORT file.name ASC
GROUP BY Tags WHERE !startswith(Tags,"#CoreItems")  AND !startswith(Tags, "#Overview")
```