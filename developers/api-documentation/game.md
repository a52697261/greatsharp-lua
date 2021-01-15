---
description: Game info and functions.
---

# Game

## property:

* `localPlayer`\(AIHeroClient\)

## Functions:

### Game.GetTickCount <a id="database-read"></a>

`Game.GetTickCount()`: integer

Returns game tick count now.



### Game.GetTime <a id="database-read"></a>

`Game.GetTime()`: number

Returns game clock time now.



### Game.fnvhash <a id="database-read"></a>

`Game.fnvhash(str: string)`: integer

| Argument | Type | Description |
| :--- | :--- | :--- |
| str | string | String for calculate\(case ignore\). |

Returns fnvhash of string.



### Game.spelldataHash <a id="database-read"></a>

`Game.spelldataHash(str: string)`: integer

| Argument | Type | Description |
| :--- | :--- | :--- |
| str | string | String for calculate\(case ignore\). |

Returns spelldataHash of string.



### Game.GameID <a id="database-read"></a>

`Game.GameID()`: number

Returns game id.



### Game.GameMode <a id="database-read"></a>

`Game.GameMode()`: string

Returns game mode.



### Game.GameType <a id="database-read"></a>

`Game.GameType()`: string

Returns game type.



### Game.IsMatchmadeGame <a id="database-read"></a>

`Game.IsMatchmadeGame()`: boolean

Returns if game is not custom.



### Game.Region <a id="database-read"></a>

`Game.Region()`: string

Returns game region.



### Game.MapID <a id="database-read"></a>

`Game.MapID()`: integer

Returns game map id.



### Game.MapName <a id="database-read"></a>

`Game.MapName()`: string

Returns game map name.



### Game.IsWallOfType <a id="database-read"></a>

`Game.IsWallOfType(pos: Vector2 or Vector3, flag: CellFlag, radius: number)`: boolean

| Argument | Type | Description |
| :--- | :--- | :--- |
| **pos** | Vector2 or Vector3 | Check pos. |
| **flag** | CellFlag | Flag for check. |
| **radius** | number | Range for check. |

Returns pos is wall of type wall.





### Game.IsInFoW <a id="database-read"></a>

`Game.IsInFoW(pos: Vector3)`: boolean

| Argument | Type | Description |
| :--- | :--- | :--- |
| **pos** | Vector3 | Check pos. |

Returns pos is in fow.



### Game.GetSpellByHash <a id="database-read"></a>

`Game.GetSpellByHash(spellHash: integer)`: [Spell](class/spell.md)

| Argument | Type | Description |
| :--- | :--- | :--- |
| **spellHash** | integer | Spell hash. |

Get Spelldata by spell hash.



**Examples:**

{% tabs %}
{% tab %}
```lua
-- Get spelldata info value
local WSpell = Game.GetSpellByHash(Game.spelldataHash("PickACard")) --you can get spelldata by hash
if WSpell then
    local sucusss,value = WSpell:GetCalculateInfo(Game.fnvhash("GoldBase"),W:DataInstance().level)
     print(value)
end
```
{% endtab %}
{% endtabs %}









