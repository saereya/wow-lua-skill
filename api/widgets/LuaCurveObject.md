# LuaCurveObject

Widget methods (`LuaCurveObjectAPI`) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/luacurveobjectapidocumentation.lua` (FileDataID 7507384)

## Methods

### AddPoint

```lua
LuaCurveObject:AddPoint(pointX: number, pointY: number)
```

Adds a single point to the curve.

`SecretArguments=AllowedWhenUntainted`

### ClearPoints

```lua
LuaCurveObject:ClearPoints()
```

Removes all points from the curve. Evaluating an empty curve always yields a zero value.

### Copy

```lua
LuaCurveObject:Copy() -> curve: LuaCurveObject
```

Returns a new copy of this curve.

`ReturnsNeverSecret`

### Evaluate

```lua
LuaCurveObject:Evaluate(x: number) -> y: number
```

Returns a calculated 'y' value from the configured curve points.

`SecretArguments=AllowedWhenUntainted` `ConstSecretAccessor`

### GetPoint

```lua
LuaCurveObject:GetPoint(index: luaIndex) -> point: vector2?
```

Returns the vector for an individual point index on the curve.

`SecretArguments=AllowedWhenUntainted` `ConstSecretAccessor`

Returns:

| Name | Type | Notes |
|---|---|---|
| `point` | `vector2?` | `Mixin=Vector2DMixin` |

### GetPointCount

```lua
LuaCurveObject:GetPointCount() -> count: size
```

Returns the total number of points on the curve.

### GetPoints

```lua
LuaCurveObject:GetPoints() -> point: vector2[]
```

Returns the vectors for all points on the curve.

### RemovePoint

```lua
LuaCurveObject:RemovePoint(index: luaIndex)
```

Removes a single point from the curve. Raises an error if the supplied point index is out of range.

`SecretArguments=AllowedWhenUntainted`

### SetPoints

```lua
LuaCurveObject:SetPoints(point: vector2[])
```

Replaces all points on the curve.

`SecretArguments=AllowedWhenUntainted`

### SetToDefaults

```lua
LuaCurveObject:SetToDefaults()
```

Resets all state on the curve, and clears the secret values flag.
