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
| **BeforeAttackOrbwalkerArgs** | args. |

### 

### OnAfterAttack

Fired ****when orbwalker finish attack.

| Key | Description |
| :--- | :--- |
| **AfterAttackOrbwalkerArgs** | args. |

### 

### OnIssueOrder

Fired ****when issue order**.**

| Key | Description |
| :--- | :--- |
| **issueorderargs\_t** | args. |



### OnSpellCastComplete

Fired ****when a spell finish cast.

| Key | Description |
| :--- | :--- |
| **sender** | AIBaseClient**.** |
| **castargs\_t** | args. |

#### 

### OnSpellAnimationCancel

Fired ****when a spell stop cast.

| Key | Description |
| :--- | :--- |
| **sender** | AIBaseClient**.** |
| **castargs\_t** | args. |

#### 

### OnSpellAnimationStart

Fired ****when a spell start cast.

| Key | Description |
| :--- | :--- |
| **sender** | AIBaseClient**.** |
| **castargs\_t** | args. |

#### 

### OnChangeSlotSpellName

Fired ****when a spell slot name change.

| Key | Description |
| :--- | :--- |
| **sender** | AIBaseClient**.** |
| **slot** | Spellslot. |
| **name** | String. |

#### 

### OnSpellCast

Fired ****when local cast spell.

| Key | Description |
| :--- | :--- |
| **castspellargs\_t** | args**.** |



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
| **flags** | integer. |



### OnNewPath

Fired ****when new path create.

| Key | Description |
| :--- | :--- |
| **sender** | AIbaseClient**.** |
| **isDash** | boolean. |
| **dashSpeed** | number. |
| **path** | Path array. |

**Note**: I think sometimes this callback is not reliable.When Leesin R kick someone path may incorrect.





