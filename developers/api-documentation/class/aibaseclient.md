---
description: Inherited from GameObject  and AttackableUnit class.
---

# AIBaseClient

## property:

* `spellBook`\(Spellbook\)
* IsFacing \(boolean\)
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

### entity:IsBot

`entity:IsBot()`: boolean

Returns the entity is a bot.

### entity:GetDirection

`entity:GetDirection()`: Vector3

Returns the entity's direction vector.

### entity:GetPet

`entity:GetPet()`: AIBaseClient

Returns the entity's pet.

### entity:GetTarget

`entity:GetTarget()`: AttackableUnit

Returns the entity's active target.

### entity:GetSpellEntry

`entity:GetSpellEntry(slot: Spellslot)`: SpellEntry

Returns a SpellEntry.

