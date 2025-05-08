---
ContentDependencies:
  - "[[Core Foundations Overview|Core Foundations]]"
tags:
  - Overview
  - CoreResting
SectionEdition: 1.0.0
aliases:
  - Core Resting
---
***Dependencies:*** `=this.ContentDependencies`
***Edition:*** `=this.SectionEdition`
***Description:***

Core Resting aims to implement a system of [[Rest]] and recovery for both [[Wounds]] and a [[Creature]]'s loss of Body and Break Endurance.

***Content Pages:***
```dataview
TABLE WITHOUT ID Tags, map(rows, (r) => link(r.file.link, r.title)) AS Pages
FROM #CoreResting 
FLATTEN file.tags as Tags
SORT file.name ASC
GROUP BY Tags WHERE !startswith(Tags,"#CoreResting") AND !startswith(Tags, "#Overview")
```