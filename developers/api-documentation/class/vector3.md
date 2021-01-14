---
description: Vector3 class.
---

# Vector3

## property:

* `x`\(number\)
* `y`\(number\)
* `z`\(number\)

## Functions:

## :**To2D**

`vector3:To2D()`: Vector2

Returns a Vector2 \(x =x, y =z\).



### :To3D

`vector3:To3D()`: [Vector3](vector3.md)

Returns a Vector3 \(x =x, y =y, z=z\).



### :Copy

`vector3:Copy()`: Vector3

Returns a Vector3 \(x =x, y =y, z=z\).



### :FixHeight

`vector3:FixHeight()`: Vector3

Returns this **ref** Vector3 \(x =x, y =GameMapHeight, z=z\).



### :Project

`vector3:Project()`: [Vector2](vector2.md)

Returns a screen position Vector2\(WorldToScreen\).



### :ToCell

`vector3:ToCell()`: NavGridCell

Returns navGridCell\(userdata\).



### :Length

`vector3:Length()`: number

Returns vector length.



### :Length2

`vector3:Length2()`: number

Returns vector length **square**.



### :Distance <a id="database-read"></a>

`vector3:Distance(v2: Vector3)`: number

| Argument | Type | Description |
| :--- | :--- | :--- |
| **v2** | Vector3 | Point2. |

Returns distance from v to v2.



### :Distance2 <a id="database-read"></a>

`vector3:Distance(v2: Vector3)`: number

| Argument | Type | Description |
| :--- | :--- | :--- |
| **v2** | Vector3 | Point2. |

Returns distance **square** from v to v2.



### :Dot <a id="database-read"></a>

`vector2:Dot(v2: Vector3)`: number

| Argument | Type | Description |
| :--- | :--- | :--- |
| **v2** | Vector3 | Point2. |

Returns dot product result.



### :Cross <a id="database-read"></a>

`vector3:`Cross`(v2: Vector3)`: Vector3

| Argument | Type | Description |
| :--- | :--- | :--- |
| **v2** | Vector3 | Point2. |

Returns cross product result.



### :Normalize

`vector3:Normalize()`: Vector3

Returns a normalized Vector3 from this vector.



### :Lerp <a id="database-read"></a>

`vector3:Lerp(v2: Vector3, time: number)`: Vector3

| Argument | Type | Description |
| :--- | :--- | :--- |
| **v2** | Vector3 | Point2. |
| **time** | number\(float\) | Time. |

Returns Linear interpolation. V1 + s \(V2-V1\)



### :Unpack

`vector3:Unpack()`: number, number,number

Returns two numbers x,y.z



### :ToCell

`vector3:ToCell()`: NavGridCell

Returns navGridCell\(userdata\).



### :RelativePos <a id="database-read"></a>

`vector3:RelativePos(v2: Vector3, distance: number)`: Vector3

| Argument | Type | Description |
| :--- | :--- | :--- |
| **v2** | Vector3 | Point2. |
| **distance** | number\(float\) | Distance to extended. |

Returns relative position in direction from v to v2 as Vector3.



### :RelativeFlatPos <a id="database-read"></a>

`vector3:RelativeFlatPos(v2: Vector3, distance: number)`: Vector3

| Argument | Type | Description |
| :--- | :--- | :--- |
| **v2** | Vector3 | Point2. |
| **distance** | number\(float\) | Distance to extended. |

Returns relative flat position in direction from v to v2 as Vector 2 with corrected height.



### :Randomize

`vector3:Randomize()`: Vector3

Randomizes vector a little.



### :Direction

`vector3:Direction()`: Vector3

Returns normalized direction vector.



### :Normal

`vector3:Normal()`: Vector3

Returns normal.



### :FlatDistance <a id="database-read"></a>

`vector3:DistanceToVec3(v2: Vector3)`: number

| Argument | Type | Description |
| :--- | :--- | :--- |
| **v2** | Vector3 | Point2. |

Returns **flat** distance ****from this to v2.



### :FlatDistanceToVec2 <a id="database-read"></a>

`vector2:DistanceToVec3(v2:` [`Vector2`](vector2.md)`)`: number

| Argument | Type | Description |
| :--- | :--- | :--- |
| **v2** | Vector2 | Point2. |

Returns **flat** distance ****from this to v2.



### :IsUnderEnemyTurret

`vector3:IsUnderEnemyTurret()`: boolean

Returns if vector3 is under enemy turret.



### :IsUnderAllyTurret

`vector3:IsUnderAllyTurret()`: boolean

Returns if vector3 is under ally turret.



### :CountAlliesInRange

`vector3:CountAlliesInRange(range: number)`: number

| Argument | Type | Description |
| :--- | :--- | :--- |
| **range** | number | Check range. |

Returns if how many **valid**  allies is in vector3 range\(**include me**\).



### :CountAllyLaneMinionsInRange

`vector3:CountAllyLaneMinionsInRange(range: number)`: number

| Argument | Type | Description |
| :--- | :--- | :--- |
| **range** | number | Check range. |

Returns if how many **valid** ally minions is in vector3 range.

### :CountEnemyLaneMinionsInRange

`vector3:CountEnemyLaneMinionsInRange(range: number)`: number

| Argument | Type | Description |
| :--- | :--- | :--- |
| **range** | number | Check range. |

Returns if how many **valid** enemy **lane** minions is in vector3 range.



### :CountEnemiesInRange

`vector3:CountEnemiesInRange(range: number)`: number

| Argument | Type | Description |
| :--- | :--- | :--- |
| **range** | number | Check range. |

Returns if how many **valid** enemies is in vector3 range.



### :IsWall

`vector3:IsWall(actorTeam: number)`: boolean

| Argument | Type | Description |
| :--- | :--- | :--- |
| **actorTeam** | number:integer | Actor team to check special air wall . \(300 == ignore air wall\) |

Returns if vector3 is not walkable.



