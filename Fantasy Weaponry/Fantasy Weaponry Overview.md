---
ContentDependencies:
  - "[[Core Items Overview|Core Items]]"
  - "[[Core Adventure Overview|Core Adventure]]"
  - "[[Core Combat Overview|Core Combat]]"
tags:
  - Overview
  - "#FantasyWeaponry"
SectionEdition: 1.0.0
aliases:
  - Fantasy Weaponry
---
***Dependencies:*** `=this.ContentDependencies`
***Edition:*** `=this.SectionEdition`
***Description:***

This Content Section adds weapons and armor commonly seen in fantasy genres, as well as common traits used for them. Note that for balancing purposes, after the first, each 4 additional points of [[Damage]] per attack on average is worth 1 value.

***Content Pages:***
```dataview
TABLE WITHOUT ID Tags, map(rows, (r) => link(r.file.link, r.title)) AS Pages
FROM #FantasyWeaponry  
FLATTEN file.tags as Tags
SORT file.name ASC
GROUP BY Tags WHERE !startswith(Tags,"#FantasyWeaponry") AND !startswith(Tags, "#Overview") AND !startswith(Tags,"#Object")
```