---
description: SDKSpell for easy cast spell.
---

# SDKSpell

## property: <a id="property"></a>

* `slot`\(SpellSlot\)
* `lastCastAttempt`\(integer\)
* `isSkillShot`\(boolean\)
* `boundingRadiusMod`\(boolean\)
* `isChargeSpell`\(boolean\)
* `chargedBuffNameHash`\(integer\)
* `chargedMaxRange`\(number\)
* `chargedMinRange`\(number\)
* `chargedSpellNameHash`\(integer\)
* `forceSpellHash`\(integer\)
* `chargedBuffNameHash`\(integer\)
* `chargeDuration`\(number\)
* `collision`\(boolean\)
* `damageType`\(DamageType\)
* `collisionFlags`\(CollisionFlag\)
* `type`\(SkillShotType\)
* `width`\(number\)
* `speed`\(number\)
* `delay`\(number\)
* `hitchance`\(HitChance\)
* `rangeCheckFrom`\(Vector3\)
* `from`\(Vector3\)
* `range`\(number\)

## Functions: <a id="functions"></a>

### Create

`SDKSpell.Create(slot: SpellSlot, range: number, damageType: DamageType)`:SDKSpell

| Argument | Type | Description |
| :--- | :--- | :--- |
| **slot** | SpellSlot | Spell slot. |
| **range** | number | Spell range. |
| **damageType** | DamageType | Damage type. |

Create a sdk spell instance.

**​**‌

### :SetSkillshot

`spell:SetSkillshot(delay: number, width: number, type: SkillshotType, collision: boolean, collisionFlags: CollisionFlag, minHitChance: HitChance, boundingRadiusMod: boolean)`

| Argument | Type | Description |
| :--- | :--- | :--- |
| **delay** | number | Spell delay. |
| **width** | number | Spell width. |
| **type** | SkillshotType | SkillshotType`.` |
| **collision** | boolean | Should calculate collision. |
| **collisionFlags** | CollisionFlag | Collision flags**.** |
| **minHitChance** | HitChance | Min hitchance for cast. |
| **boundingRadiusMod** | boolean | Should include target bounding radius. |

Set skillshot.



### :Delete <a id="addtooltip"></a>

`spell:Delete()`

Delete spell instance and clean memory. \(Do it when unload if you create a spell and not manage it to Champions class Q/W/E/R\)



### :Ready <a id="addtooltip"></a>

`spell:Ready()`

Returns if spell is ready to cast.



### :IsCharging <a id="addtooltip"></a>

`spell:IsCharging()`

Returns if spell is charging.



### :DataInstance <a id="addtooltip"></a>

`spell:DataInstance()`:  SpellBookEntry

Returns datainstance.



### :SetCharged

`spell:SetCharged(spellName: string, buffName: string, minRange: number, maxRange: number, duration: number)`

| Argument | Type | Description |
| :--- | :--- | :--- |
| **spellName** | string | Spell name. |
| **buffName** | string | Charge buff name. |
| **minRange** | number | Min charge range. |
| **maxRange** | number | Max charge range. |
| **duration** | number | Charge max duration. |

Set charge spell like varus Q etc.



### :ManaCost <a id="addtooltip"></a>

`spell:ManaCost()`:  number

Returns spell mana cost.



### :ChargePercent <a id="addtooltip"></a>

`spell:ChargePercent()`:  number

Returns spell charge percent.



### :Cooldown <a id="addtooltip"></a>

`spell:Cooldown()`:  number

Returns spell cooldown.



### :Level <a id="addtooltip"></a>

`spell:Level()`:  number



Returns spell level.



### :CastOnUnit <a id="addtooltip"></a>

`spell:CastOnUnit(target: AIBaseClient, usePacket: boolean)`:  boolean

| Argument | Type | Description |
| :--- | :--- | :--- |
| **target** | AIBaseClient | Spell target. |
| **usePacket** | boolean | Use packet cast.\(should be **false** in most of case\) |

Returns if cast sucessfully.



### :Cast <a id="addtooltip"></a>

`spell:Cast([usePacket: boolean])`:  boolean

| Argument | Type | Description |
| :--- | :--- | :--- |
| **usePacket** | boolean | Use packet cast.\(should be **false** in most of case\) |

Returns if cast sucessfully.



### :Cast <a id="addtooltip"></a>

`spell:Cast(target: AIBaseClient[, hitChanceMenu:UI.List, usePacket:boolean])`:  boolean

| Argument | Type | Description |
| :--- | :--- | :--- |
| **target** | AIBaseClient | Spell target. |
| **hitChanceMenu** | UI.List | Use menu to check min hitchance. |
| **usePacket** | boolean | Use packet cast.\(should be **false** in most of case\) |

Returns if cast sucessfully.



### :Cast <a id="addtooltip"></a>

`spell:Cast(pos: Vector3[, limit: Vector3, usePacket: boolean])`:  boolean

| Argument | Type | Description |
| :--- | :--- | :--- |
| **pos** | Vector3 | Cast position. |
| **limit** | Vector3 | Cast posiiton limit, use for Viktor E etc. |
| **usePacket** | boolean | Use packet cast.\(should be **false** in most of case\) |

Returns if cast sucessfully.



### :GetPrediction <a id="addtooltip"></a>

`spell:GetPrediction(target:AIBaseClient)`:  [PredictionOutput](predictionoutput.md)

| Argument | Type | Description |
| :--- | :--- | :--- |
| **target** | AIBaseClient | Target. |

Returns prediction output.



### :GetDamage <a id="addtooltip"></a>

`spell:GetDamage(target:AIBaseClient[, stage:integer])`:  number

| Argument | Type | Description |
| :--- | :--- | :--- |
| **target** | AIBaseClient | Target. |
| **stage** | integer | Damage stage. |

Returns spell damage to target.



### :IsCollision <a id="addtooltip"></a>

`spell:IsCollision(from: Vector3, to: Vector3 [, target:AIBaseClient])`:  boolean

| Argument | Type | Description |
| :--- | :--- | :--- |
| **from** | Vector3 | From pos. |
| **to** | Vector3 | To pos. |
| **target** | AIBaseClient | Target to ignore. |

Returns if spell is coliision from A to B.



### :CastSpecialImmobileTarget <a id="addtooltip"></a>

`spell:CastSpecialImmobileTarget(from: Vector3, isSnare: boolean , strictlyTimeCheck: boolean])`:  boolean

| Argument | Type | Description |
| :--- | :--- | :--- |
| **from** | Vector3 | From pos. |
| **isSnare** | boolean | Is snare spell Jinx E etc. |
| **strictlyTimeCheck** | boolean | Strictly time check for some important R spell. |

Returns ture if cast sucessfully to a retrive/zhonya/teleport target.



### :StartCharging <a id="addtooltip"></a>

`spell:StartCharging(pos: Vector3, usePacket: boolean)`:  boolean

| Argument | Type | Description |
| :--- | :--- | :--- |
| **pos** | Vector3 | Cast position. |
| **usePacket** | boolean | Use packet cast.\(should be **false** in most of case\) |

Returns if cast sucessfully.



### :ShootChargedSpell <a id="addtooltip"></a>

`spell:ShootChargedSpell(pos: Vector3,releaseCast: boolean,extraRange: number, usePacket: boolean)`:  boolean

| Argument | Type | Description |
| :--- | :--- | :--- |
| **pos** | Vector3 | Cast position. |
| **releaseCast** | boolean | Is release cast. |
| **extraRange** | number | extra cast end pos. |
| **usePacket** | boolean | Use packet cast.\(should be **false** in most of case\) |

Returns if cast sucessfully.





























