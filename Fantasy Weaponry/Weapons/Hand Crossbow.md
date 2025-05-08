---
tags:
  - Object
  - Item
  - Weapon
  - FantasyWeaponry
EntityValue: "0"
Source: "[[Fantasy Weaponry Overview|Fantasy Weaponry]]"
ObjectSize: .5 meter
ObjectResistance: "20"
ObjectLuck: "20"
ObjectBody: "5"
FoundationTraits:
  - "[[Object]]"
MajorTraits:
  - "[[Weapon]]"
  - "[[Item]]"
MinorTraits:
  - "[[Ammunition]]"
  - "[[Dual Wield]]"
  - "[[Reset]]"
  - "[[Ranged]]"
WeaponReach: 25 meters
WeaponScore: Focus
WeaponDamage: 1d6+2 pierce damage
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

A hand-held crossbow, capable of long range attacks for even the most inexperienced individual.

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