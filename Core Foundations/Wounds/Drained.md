---
tags:
  - Wound
  - Entity
  - CoreFoundations
WoundSeverity: "0"
Source: "[[Core Foundations Overview|Core Foundations]]"
EntityValue: "0"
FoundationTraits:
  - "[[Wound]]"
MajorTraits:
  - "[[None]]"
MinorTraits:
  - "[[None]]"
cssclasses:
  - clean-embeds
EntityTags:
  - None
WoundTags:
  - Fatal
  - Attrition
---
***Value:*** `=this.EntityValue`
***Severity:*** `=this.WoundSeverity`
***Description:***

You are [[Dead]] from pure exhaustion. 

This wound is received automatically when a creature's maximum Body Endurance is reduced to 0, and is immediately removed if its maximum increases again. In this case, however, the creature remains dead.

***Tags:*** `=filter(unique(this.EntityTags + this.WoundTags),(x) => x!="None")`
***Source:*** `=this.Source`
### Traits

***Minor Traits:***
```dataviewjs
let current = dv.current()
let traits = current.MinorTraits
let embeds = traits.map(x => `****\n**${x}**\n!${x}`)

dv.span(embeds.join('\n'))
```
****

***Major Traits:***
```dataviewjs
let current = dv.current()
let traits = current.MajorTraits
let embeds = traits.map(x => `****\n**${x}**\n!${x}`)

dv.span(embeds.join('\n'))
```
****

***Foundation Traits:***
```dataviewjs
let current = dv.current()
let traits = current.FoundationTraits
let embeds = traits.map(x => `****\n**${x}**\n!${x}`)

dv.span(embeds.join('\n'))
```