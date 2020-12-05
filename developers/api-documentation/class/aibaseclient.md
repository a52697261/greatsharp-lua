---
description: Inherited from GameObject  and AttackableUnit class.
---

# AIBaseClient

## property:

* `spellBook`\(Spellbook\)
* \(boolean\)
* `networkId` \(integer\)
* `isVisibleOnScreen` \(boolean\)
* `type` \(integer\)
* `flags` \(integer\)
* `displayName` \(string\)
* `bboxMax`\(Vector3\)
* `bboxMin` \(Vector3\)
* `position`\(Vector3\)
* `position2D`\(Vector2\)
* `isVisible` \(boolean\)
* `isAlive` \(boolean\)
* `isMe` \(boolean\)
* `hitboxRadius` \(float\)
* `isStructure` \(boolean\)
* `isAttacableUnit` \(boolean\)
* `isAlly` \(boolean\)
* `isEnemy` \(boolean\)
* `isNeutral` \(boolean\)
* `isMonster`  \(boolean\)
* `isAIBase` \(boolean\)
* `isMinion` \(boolean\)
* `isHero`\(boolean\)
* `isTurret` \(boolean\)
* `isMissile` \(boolean\)

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

### :GetSpellEntry

`entity:GetSpellEntry(slot: SpellSlot)`: SpellEntry

| Argument | Type | Description |
| :--- | :--- | :--- |
| **slot** | SpellSlot\(integer:0-64\) | SpellSlot enum. |

Returns a SpellEntry.

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

Use an object like lantern.

### :HasBuffOfType

`entity:HasBuffOfType(type: BuffType)`: boolean

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



