---
tags:
  - Item
  - CoreItems
  - Object
ObjectValue: "0"
Source: "[[Core Items Overview|Core Items]]"
ItemSlot: None
ObjectSize: 1 meter
ObjectResistance: "20"
ObjectLuck: "20"
ObjectBody: "5"
EntityValue: "0"
ItemPrereqs:
  - None
FoundationTraits:
  - "[[Object]]"
MajorTraits:
  - "[[Item]]"
MinorTraits:
  - "[[None]]"
cssclasses:
  - clean-embeds
---
***Value:*** `=this.EntityValue`
***Slot:*** `=this.ItemSlot`
***Prerequisites:*** `=this.ItemPrereqs`
***Description:***

This clothing is standard, inexpensive, and would generally fit in wherever its owner is from.

***Size:*** `=this.ObjectSize`
***Resistance:*** `=this.ObjectResistance`
***Luck:*** `=this.ObjectLuck`
***Body:*** `=this.ObjectBody`

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