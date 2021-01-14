---
description: Inherited from GameObject class.
---

# AttackableUnit

## property:

* `mp` \(number\)
* `maxMp` \(number\)
* `resourceType`\(integer\)
* `secondaryResource`\(number\)
* `maxSecondaryResource`\(number\)
* `statusFlags`\(integer\)
* `pathfindingCollisionRadius`\(number\)
* `lifetime`\(number\)
* `maxLifetime`\(number\)
* `lifetimeTicks`\(number\)
* `physicalDamagePercentageModifier`\(number\)
* `magicalDamagePercentageModifier`\(number\)
* `hpPercent`\(number\)
* `mpPercent`\(number\)
* `isVisible`\(boolean\)

## Functions:

### :IsWindingUp

`entity:IsWindingUp()`: boolean

Returns if this entity is winding up.



### :IsValidTarget

`entity:IsValidTarget([range: number, onlyEnemyTeam: number, from: [Vector2 or Vector3]])`: boolean

| Argument | Type | Description |
| :--- | :--- | :--- |
| **range** | number | Check range. |
| **onlyEnemyTeam** | bool | Check target team. |
| **from** | Vector2 or Vector3 | Check from pos. |

Returns if this entity is valid target.

