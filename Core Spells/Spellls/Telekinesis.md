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
  - "[[Concentration 0]]"
cssclasses:
  - clean-embeds
EntityTags:
  - None
SpellTags:
  - "[[Mage]]"
SpellPower: "1"
SpellVersatility: "5"
SpellCastingTime: 1 Action
---
***Value:*** `=this.EntityValue`
***Power:*** `=this.SpellPower`
***Versatility:*** `=this.SpellVersatility`
***Casting Time:*** `=this.SpellCastingTime`
***Description:***

You exert a mental force on another object or creature you can see, lifting or moving the target.

Choose an object or creature creature you can see within 10 meters that has a size at or under 1/2 meter, and manipulate it as you wish as long as you hold concentration on this spell. Your options are as follows:

- 1 Action: Move it a distance equal to you speed in any direction (even into the air, if its size is less than or equal to 1/2 the targetable size).
- 2 Actions: Make an attack against the target using the [[Unarmed Strike]] weapon.

If a creature is targeted with this spell, it must make a Strength or Dexterity Check to avoid the effects of the spell, and may make another check at the cost of 2 Actions.

For each additional 5 power spent when casting this spell, you may target a creature or object an additional 10 meters away and 1/2 meter larger.

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