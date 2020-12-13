---
description: Math library.
---

# Math

## Functions:

### Math.LineIntersection <a id="database-read"></a>

`Math.LineIntersection(a1:` [`Vector2`](../class/vector2.md)`, a2:` [`Vector2`](../class/vector2.md)`, b1:` [`Vector2`](../class/vector2.md)`, b2:` [`Vector2`](../class/vector2.md)`)`: boolean

| Argument | Type | Description |
| :--- | :--- | :--- |
| **a1** | Vector2 | Line 1 start. |
| **a2** | Vector2 | Line 1 end. |
| **b1** | Vector2 | Line 2 start. |
| **b2** | Vector2 | Line 2 end. |

Returns if Line1 and Line2 have Intersection.

### Math.LineSegmentIntersection <a id="database-read"></a>

`Math.LineSegmentIntersection(a1:` [`Vector2`](../class/vector2.md)`, a2:` [`Vector2`](../class/vector2.md)`, b1:` [`Vector2`](../class/vector2.md)`, b2:` [`Vector2`](../class/vector2.md)`)`: boolean

| Argument | Type | Description |
| :--- | :--- | :--- |
| **a1** | Vector2 | Segment 1 start. |
| **a2** | Vector2 | Segment1 end. |
| **b1** | Vector2 | Segment2 start. |
| **b2** | Vector2 | Segment2 end. |

Returns if Line1 and Line2 have Intersection.



### Math.FastSqrt <a id="database-read"></a>

`Math.FastSqrt(value: number)`: number

| Argument | Type | Description |
| :--- | :--- | :--- |
| **value** | number\(float\) | Number for sqrt. |

Returns sqrt result.



### Math.QuaternionRotation <a id="database-read"></a>

`Math.QuaternionRotation(yaw: number, pitch: number, roll: number)`: [Vector4](../class/vector4.md)

| Argument | Type | Description |
| :--- | :--- | :--- |
| **yaw** | number\(float\) | Yaw |
| **pitch** | number\(float\) | Pitch |
| **roll** | number\(float\) | Angle |

Returns Quaternion Rotation Vector4.



### Math.Vector4 <a id="database-read"></a>

`Math.Vector4(x: number, y: number, z: number, w: number)`: [Vector4](../class/vector4.md)

| Argument | Type | Description |
| :--- | :--- | :--- |
| **x** | number\(float\) | x |
| **y** | number\(float\) | y |
| **z** | number\(float\) | z |
| **w** | number\(float\) | w |

Returns Vector4.



### Math.Vector3 <a id="database-read"></a>

`Math.Vector3(x: number, y: number, z: number)`: [Vector3](../class/vector3.md)

| Argument | Type | Description |
| :--- | :--- | :--- |
| **x** | number\(float\) | x |
| **y** | number\(float\) | y |
| **z** | number\(float\) | z |

Returns Vector3.



### Math.Vector2 <a id="database-read"></a>

`Math.Vector2(x: number, y: number)`: [Vector2](../class/vector2.md)

| Argument | Type | Description |
| :--- | :--- | :--- |
| **x** | number\(float\) | x |
| **y** | number\(float\) | y |

Returns Vector2.



### Math.CatmullRom <a id="database-read"></a>

`Math.CatmullRom(a: Vector2, b: Vector2, c: Vector2, d: Vector2, t:number)`: Vector2

| Argument | Type | Description |
| :--- | :--- | :--- |
| **a** | Vector2 | a |
| **b** | Vector2 | b |
| **c** | Vector2 | c |
| **d** | Vector2 | d |
| t | number\(float） | Weighting factor. |

Returns the result of the Catmull-Rom interpolation.



### Math.GetAngle <a id="database-read"></a>

`Math.GetAngle(a: Vector2, b: Vector2, c:Vector2)`: number

| Argument | Type | Description |
| :--- | :--- | :--- |
| **a** | Vector2 | PA |
| **b** | Vector2 | PB |
| **c** | Vector2 | PC |

Returns angle between ba and bc.



### Math.GetAngleDeg <a id="database-read"></a>

`Math.GetAngleDeg(a: Vector2, b: Vector2, c:Vector2)`: number

| Argument | Type | Description |
| :--- | :--- | :--- |
| **a** | Vector2 | PA |
| **b** | Vector2 | PB |
| **c** | Vector2 | PC |

Returns angle degree between ba and bc \(0-180\).



### Math.GetFullAngleDeg <a id="database-read"></a>

`Math.GetFullAngleDeg(a: Vector2, b: Vector2, c:Vector2)`: number

| Argument | Type | Description |
| :--- | :--- | :--- |
| **a** | Vector2 | PA |
| **b** | Vector2 | PB |
| **c** | Vector2 | PC |

Returns angle degree between ba and bc \(-180-180\).



### Math.LineSegmentIntersection <a id="database-read"></a>

`Math.LineSegmentIntersection(a: Vector2, b: Vector2, c:Vector2, d:Vector2)`: boolean,Vector2

| Argument | Type | Description |
| :--- | :--- | :--- |
| **a** | Vector2 | Line 1 start. |
| **b** | Vector2 | Line 1 end. |
| **c** | Vector2 | Line 2 start |
| d | Vector2 | Line 2 end. |

Returns true if line segment 1 and line segment2 has intersection and intersection point\(if false ,defalut return point a\).



### Math.CircleLineIntersection <a id="database-read"></a>

`Math.CircleLineIntersection(a: Vector2, b: Vector2, c:Vector2, radius:number, onlySegment:boolean)`: \[Vector2\],\[Vector2\]

| Argument | Type | Description |
| :--- | :--- | :--- |
| **a** | Vector2 | Line start. |
| **b** | Vector2 | Line end. |
| **c** | Vector2 | Center. |
| **radius** | number | Circle radius. |
| **onlySegment** | boolean | Only check ab as line segment. |

Returns two Intersection points if exist or else reutrns nil.



### Math.BuildCircle <a id="database-read"></a>

`Math.BuildCircle(center: Vector2, radius:number, quality:number)`: table \(Vector2\)

| Argument | Type | Description |
| :--- | :--- | :--- |
| **center** | Vector2 | Center. |
| **radius** | number | Circle radius. |
| **quality** | number | Circle sides. |

Returns circle points table.



### Math.BuildSafeCircle <a id="database-read"></a>

`Math.BuildSafeCircle(center: Vector2, radius:number, quality:number)`: table \(Vector2\)

| Argument | Type | Description |
| :--- | :--- | :--- |
| **center** | Vector2 | Center. |
| **radius** | number | Circle radius. |
| **quality** | number | Circle sides. |

Returns safe circle points table.

