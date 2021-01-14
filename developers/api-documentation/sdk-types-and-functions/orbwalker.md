---
description: Orbwalker.
---

# Orbwalker

## property:

* `lastAttackOrder`\(number\)
* `lastAttackRange`\(number\)
* `lastTargetNID`\(integer\)
* `lastAttack`\(number\)
* `missileID`\(integer\)
* `forcedPosition`\(Vector3\)
* `forcedTarget`\(AttackableUnit\)
* `bMove`\(boolean\)
* `bAttack`\(boolean\)



## Functions: <a id="functions"></a>

### GetTarget

`Orbwalker.GetTarget()`:AttackableUnit

Returns orbwalker target.

**​**‌

### :GetAttackCastDelay

`Orbwalker.GetAttackCastDelay(targetAgainst: AIBaseClient)`: number

| Argument | Type | Description |
| :--- | :--- | :--- |
| **targetAgainst** | AIBaseClient | Target against player. |

Returns **local player** 's attack cast delay against target .



### :GetAttackDelay

`Orbwalker.GetAttackDelay(targetAgainst: AIBaseClient)`: number

| Argument | Type | Description |
| :--- | :--- | :--- |
| **targetAgainst** | AIBaseClient | Target against player. |

Returns **local player** 's attack delay against target .



### :GetAttackMissileSpeed

`Orbwalker.GetAttackMissileSpeed(source: AIHeroClient,targetAgainst: AIBaseClient)`: number

| Argument | Type | Description |
| :--- | :--- | :--- |
| **source** | AIHeroClient | Souce to calculate missile speed. |
| **targetAgainst** | AIBaseClient | Target against source. |

Returns a **hero** 's attack missile speed against target .



### :CanAttack

`Orbwalker.CanAttack()`: boolean

Returns if orbwalker ready for next attack.



### :CanMove

`Orbwalker.CanMove()`: boolean

Returns if orbwalker ready for next move.



### :IsInAutoAttackRange

`Orbwalker.IsInAutoAttackRange(source: AIBaseClient,targetAgainst: AttackableUnit[,extraRange: number])`: number

| Argument | Type | Description |
| :--- | :--- | :--- |
| **source** | AIHeroClient | Souce to calculate missile speed. |
| **targetAgainst** | AIBaseClient | Target against source. |
| **extraRange** | number | Extra range for check. |

Returns if target is in source attack range.





\`\`

