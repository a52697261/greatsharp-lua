---
description: 'CollisionFlag enum:bit flag.'
---

# CollisionFlag

`CollisionFlag.CollidesWithNothing`

`CollisionFlag.CollidesWithYasuoWall`

`CollisionFlag.CollidesWithMinions`

`CollisionFlag.CollidesWithWalls`

`CollisionFlag.CollidesWithStructures`

`CollisionFlag.CollidesWithHeroes`

**Note:you can use bit operation to contact multi flag.**

\*\*\*\*

**Examples:**

{% tabs %}
{% tab %}
```lua
--Set Collides with Minions,YasuoWall and Heroes.
collisionFlags = bit.bor(CollisionFlag.CollidesWithYasuoWall,CollisionFlag.CollidesWithMinions,CollisionFlag.CollidesWithHeroes)
Champions.Q:SetSkillshot(0.25,60,1000,SkillshotType.SkillshotLine,true,collisionFlags,HitChance.High,true)
        
```
{% endtab %}
{% endtabs %}

