---
description: Vector4 class
---

# Vector4

## property:

* `x`\(number\)
* `y`\(number\)
* `z`\(number\)
* `w`\(number\)

## Functions:

### :Copy

`vector4:Copy()`: Vector4

Returns a Vector4 \(x =x, y =y, z=z, w=w\).



### :Length

`vector4:Length()`: number

Returns vector length.



### :Length2

`vector4:Length2()`: number

Returns vector length **square**.



### :Distance <a id="database-read"></a>

`vector4:Distance(v2: Vector4)`: number

| Argument | Type | Description |
| :--- | :--- | :--- |
| **v2** | Vector4 | Point2. |

Returns distance from v to v2.



### :Distance2 <a id="database-read"></a>

`vector3:Distance(v2: Vector4)`: number

| Argument | Type | Description |
| :--- | :--- | :--- |
| **v2** | Vector4 | Point2. |

Returns distance **square** from v to v2.



### :Dot <a id="database-read"></a>

`vector2:Dot(v2: Vector4)`: number

| Argument | Type | Description |
| :--- | :--- | :--- |
| **v2** | Vector4 | Point2. |

Returns dot product result.



### :Normalize

`vector4:Normalize()`: Vector4

Returns a normalized Vector4 from this vector.



### :Lerp <a id="database-read"></a>

`vector4:Lerp(v2: Vector4, time: number)`: Vector3

| Argument | Type | Description |
| :--- | :--- | :--- |
| **v2** | Vector4 | Point2. |
| **time** | number\(float\) | Time. |

Returns Linear interpolation. V1 + s \(V2-V1\)



### :Unpack

`vector4:Unpack()`: number, number,number,number

Returns two numbers x,y.z,w



### :Randomize

`vector4:Randomize()`: Vector4

Randomizes vector a little.



