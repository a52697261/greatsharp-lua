---
description: Bind or unbind event.
---

# Callback

## Functions:

### Callback**.Bind**

`Callback.Bind(type:CallbackType, callback: function[, ...] [,priority:number])`: number



| Argument | Type | Description |
| :--- | :--- | :--- |
| **type** | [CallbackType](../enums/callback.md) | CallbackType. |
| **callback** | function | Callback function. |
| **priority** | number\(integer\) | Callback priority\(default 0\) |

Returns callback unique id.



### Callback**.**Unbind

`Callback.Unbind(id:number)`

Unblind callback by unique id.

