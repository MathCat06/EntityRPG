---
tags:
  - Item
  - Object
  - FantasyWeaponry
EntityValue: "1"
Source: "[[Fantasy Weaponry Overview|Fantasy Weaponry]]"
ItemSlot: Torso
ItemPrereqs:
  - Strength less than 15
ObjectSize: 1 meter
ObjectResistance: "10"
ObjectLuck: "20"
ObjectBody: "10"
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

Gain a -5 [[Defense Modifiers|Defense Modifier]] to all attacks against you.

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