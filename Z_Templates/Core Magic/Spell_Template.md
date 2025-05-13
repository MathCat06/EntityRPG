---
tags:
  - Entity
  - Spell
EntityValue: "0"
Source: None
FoundationTraits:
  - "[[Spell]]"
MajorTraits:
  - "[[None]]"
MinorTraits:
  - "[[None]]"
cssclasses:
  - clean-embeds
EntityTags:
  - None
SpellTags:
  - None
SpellPower: "1"
SpellVersatility: "1"
SpellCastingTime: 1 Action
---
***Value:*** `=this.EntityValue`
***Power:*** `=this.SpellPower`
***Versatility:*** `=this.SpellVersatility`
***Casting Time:*** `=this.SpellCastingTime`
***Description:***



***Tags:*** `=filter(unique(this.EntityTags + this.SpellTags),(x) => x!="None")`
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