---
description: SpellBook class.
---

# SpellBook

## Functions:

### :GetSpellEntry

`spellbook:GetSpellEntry(slot: SpellSlot)`: [SpellBookEntry](spellbookentry.md)

| Argument | Type | Description |
| :--- | :--- | :--- |
| **slot** | SpellSlot\(integer:0-64\) | SpellSlot enum. |

Returns SpellBookEntry.



### :GetSpellEntry

`spellbook:GetSpellEntry(spellname: string)`: SpellSlot

| Argument | Type | Description |
| :--- | :--- | :--- |
| **spellname** | string | Spell Name for finding spell. |

If find , returns  SpellSlot .

Else returns SpellSlot.NullSlot.



### :PrintSpells

`spellbook:GetSpellEntry(slot: SpellSlot)`

| Argument | Type | Description |
| :--- | :--- | :--- |
| **slot** | SpellSlot\(integer:0-64\) | SpellSlot enum. |

Print spell range,cost and missile speed on console.

