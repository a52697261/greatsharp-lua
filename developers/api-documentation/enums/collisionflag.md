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
collisionFlags = bit.bor(CollisionFlag.CollidesWithYasuoWall,CollisionFlag.CollidesWithMinions,CollisionFlag.CollidesWithHeroes)
```
{% endtab %}
{% endtabs %}

