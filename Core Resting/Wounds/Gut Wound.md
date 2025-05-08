---
tags:
  - Wound
  - Entity
  - CoreResting
WoundSeverity: "20"
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
  - Pierce
  - Slash
---
***Value:*** `=this.EntityValue`
***Severity:*** `=this.WoundSeverity`
***Description:***

You have [[Disadvantage]] on all rolls you make during [[Rest Period|Rest Periods]].

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