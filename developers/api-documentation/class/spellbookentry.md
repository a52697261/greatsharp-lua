---
description: SpellBookEntry class.
---

# SpellBookEntry

## property:

* `info`\([SpellInfo](spellinfo.md)\)
* `isToggled`\(boolean\)
* `internalState`\(boolean\)
* `timeCooldownOver`\(number\)
* `timeNextRecharge`\(number\)
* `ammo`\(number\)
* `cooldown`\(number\)
* `rechargeTime`\(number\)

## Functions:

### :IsValid

`entry:IsValid()`: boolean

Returns if entry is valid.

### :GetName

`entry:GetName()`: string

Returns SpellData Name.



### :ManaCost

`entry:ManaCost()`: number

Returns spell mana cost.



### :DisplayRange

`entry:DisplayRange()`: number

Returns spell displayRange.



### :GetCalculateInfo

`entry:GetCalculateInfo(source: AIBaseClient, hash:number, slot: SpellSlot)`: number

| Argument | Type | Description |
| :--- | :--- | :--- |
| **source** | [AIBaseClient](aibaseclient.md) | Souce for calculate. |
| **hash** | number\(integer\) | Calculation name hash. |
| **slot** | SpellSlot\(integer:0-64\) | SpellSlot enum. |

Returns calculation result

### :PrintTooltip

`entry:PrintTooltip(extended: boolean)`:

| Argument | Type | Description |
| :--- | :--- | :--- |
| **extended** | boolean | Print extended tooltip. |

Print spell tooltip text in game. you can use **GetCalculateInfo** to get tooltip tag value**.**





### 

