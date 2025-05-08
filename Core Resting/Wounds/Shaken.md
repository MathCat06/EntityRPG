---
tags:
  - Wound
  - Entity
  - CoreResting
WoundSeverity: "30"
Source: "[[Core Resting Overview|Core Resting]]"
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
  - Temporary
  - Attrition
---
***Value:*** `=this.EntityValue`
***Severity:*** `=this.WoundSeverity`
***Description:***

While you take a [[Refresh]], you have a -10 modifier to your Resistance [[Check|Checks]].

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