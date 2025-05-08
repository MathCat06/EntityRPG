---
tags:
  - Overview
  - "#GeneralRules"
ContentDependencies:
  - None
SectionEdition: 1.0.0
aliases:
  - Entity Overview
---
***Dependencies:*** `=this.ContentDependencies`
***Edition:*** `=this.SectionEdition`
***Description:***

EntityRPG  is intended to be a flexible, in depth, mechanically rich, expandable RPG system. The intention is to easily be able to expand and use almost any mechanic you want, for any setting you want. The core rules are more of a suggestion, and should be adjusted if balance is off. As such, the rules are broken into [[Content Sections]], each of which will have an overview like this one. These are what will determine the exact nature of your game.

Outlined in this section is the main framework of play; how players interact with a world and the basic building blocks of how Entity represents that world.

To get started, see [[Entities]] to begin looking through the detailed contents of the game, or [[How to Play]] for the basics of how to resolve a story.


***Content Pages:***
```dataview
TABLE WITHOUT ID Tags, map(rows, (r) => link(r.file.link, r.title)) AS Pages
FROM #GeneralRules
FLATTEN file.tags as Tags 
SORT file.name ASC
GROUP BY Tags WHERE !startswith(Tags,"#GeneralRules")  AND !startswith(Tags, "#Overview")
```