---
tags:
  - Object
  - Item
  - Weapon
  - FantasyWeaponry
EntityValue: "4"
Source: "[[Fantasy Weaponry Overview|Fantasy Weaponry]]"
ObjectSize: 2 meters
ObjectResistance: "15"
ObjectLuck: "20"
ObjectBody: "10"
FoundationTraits:
  - "[[Object]]"
MajorTraits:
  - "[[Weapon]]"
  - "[[Item]]"
MinorTraits:
  - "[[Bulky]]"
  - "[[Crushing]]"
  - "[[Unwieldly]]"
WeaponReach: 2 meters
WeaponScore: Strength
WeaponDamage: 3d6+3 impact damage
ItemSlot: 2 Hands
ItemPrereqs:
  - Strength less than 12
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

The warhammer is one of the most feared weapons on the open battlefield, with a long reach and the ability to brutally injure opponents.

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