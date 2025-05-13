---
ContentDependencies:
  - "[[Core Magic Overview|Core Magic]]"
tags:
  - Overview
  - CoreSpells
SectionEdition: 1.0.0
---
***Dependencies:*** `=this.ContentDependencies`
***Edition:*** `=this.SectionEdition`
***Description:***

Implements basic magic spells.

***Content Pages:***
```dataview
TABLE WITHOUT ID Tags, map(rows, (r) => link(r.file.link, r.title)) AS Pages
FROM #CoreSpells  
FLATTEN file.tags as Tags
SORT file.name ASC
GROUP BY Tags WHERE !startswith(Tags,"#CoreSpells") AND !startswith(Tags, "#Overview")
```