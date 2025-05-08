---
ContentDependencies:
  - "[[Core Adventure Overview|Core Adventure]]"
tags:
  - Overview
  - GauntletArchetypes
SectionEdition: 1.0.0
aliases:
  - Gauntlet Archetypes
---
***Dependencies:*** `=this.ContentDependencies`
***Edition:*** `=this.SectionEdition`
***Description:***

This content section aims to add [[Gauntlet Character Creation]], [[Gauntlet Progression]], and [[Archetype Traits]] to a Foundations Ruleset. It does not actually implement the Traits, only the framework for how they are used. 

***Content Pages:***
```dataview
TABLE WITHOUT ID Tags, map(rows, (r) => link(r.file.link, r.title)) AS Pages
FROM #GauntletArchetypes 
FLATTEN file.tags as Tags
SORT file.name ASC
GROUP BY Tags WHERE !startswith(Tags,"#GauntletArchetypes") AND !startswith(Tags, "#Overview")
```