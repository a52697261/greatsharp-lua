---
description: Buffs Manger.
---

# BuffManager

## property:

* `buffs`\(std::vector&lt;buff&gt;\)
* `owner`\(AIBaseClient\)
* `ownerHandle`\(integer\)
* `ownerNetworkID`\(integer\)

## Functions:

### BuffManager.GetDragonBuffCount

`BuffManager.GetDragonBuffCount(type: DragonType, team:Team)`: integer

| Argument | Type | Description |
| :--- | :--- | :--- |
| **type** | [DragonType](../enums/dragontype.md) | DragonType enum. |
| **team** | [Team](../enums/team.md) | Team number. |

Returns team dragon buff count.

