---
description: 'Callback types:Integer'
---

# CallbackType

## List of callbacks:

### OnDraw

Fired every time the game renders a frame. Can be used to draw to the screen using the renderer.\* functions



### OnTick

Fired every time the game update object. Can be used to run champion logic.



### OnFastTick

Fired every time the game update object. Can be used to run champion logic.Faster than on tick,do not use if not neccessray.



### OnUnload

Fired ****when script unload.



### OnBeforeAttack

Fired ****before orbwalker want to attack someone.

| Key | Description |
| :--- | :--- |
| **BeforeAttackOrbwalkerArgs** | [Args](../api-documentation/callback-args/beforeattackorbwalkerargs.md). |

### 

### OnAfterAttack

Fired ****when orbwalker finish attack.

| Key | Description |
| :--- | :--- |
| **AfterAttackOrbwalkerArgs** | [Args](../api-documentation/callback-args/afterattackorbwalkerargs.md). |

### 

### OnIssueOrder

Fired ****when issue order**.**

| Key | Description |
| :--- | :--- |
| **issueorderargs\_t** | [Args](../api-documentation/callback-args/issueorderargs_t.md). |



### OnSpellCastComplete

Fired ****when a spell finish cast.

| Key | Description |
| :--- | :--- |
| **sender** | [AIBaseClient](../api-documentation/class/aibaseclient.md)**.** |
| **castargs\_t** | [args](../api-documentation/callback-args/castargs_t.md). |

#### 

### OnSpellAnimationCancel

Fired ****when a spell stop cast.

| Key | Description |
| :--- | :--- |
| **sender** | [AIBaseClient](../api-documentation/class/aibaseclient.md)**.** |
| **castargs\_t** | [Args](../api-documentation/callback-args/castargs_t.md). |

#### 

### OnSpellAnimationStart

Fired ****when a spell start cast.

| Key | Description |
| :--- | :--- |
| **sender** | [AIBaseClient](../api-documentation/class/aibaseclient.md)**.** |
| **castargs\_t** | [Args](../api-documentation/callback-args/castargs_t.md). |

#### 

### OnChangeSlotSpellName

Fired ****when a spell slot name change.

| Key | Description |
| :--- | :--- |
| **sender** | [AIBaseClient](../api-documentation/class/aibaseclient.md)**.** |
| **slot** | [Spellslot](../api-documentation/enums/spellslot.md). |
| **name** | String. |

#### 

### OnSpellCast

Fired ****when local cast spell.

| Key | Description |
| :--- | :--- |
| **castspellargs\_t** | [Args](../api-documentation/callback-args/castspellargs_t.md)**.** |



### OnObjectCreate

Fired ****when object create.

| Key | Description |
| :--- | :--- |
| **sender** | GameObject**.** |



### OnObjectRemove

Fired ****when object delete.

| Key | Description |
| :--- | :--- |
| **sender** | GameObject**.** |



### OnPrintChat

Fired ****when print a message to game chat.

| Key | Description |
| :--- | :--- |
| **message** | String**.** |
| **flags** | Integer. |



### OnNewPath

Fired ****when new path create.

| Key | Description |
| :--- | :--- |
| **sender** | [AIbaseClient](../api-documentation/class/aibaseclient.md)**.** |
| **isDash** | Boolean. |
| **dashSpeed** | Number. |
| **path** | Path array. |

**Note**: I think sometimes this callback is not reliable.When Leesin R kick someone path may incorrect.

{% code title="Example for OnNewpath callback." %}
```lua
Callback.Bind(CallbackType.OnNewPath,function(sender,isDash,dashSpeed,path)
    for i, v in path:pairs() do
         PrintChat(tostring(i))
         PrintChat(tostring(v))
    end
end)
```
{% endcode %}





### OnGainLoseBuff

Fired ****when gain or lose buff.

| Key | Description |
| :--- | :--- |
| **buffScriptInstance** | [BuffScript](../api-documentation/class/buffscript.md)**.** |
| **isGain** | Boolean. |

\*\*\*\*

### OnUpdateBuff

Fired ****when buff ****update.

| Key | Description |
| :--- | :--- |
| **sender** | [AIBaseClient](../api-documentation/class/aibaseclient.md). |
| **buffInstance** | [Buff](../api-documentation/class/buff.md). |



