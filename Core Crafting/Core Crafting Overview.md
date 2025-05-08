---
ContentDependencies:
  - "[[Core Foundations Overview|Core Foundations]]"
  - "[[Core Items Overview|Core Items]]"
tags:
  - CoreCrafting
  - Overview
SectionEdition: 1.0.0
aliases:
  - Core Crafting
---
***Dependencies:*** `=this.ContentDependencies`
***Edition:*** `=this.SectionEdition`
***Description:***

This section introduces the rules for how [[Creature|Creatures]] may [[Crafting|Craft]] [[Item|Items]].


***Content Pages:***
```dataview
TABLE WITHOUT ID Tags, map(rows, (r) => link(r.file.link, r.title)) AS Pages
FROM #CoreCrafting 
FLATTEN file.tags as Tags 
SORT file.name ASC
GROUP BY Tags WHERE !startswith(Tags,"#CoreCrafting") AND !startswith(Tags, "#Overview")
```