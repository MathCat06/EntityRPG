---
ContentDependencies:
  - "[[Gauntlet Archetypes Overview|Gauntlet Archetypes]]"
  - "[[Core Combat Overview|Core Combat]]"
  - "[[Fantasy Weaponry Overview|Fantasy Weaponry]]"
tags:
  - Overview
  - RogueArchetype
SectionEdition: 1.0.0
aliases:
  - Rogue Archetype
---
***Dependencies:*** `=this.ContentDependencies`
***Edition:*** `=this.SectionEdition`
***Description:***

This content section introduces the rogue: an archetype that focuses on mobility and a varies set of skills.

***Content Pages:***
```dataview
TABLE WITHOUT ID Tags, map(rows, (r) => link(r.file.link, r.title)) AS Pages
FROM #RogueArchetype  
FLATTEN file.tags as Tags
SORT file.name ASC
GROUP BY Tags WHERE !startswith(Tags,"#RogueArchetype") AND !startswith(Tags, "#Overview")
```