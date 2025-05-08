---
tags:
  - Wound
  - Entity
  - CoreFoundations
WoundTypes:
  - Fatal
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
---
***Value:*** `=this.EntityValue`
***Severity:*** `=this.WoundSeverity`
***Description:***

A generic death. You are [[Dead]].

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