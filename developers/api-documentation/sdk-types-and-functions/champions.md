---
description: Champions script manager.
---

# Champions



## property: <a id="property"></a>

* `Q`\(SDKSpell\)
* `W`\(SDKSpell\)
* `E`\(SDKSpell\)
* `R`\(SDKSpell\)
* `QMANA`\(number\)
* `WMANA`\(number\)
* `EMANA`\(number\)
* `RMANA`\(number\)
* `Combo`\(boolean\)
* `Harass`\(boolean\)
* `LaneClear`\(boolean\)
* `None`\(boolean\)
* `Flee`\(boolean\)
* `OnlyHarass`\(boolean\)
* `Hash`\(interger\)
* `FarmMinions`\(UI.Slider\)
* `spellFarm`\(UI.KeyBind\)
* `harassToggle`\(UI.KeyBind\)
* `PredictionType`\(UI.List\)

**note:Q/W/E/R/QMANA/WMANA/EMANA/RMANA shoud be set by your self.** 

\*\*\*\*

**Examples:**

{% tabs %}
{% tab %}
```lua
 --Manager Spell class pointer so we call use  Champions.Clean() when unload
        Champions.Q = SDKSpell.Create(SpellSlot.Q,1400,DamageType.Magical)
        Champions.W = SDKSpell.Create(SpellSlot.W,100,DamageType.Magical)
        Champions.E = SDKSpell.Create(SpellSlot.E,1200,DamageType.Magical)
        Champions.R = SDKSpell.Create (SpellSlot.R,5500,DamageType.Magical)
 --Set skillshot        
        Champions.Q:SetSkillshot(0.25,60,1000,SkillshotType.SkillshotLine,true,CollisionFlag.CollidesWithYasuoWall,HitChance.High,true)
        Champions.R:SetSkillshot(1,65,math.huge,SkillshotType.SkillshotCircle,false,CollisionFlag.CollidesWithNothing,HitChance.High,true)
       
```
{% endtab %}
{% endtabs %}

## Functions: <a id="functions"></a>

### CreateBaseMenu

`Champions.CreateBaseMenu(menu: UI.Menu, predictionType: integer)`

| Argument | Type | Description |
| :--- | :--- | :--- |
| **menu** | UI.Menu | Root menu. |
| **predictionType** | integer\(0-1\) | Default prediction type\(0 = default ,1 = fast\). |

Create a champion base menu.

**​**‌

### :CreateColorMenu

`Champions.CreateColorMenu(menu: UI.Menu, defaultValue: boolean)`

| Argument | Type | Description |
| :--- | :--- | :--- |
| **menu** | UI.Menu | Dawing sub menu. |
| **defaultValue** | boolean | Default value of range check box. |

Create a champion Q\W\E\R drawing menu \(If Chamipons.Q/W/E/R has been set\).



**LagFree**

`Champions.LagFree(index: integer)`

| Argument | Type | Description |
| :--- | :--- | :--- |
| **index** | integer\(0-4\) | Index. |

Lagfree check for better performance.



**CanHarass**

`Champions.CanHarass()`

Harass check  \(under enemy turret and toggle check\).



### CanSpellFarm

`Champions.CanSpellFarm([checkMinionsNumber: boolean])`

| Argument | Type | Description |
| :--- | :--- | :--- |
| **checkMinionsNumber** | boolean\(false\) | Should check enemy minions aournd with laneclear slider. |

Spell farm check  \(check spellFarm toggle,mana setting,minions nearby and orbwalker is LaneClear mode\).



### CppScriptMaster

`Champions.CppScriptMaster(enable: boolean)`

| Argument | Type | Description |
| :--- | :--- | :--- |
| **enable** | boolean | Enabled. |

Master switch to control internal Cpp scripts.



### CanMove

`Champions.CanMove(target: AIBaseClient, delay:number)`

| Argument | Type | Description |
| :--- | :--- | :--- |
| **target** | AIBaseClient | Target. |
| **delay** | number | After the delay target can move. |

Check a target is can move\(not been CCed\) after delay.



### GetIncomingDamage

`Champions.GetIncomingDamage(target: AIBaseClient)`

| Argument | Type | Description |
| :--- | :--- | :--- |
| **target** | AIBaseClient | Target. |

Get incoming damage.



**IsMovingInSameDirection**

`Champions.IsMovingInSameDirection(source: AIBaseClient, target: AIBaseClient, angle: number)`

| Argument | Type | Description |
| :--- | :--- | :--- |
| **source** | AIBaseClient | Source |
| **target** | AIBaseClient | Target. |
| **angle** | number\(default = 20\) | Angle for check. |

Returns if souce and target is moving in same direction.



### ValidKillTarget

`Champions.ValidKillTarget(target: AIBaseClient, delay: number)`

| Argument | Type | Description |
| :--- | :--- | :--- |
| **target** | AIBaseClient | Target. |
| **delay** | number | Spell delay. |

Returns if target is unkillable after delay.



### ValidUlt

`Champions.ValidUlt(target: AIBaseClient, delay: number)`

| Argument | Type | Description |
| :--- | :--- | :--- |
| **target** | AIBaseClient | Target. |
| **delay** | number | Spell delay. |

Returns if target is unkillable or **overkill** after delay.



**Clean**

`Champions.Clean()`

Clean base menu  and QWER instance. Should be called when **unload**.















