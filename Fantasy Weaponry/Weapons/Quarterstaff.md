---
tags:
  - Object
  - Item
  - Weapon
  - FantasyWeaponry
EntityValue: "1"
Source: "[[Fantasy Weaponry Overview|Fantasy Weaponry]]"
ObjectSize: 1 meter
ObjectResistance: "20"
ObjectLuck: "20"
ObjectBody: "5"
FoundationTraits:
  - "[[Object]]"
MajorTraits:
  - "[[Weapon]]"
  - "[[Item]]"
MinorTraits:
  - "[[Steadied]]"
WeaponReach: 1 meter
WeaponScore: Strength
WeaponDamage: 1d4+2 impact damage
ItemSlot: Hand
ItemPrereqs:
  - None
cssclasses:
  - clean-embeds
---
***Value:*** `=this.EntityValue`
***Reach:*** `=this.WeaponReach`
***Score:*** `=this.WeaponScore`
***Damage:*** `=this.WeaponDamage`
***Slot:*** `=this.ItemSlot`
***Prerequisites:*** `=this.ItemPrereqs`
***Description:***

The quarterstaff, while not flashy, is just as good for walking as it is for combat.

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