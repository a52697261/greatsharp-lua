---
description: Inherited from GameObject and AttackableUnit class.
---

# AIBaseClient

## property:

* `spellBook`\([Spellbook](spellbook.md)\)
* `isZombie`\(boolean\)
* `charName`\(string\)
* `actionState`\(integer\)
* `actionState2`\(integer\)
* `isMoving`\(boolean\)
* `petOwner`\(AIBaseClient\)
* `attackDelay`\(number\)
* `attackCastDelay`\(number\)
* `isClone`\(boolean\)
* `dashSpeed`\(number\)
* `isDashing`\(boolean\)
* `serverPosition`\(Vector3\)
* `isInvulnerable`\(boolean\)
* `isMagicImmune`\(boolean\)
* `isPhysicalImmune`\(boolean\)
* `isUnstoppable`\(boolean\)
* `totalHealth`\(number\)
* `missingHealth`\(number\)
* `totalMaxHealth`\(number\)
* `totalMaxHealth`\(number\)
* `totalShield`\(number\)
* `canAttack`\(boolean\)
* `canCrit`\(boolean\)
* `canCast`\(boolean\)
* `canMove`\(boolean\)
* `isImmovable`\(boolean\)
* `isStealthed`\(boolean\)
* `isTaunted`\(boolean\)
* `isFeared`\(boolean\)
* `isFleeing`\(boolean\)
* `isSupressed`\(boolean\)
* `isAsleep`\(boolean\)
* `isGhosted`\(boolean\)
* `isCharmed`\(boolean\)
* `isDisarmed`\(boolean\)
* `isRooted`\(boolean\)
* `isSilenced`\(boolean\)
* `isStunned`\(boolean\)
* `hasAABlockingBuff`\(boolean\)
* `isMelee`\(boolean\)
* `isRanged`\(boolean\)
* `hash`\(integer\)
* `totalBaseAttackDamage`\(number\)
* `totalBonusAttackDamage`\(number\)
* `totalAttackDamage`\(number\)
* `totalAbilityPower`\(number\)
* `isCasting`\(boolean\)
* `isLaneMinion`\(boolean\)
* `isSiegeMinion`\(boolean\)
* `isSuperMinion`\(boolean\)
* `isCasterdMinion`\(boolean\)
* `isMeleeMinion`\(integer\)
* `isPet`\(boolean\)
* `isWard`\(boolean\)
* `isWardNoBlue`\(boolean\)
* `isTrap`\(boolean\)
* `isPlant`\(boolean\)
* `isLargeMonster`\(boolean\)
* `isBaron`\(boolean\)
* `isDragon`\(boolean\)
* `isEpicMonster`\(boolean\)
* `isSmiteMonster`\(boolean\)
* `charIntermediate`\([CharIntermediate](charintermediate.md)\)



## Functions:

### :IsBot

`entity:IsBot()`: boolean

Returns the entity is a bot.



### :GetDirection

`entity:GetDirection()`: Vector3

Returns the entity's direction vector.



### :GetPet

`entity:GetPet()`: AIBaseClient

Returns the entity's pet.



### :GetTarget

`entity:GetTarget()`: AttackableUnit

Returns the entity's active target.

### :GetWayPoint

`entity:GetWayPoint()`: Vector3

Returns the entity's last waypoint.



### :GetRemainingPath2D

`entity:GetRemainingPath2D()`: std::vector&lt;Vector2&gt;

Returns the entity's remaining path array.



### :GetSpellEntry

`entity:GetSpellEntry(slot: SpellSlot)`: [SpellBookEntry](spellbookentry.md)

| Argument | Type | Description |
| :--- | :--- | :--- |
| **slot** | SpellSlot\(integer:0-64\) | SpellSlot enum. |

Returns a SpellBookEntry.



### :GetAutoAttackDamage

`entity:GetAutoAttackDamage(target: AttackableUnit)`: number

| Argument | Type | Description |
| :--- | :--- | :--- |
| **target** | AttackableUnit | Target. |

Returns a entity's auto attack damage to target.



### :IsFacing

`entity:IsFacing(source: AIBaseClient, angle: number, range: number):` boolean

| Argument | Type | Description |
| :--- | :--- | :--- |
| **source** | AIBaseClient | Check from source. |
| **angle** | number \(float\) | Cone angle. |
| **range** | number \(float\) | Max check range. |

Returns if entity is facing source \(inside cone\).



### :UseObject

`entity:UseObject(target: AttackableUnit)`

| Argument | Type | Description |
| :--- | :--- | :--- |
| **target** | AttackableUnit | Target to use. |

Use an object like lantern etc.



### :HasBuffOfType

`entity:HasBuffOfType(type:` [`BuffType`](../enums/bufftype.md)`)`: boolean

| Argument | Type | Description |
| :--- | :--- | :--- |
| **type** | BuffType\(integer\) | BuffType enum. |

Returns if has buff of type.



### :IsCloneFrom

`entity:IsCloneFrom(source: AIBaseClient)`: boolean

| Argument | Type | Description |
| :--- | :--- | :--- |
| **source** | AIBaseClient | Source of clone. |

Returns if entity is a clone from source entity.



### :CanUseSpell

`entity:CanUseSpell(slot: SpellSlot)`: boolean

| Argument | Type | Description |
| :--- | :--- | :--- |
| **slot** | SpellSot\(integer:0-64\) | SpellSlot enum. |

Returns if entity can use spell of given slot.



### :GetRealHealth

`entity:GetRealHealth(msTime: number, type: DamageType)`: number

| Argument | Type | Description |
| :--- | :--- | :--- |
| **msTime** | `number(float)` | Time to predict HPRegenRate. |
| **type** | `DamageType` | DamageType enum. |

Returns entity real health include Shields and Blitzcrank's passive.



### :GetBuff

`entity:GetBuff(index: Integer)`: [Buff](buff.md)

| Argument | Type | Description |
| :--- | :--- | :--- |
| **index** | Integer | Buff array index. |

Returns a buff at \[index\].



### :FindBuff

`entity:GetBuff(hash: number)`: [Buff](buff.md)

| Argument | Type | Description |
| :--- | :--- | :--- |
| **hash** | number\(Integer\) | Buff name Hash |

Returns Buff find by fnv\_hash\(name\).



### :GetBuffStacks

`entity:GetBuffStacks(hash: number)`: number

| Argument | Type | Description |
| :--- | :--- | :--- |
| **hash** | number\(Integer\) | Buff name Hash |

Returns Buff stacks find by fnv\_hash\(name\).



### :GetAutoAttackRange

`entity:GetAutoAttackRange([target: AttackableUnit])`: number

| Argument | Type | Description |
| :--- | :--- | :--- |
| **target** | `AttackableUnit` | Target could be null. |

Returns real auto attack range \(worked for Azir , Aphelios ,Caitlyn and all heroes\).

