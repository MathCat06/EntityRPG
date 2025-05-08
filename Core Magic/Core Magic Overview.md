---
ContentDependencies:
  - "[[Core Foundations Overview|Core Foundations]]"
tags:
  - Overview
  - CoreMagic
SectionEdition: 1.0.0
aliases:
  - Core Magic
---
***Dependencies:*** `=this.ContentDependencies`
***Edition:*** `=this.SectionEdition`
***Description:***

Core Magic Implements a system for magic and spells for [[Creature|Creatures]] to use. In addition to specific spells, it implements various magic-related rules, like concentration and arcane knowledge.

***Content Pages:***
```dataview
TABLE WITHOUT ID Tags, map(rows, (r) => link(r.file.link, r.title)) AS Pages
FROM #CoreMagic 
FLATTEN file.tags as Tags
SORT file.name ASC
GROUP BY Tags WHERE !startswith(Tags,"#CoreMagic") AND !startswith(Tags, "#Overview")
```