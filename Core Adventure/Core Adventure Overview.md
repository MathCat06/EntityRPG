---
ContentDependencies:
  - "[[Core Foundations Overview|Core Foundations]]"
tags:
  - Overview
  - CoreAdventure
SectionEdition: 1.0.0
aliases:
  - Core Adventure
---
***Dependencies:*** `=this.ContentDependencies`
***Edition:*** `=this.SectionEdition`
***Description:***

This Content Section aims to establish a system of play most similar to Dungeons and Dragons, Pathfinder, and other games of exploration and combat through the use of adventure-relevant attributes and miscellaneous rules. It includes mostly setting neutral attributes as a foundation for most games in any genre. The recommended set of additional sections for a game like this would be [[Core Combat Overview|Core Combat]], [[Core Items Overview|Core Items]], [[Core Resting Overview|Core Resting]] and [[Core Crafting Overview|Core Crafting]]. For further expansion, this list doesn't have any Knowledge Attributes, which are more setting specific.

***Content Pages:***
```dataview
TABLE WITHOUT ID Tags, map(rows, (r) => link(r.file.link, r.title)) AS Pages
FROM #CoreAdventure  
FLATTEN file.tags as Tags
SORT file.name ASC
GROUP BY Tags WHERE !startswith(Tags,"#CoreAdventure") AND !startswith(Tags, "#Overview")
```