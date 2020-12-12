---
description: Vector2 class
---

# Vector2



## property:

* x\(number\)
* y\(number\)

## Functions:

### :To3D

`vector2:To3D()`: [Vector3](vector3.md)

Returns a Vector3 \(x =x, y =0, z=y\).



### :To2D

`vector2:To2D()`: Vector2

Returns a Vector2 \(x =x, y =y\).



### :Copy

`vector2:Copy()`: Vector2

Returns a Vector2 \(x =x, y =y\).



### :Project

`vector2:Project()`: [Vector3](vector3.md)

Returns a game world position Vector3 \(ScreenToWorld\).



### :ProjectOnLine <a id="database-read"></a>

`vector2:ProjectOnLine(A: Vector2, B: Vector2)`: Vector2

| Argument | Type | Description |
| :--- | :--- | :--- |
| **A** | Vector2 | Line  start. |
| **B** | Vector2 | Line  end. |

Returns project on line AB.



### :ProjectOnLineSegment <a id="database-read"></a>

`vector2:ProjectOnLineSegment(A: Vector2, B: Vector2)`: Vector2

| Argument | Type | Description |
| :--- | :--- | :--- |
| **A** | Vector2 | Line segment start. |
| **B** | Vector2 | Line segment end. |

Returns project on line segment AB.



### :IsOnLineSegment <a id="database-read"></a>

`vector2:IsOnLineSegment(A: Vector2, B: Vector2)`: boolean

| Argument | Type | Description |
| :--- | :--- | :--- |
| **A** | Vector2 | Line segment start. |
| **B** | Vector2 | Line segment end. |

Returns if point's project is on line segment AB.



### :Length

`vector2:Length()`: number

Returns vector length.



### :Length2

`vector2:Length2()`: number

Returns vector length **square**.



### :Distance <a id="database-read"></a>

`vector2:Distance(v2: Vector2)`: number

| Argument | Type | Description |
| :--- | :--- | :--- |
| **v2** | Vector2 | Point2. |

Returns distance from v to v2.



### :Distance2 <a id="database-read"></a>

`vector2:Distance(v2: Vector2)`: number

| Argument | Type | Description |
| :--- | :--- | :--- |
| **v2** | Vector2 | Point2. |

Returns distance **square** from v to v2.



### :Dot <a id="database-read"></a>

`vector2:Dot(v2: Vector2)`: number

| Argument | Type | Description |
| :--- | :--- | :--- |
| **v2** | Vector2 | Point2. |

Returns dot result.



### :Normalize

`vector2:Normalize()`: Vector2

Returns a normalized Vector2 from this vector.



### :Lerp <a id="database-read"></a>

`vector2:Lerp(v2: Vector2)`: Vector2

| Argument | Type | Description |
| :--- | :--- | :--- |
| **v2** | Vector2 | Point2. |
| **time** | number\(float\) | Time. |

Returns Linear interpolation. V1 + s \(V2-V1\)



### :Angle

`vector2:Angle()`: number

Returns this vector angle.



### :AngleDeg

`vector2:AngleDeg()`: number

Returns this vector angle **degree**.



### :AngleBetween <a id="database-read"></a>

`vector2:AngleBetween(v2: Vector2)`: number

| Argument | Type | Description |
| :--- | :--- | :--- |
| **v2** | Vector2 | Point2. |

Returns angle between this and v2.



### :AngleDegBetween <a id="database-read"></a>

`vector2:AngleDegBetween(v2: Vector2)`: number

| Argument | Type | Description |
| :--- | :--- | :--- |
| **v2** | Vector2 | Point2. |

Returns angle **degree** between this and v2.



### :Rotate <a id="database-read"></a>

`vector2:Rotate(angle: number)`: Vector2

| Argument | Type | Description |
| :--- | :--- | :--- |
| **angle** | number\(float\) | Angle for rotate. |

Returns a vector2 rotate angle .



### :RotateDeg <a id="database-read"></a>

`vector2:RotateDeg(angle: number)`: Vector2

| Argument | Type | Description |
| :--- | :--- | :--- |
| **angle** | number\(float\) | Angle for rotate. |

Returns a vector2 rotate angle **degree** .



### :Unpack

`vector2:Unpack()`: number, number

Returns two numbers x,y.



### :RelativePos <a id="database-read"></a>

`vector2:RelativePos(v2: Vector2, distance: number)`: Vector2

| Argument | Type | Description |
| :--- | :--- | :--- |
| **v2** | Vector2 | Point2. |
| **distance** | number\(float\) | Distance to extended. |

Returns a Vector2 that extened or shorter a given distance ****.



### :Randomize

`vector2:Randomize()`: Vector2

Randomizes vector a little.



### :Direction

`vector2:Direction()`: Vector2

Returns normalized direction vector.



### :Normal

`vector2:Normal()`: Vector2

Returns normal.



### :DistanceToVec3 <a id="database-read"></a>

`vector2:DistanceToVec3(v2:` [`Vector3`](vector3.md)`)`: number

| Argument | Type | Description |
| :--- | :--- | :--- |
| **v2** | Vector3 | Point2. |

Returns distance ****from this to v2.



### :DistanceToLine <a id="database-read"></a>

`vector2:DistanceToLine(A: Vector2, B:Vector2)`: number

| Argument | Type | Description |
| :--- | :--- | :--- |
| **A** | Vector3 | Line start. |
| B | Vector3 | Line end. |

Returns distance ****from this to line AB.



### :DistanceToLine2 <a id="database-read"></a>

`vector2:DistanceToLine2(A: Vector2, B:Vector2)`: number

| Argument | Type | Description |
| :--- | :--- | :--- |
| **A** | Vector3 | Line start. |
| B | Vector3 | Line end. |

Returns distance **square** from this to line AB.















