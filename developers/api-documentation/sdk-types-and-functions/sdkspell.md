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

Create a  sdk spell instance.

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
| `boundingRadiusMod` |  |  |

Set charge spell like varus Q etc.



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

















