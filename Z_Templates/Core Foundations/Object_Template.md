---
tags:
  - Object
  - Entity
EntityValue: "0"
Source: None
ObjectSize: 1 meter
ObjectResistance: "20"
ObjectLuck: "20"
ObjectBody: "5"
FoundationTraits:
  - "[[Object]]"
MajorTraits:
  - "[[None]]"
MinorTraits:
  - "[[None]]"
cssclasses:
  - clean-embeds
EntityTags:
  - None
---
***Value:*** `=this.EntityValue`
***Description:***



***Size:*** `=this.ObjectSize`
***Resistance:*** `=this.ObjectResistance`
***Luck:*** `=this.ObjectLuck`
***Body:*** `=this.ObjectBody`

***Tags:*** `=this.EntityTags`
***Source:*** `=this.Source`

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