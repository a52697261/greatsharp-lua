---
description: Base entity class.
---

# GameObject

## property:

* `team` \(integer\)
* `handle` \(integer\)
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

### :Level

`entity:Level()`: number

Returns the entity level.

### :GetAddress

`entity:GetAddress()`: number

Returns the entity's memory address.

### :PrintAddress

`entity:PrintAddress()`

Print the entity's memory address on console.

### :IsValid

`entity:IsValid()`: boolean

Returns if this is a valid entity.

### :GetUniqueName

`entity:GetUniqueName()`: string

Returns entity's unique name.

### :GetData

`entity:GetData()`: table \(any\)

Returns entity's unique data table.



## Note:

"**\_\_eq**"  has been override so that you can just use "==" to compare entities.









