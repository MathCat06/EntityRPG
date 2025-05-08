---
tags:
  - Creature
EntityValue: "70"
Source: None
CreatureSpeed: 3 meter
CreatureSize: 1 meter
CreatureStrength: "10"
CreatureDexterity: "17"
CreatureKnowledge: "23"
CreatureFocus: "18"
CreatureInsight: "19"
CreatureCharisma: "19"
CreatureResistance: "17"
CreatureLuck: "20"
CreatureBody: "25"
CreatureBreak: "20"
FoundationTraits:
  - "[[Creature]]"
MajorTraits:
  - "[[Champion]]"
MinorTraits:
  - "[[Melee Proficiency]]"
  - "[[Champion's Strike]]"
  - "[[Expanded Champion Die]]"
  - "[[Cleave]]"
cssclasses:
  - clean-embeds
---
***Value:*** `=this.EntityValue`
***Description:***

***Inventory:*** [[Battleaxe]], [[Heavy Armor]], [[Standard Clothing]]

***Speed:*** `=this.CreatureSpeed`
***Size:*** `=this.CreatureSize`

***Strength:*** `=this.CreatureStrength`
***Dexterity:*** `=this.CreatureDexterity`
***Knowledge:*** `=this.CreatureKnowledge`
***Focus:*** `=this.CreatureFocus`
***Insight:*** `=this.CreatureInsight`
***Charisma:*** `=this.CreatureCharisma`
***Resistance:*** `=this.CreatureResistance`
***Luck:*** `=this.CreatureLuck`

***Body:*** `=this.CreatureBody`
***Break:*** `=this.CreatureBreak`

***Current Body:*** 8
***Current Break:*** 0

***Wounds:*** 
[[Stunned]]

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