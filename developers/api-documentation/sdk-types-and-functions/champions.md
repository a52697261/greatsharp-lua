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

