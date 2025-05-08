---
ContentDependencies:
  - "[[Gauntlet Archetypes Overview|Gauntlet Archetypes]]"
  - "[[Core Combat Overview|Core Combat]]"
  - "[[Core Magic Overview|Core Magic]]"
  - "[[Fantasy Weaponry Overview|Fantasy Weaponry]]"
  - "[[Core Resting Overview|Core Resting]]"
tags:
  - Overview
  - MageArchetype
SectionEdition: 1.0.0
aliases:
  - Mage Archetype
---
***Dependencies:*** `=this.ContentDependencies`
***Edition:*** `=this.SectionEdition`
***Description:***

This content section introduces the mage: an archetype that focuses on versatile spellcasting and magical knowledge

***Content Pages:***
```dataview
TABLE WITHOUT ID Tags, map(rows, (r) => link(r.file.link, r.title)) AS Pages
FROM #MageArchetype  
FLATTEN file.tags as Tags
SORT file.name ASC
GROUP BY Tags WHERE !startswith(Tags,"#MageArchetype") AND !startswith(Tags, "#Overview")
```