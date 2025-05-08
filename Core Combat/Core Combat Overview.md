---
ContentDependencies:
  - "[[Core Foundations Overview|Core Foundations]]"
tags:
  - Overview
  - CoreCombat
aliases:
  - Core Combat
SectionEdition: 1.0.0
---
***Dependencies:*** `=this.ContentDependencies`
***Edition:*** `=this.SectionEdition`
***Description:***


Core Combat aims to implement combat through [[Weapon|Weapons]], [[Attack|Attacks]], and related [[Combat Actions]], though it doesn't actually implement the weapons themselves. It pairs well with the [[Core Items Overview|Core Items]] content section, but is not reliant on it.

***Content Pages:***
```dataview
TABLE WITHOUT ID Tags, map(rows, (r) => link(r.file.link, r.title)) AS Pages
FROM #CoreCombat 
FLATTEN file.tags as Tags 
SORT file.name ASC
GROUP BY Tags WHERE !startswith(Tags,"#CoreCombat")  AND !startswith(Tags, "#Overview")
```