---
ContentDependencies:
  - "[[Gauntlet Archetypes Overview|Gauntlet Archetypes]]"
  - "[[Core Combat Overview|Core Combat]]"
  - "[[Fantasy Weaponry Overview|Fantasy Weaponry]]"
tags:
  - Overview
  - ChampionArchetype
SectionEdition: 1.0.0
aliases:
  - Champion Archetype
---
***Dependencies:*** `=this.ContentDependencies`
***Edition:*** `=this.SectionEdition`
***Description:***

This content section introduces the champion: an archetype that focuses on powerful offense and defense. 

***Content Pages:***
```dataview
TABLE WITHOUT ID Tags, map(rows, (r) => link(r.file.link, r.title)) AS Pages
FROM #ChampionArchetype   
FLATTEN file.tags as Tags
SORT file.name ASC
GROUP BY Tags WHERE !startswith(Tags,"#ChampionArchetype") AND !startswith(Tags, "#Overview")
```