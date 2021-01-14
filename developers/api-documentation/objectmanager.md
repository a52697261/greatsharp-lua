---
description: ObjectManager contains some list of objects.
---

# ObjectManager

## property:

* `enemyHeroes`\(list\)
* `enemyLaneMinions` \(list\)
* `allyHeroes`\(list\)
* `activeAllyWindWalls`\(list\)
* `activeEnemyWindWalls`\(list\)
* `allAIBaseClients`\(list\)
* `allAttackableUnits` \(list\)
* `allGameObjects`\(list\)
* `allMissileClients`\(list\)
* `enemyMinions`\(list\)
* `enemyPets`\(list\)
* `enemyStructures`\(list\)
* `enemyTurrets`\(list\)
* `enemyWards`\(list\)
* `allyLaneMinions`\(list\)
* `allyMinions`\(list\)
* `allyPets`\(list\)
* `allyTurrets`\(list\)
* `allyWards`\(list\)
* `barrels`\(list\)
* `jungleMinions`\(list\)



**Examples:**

{% tabs %}
{% tab %}
```lua
-- find first can't move enemy and cast spell Q.
for _, entity in ObjectManager.enemyHeroes:pairs() do
    if entity:IsValidTarget(Q.range) and not Champions.CanMove(entity,0.1) and Q:Cast(entity,menu.Q.hitchanceQ) then
        return;
    end
end
```
{% endtab %}
{% endtabs %}

\`\`

## Functions:

### ObjectManager.ResolveHandle

`ObjectManager.resolveHandle(handle: number)`: [GameObject](class/gameobject.md)

| Argument | Type | Description |
| :--- | :--- | :--- |
| **handle** | number \(integer\) | Handle for query. |

Get a object by handle.\(if failed,returns nil\)



### ObjectManager.ResolveNetworkId

`ObjectManager.ResolveHandle(netHandle: number)`: [GameObject](class/gameobject.md)

| Argument | Type | Description |
| :--- | :--- | :--- |
| **netHandle** | number \(integer\) | Network handle for query. |

Get a object by net handle.\(if failed,returns nil\)

