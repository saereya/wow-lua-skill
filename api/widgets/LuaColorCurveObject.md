# LuaColorCurveObject

Widget methods (`LuaColorCurveObjectAPI`) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/luacolorcurveobjectapidocumentation.lua` (FileDataID 7507385)

## Methods

### AddPoint

```lua
LuaColorCurveObject:AddPoint(x: number, y: colorRGBA)
```

Adds a single point to the curve.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `x` | `number` |  |
| `y` | `colorRGBA` | `Mixin=ColorMixin` |

### ClearPoints

```lua
LuaColorCurveObject:ClearPoints()
```

Removes all points from the curve. Evaluating an empty curve always yields a zero value.

### Copy

```lua
LuaColorCurveObject:Copy() -> curve: LuaColorCurveObject
```

Returns a new copy of this curve.

`ReturnsNeverSecret`

### Evaluate

```lua
LuaColorCurveObject:Evaluate(x: number) -> y: colorRGBA
```

Returns a calculated color value from the configured curve points.

`SecretArguments=AllowedWhenUntainted` `ConstSecretAccessor`

Returns:

| Name | Type | Notes |
|---|---|---|
| `y` | `colorRGBA` | `Mixin=ColorMixin` |

### EvaluateUnpacked

```lua
LuaColorCurveObject:EvaluateUnpacked(x: number) -> yR: number, yG: number, yB: number, yA: number
```

Returns an unpacked calculated color value from the configured curve points.

`SecretArguments=AllowedWhenUntainted` `ConstSecretAccessor`

### GetPoint

```lua
LuaColorCurveObject:GetPoint(index: luaIndex) -> point: LuaColorCurvePoint?
```

Returns the vector for an individual point index on the curve.

`SecretArguments=AllowedWhenUntainted` `ConstSecretAccessor`

### GetPointCount

```lua
LuaColorCurveObject:GetPointCount() -> count: size
```

Returns the total number of points on the curve.

### GetPoints

```lua
LuaColorCurveObject:GetPoints() -> point: LuaColorCurvePoint[]
```

Returns the vectors for all points on the curve.

### RemovePoint

```lua
LuaColorCurveObject:RemovePoint(index: luaIndex)
```

Removes a single point from the curve. Raises an error if the supplied point index is out of range.

`SecretArguments=AllowedWhenUntainted`

### SetPoints

```lua
LuaColorCurveObject:SetPoints(point: LuaColorCurvePoint[])
```

Replaces all points on the curve.

`SecretArguments=AllowedWhenUntainted`

### SetToDefaults

```lua
LuaColorCurveObject:SetToDefaults()
```

Resets all state on the curve, and clears the secret values flag.

## Types

### LuaColorCurvePoint

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `x` | `number` |  |
| `y` | `colorRGBA` | `Mixin=ColorMixin` |
