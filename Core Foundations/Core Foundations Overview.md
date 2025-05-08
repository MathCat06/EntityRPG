---
ContentDependencies:
  - "[[(START HERE) Entity Overview|Entity General Rules]]"
  - None
tags:
  - Overview
  - CoreFoundations
aliases:
  - Core Foundations
SectionEdition: 1.0.0
---
***Dependencies:*** `=this.ContentDependencies`
***Edition:*** `=this.SectionEdition`
***Description:***

This content section provides basic information on the [[Foundation Traits]] used in the Foundations ruleset. These are intended to provide a balanced set of traits for almost any type of game, as well as the basics of how to create player characters. In addition to adding [[Creature|Creatures]] and [[Object|Objects]], this ruleset implements a [[Turn Order]] system as well as a [[Damage]] and [[Targeting]] system. Finally, it implements core [[Minor Traits]] for balancing Creatures and Objects.

***Content Pages:***
```dataview
TABLE WITHOUT ID Tags, map(rows, (r) => link(r.file.link, r.title)) AS Pages
FROM #CoreFoundations 
FLATTEN file.tags as Tags 
SORT file.name ASC
GROUP BY Tags WHERE !startswith(Tags,"#CoreFoundations") AND !startswith(Tags, "#Overview")
```