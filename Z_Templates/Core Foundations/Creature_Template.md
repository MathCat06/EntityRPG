---
tags:
  - Creature
  - Entity
EntityValue: "0"
Source: None
CreatureSpeed: 1 meter
CreatureSize: 1 meter
CreatureStrength: "20"
CreatureDexterity: "20"
CreatureKnowledge: "20"
CreatureFocus: "20"
CreatureInsight: "20"
CreatureCharisma: "20"
CreatureResistance: "20"
CreatureLuck: "20"
CreatureBody: "5"
CreatureBreak: "5"
FoundationTraits:
  - "[[Creature]]"
MajorTraits:
  - "[[None]]"
MinorTraits:
  - "[[None]]"
EntityTags:
  - None
cssclasses:
  - clean-embeds
---
***Value:*** `=this.EntityValue`
***Description:***



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

***Current Body:*** 5
***Current Break:*** 5

***Wounds:*** 
None

***Tags:*** `=this.EntityTags`
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