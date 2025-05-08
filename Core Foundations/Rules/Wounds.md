---
aliases:
  - Wound
tags:
  - Rules
  - CoreFoundations
Source: "[[Core Foundations Overview|Core Foundations]]"
---
When a Creature's Body endurance is reduced to 0, they take a Wound. The creature makes a Luck Tier Check, subtracting a -10 modifier from it for each wound they already have. Depending on how brutal you desire your game to be, you may add a modifier to this as well: a flat +20 means that the third wound a creature takes has a 50% chance of fatality, and the first almost certainly will not. They then take a wound with severity rank greater then their result at the GM's discretion (Greater severity ranks are less severe, and usually the most severe wound possible should be chosen). A wound must always be selected, however minor, unless specifically negated by another effect.

Wounds have a number of different types, usually corresponding to what they are caused by, as well a severity rank and a description. Fatality is a special wound type; if this is included, then the wound results in Creature [[Death]], usually also mentioned in the wound's description.

```dataview
LIST FROM #Wound WHERE file.name !="Wound_Template" SORT woundseverity ASC
```

***Source:*** `=this.Source`