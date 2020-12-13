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

