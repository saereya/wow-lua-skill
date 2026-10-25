# CurveUtil

Namespace `C_CurveUtil` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/curveutildocumentation.lua` (FileDataID 7507386)

## Functions

### CreateColorCurve

```lua
C_CurveUtil.CreateColorCurve() -> curve: LuaColorCurveObject
```

Returns a new color curve object with no assigned points.

### CreateCurve

```lua
C_CurveUtil.CreateCurve() -> curve: LuaCurveObject
```

Returns a new curve object with no assigned points.

### EvaluateColorFromBoolean

```lua
C_CurveUtil.EvaluateColorFromBoolean(boolean: bool, valueIfTrue: colorRGBA, valueIfFalse: colorRGBA) -> value: colorRGBA
```

Evaluates a potentially-secret boolean value and returns a color.

`SecretArguments=AllowedWhenTainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `boolean` | `bool` |  |
| `valueIfTrue` | `colorRGBA` | `Mixin=ColorMixin` |
| `valueIfFalse` | `colorRGBA` | `Mixin=ColorMixin` |

Returns:

| Name | Type | Notes |
|---|---|---|
| `value` | `colorRGBA` | `Mixin=ColorMixin` |

### EvaluateColorValueFromBoolean

```lua
C_CurveUtil.EvaluateColorValueFromBoolean(boolean: bool, valueIfTrue: SingleColorValue, valueIfFalse: SingleColorValue) -> value: SingleColorValue
```

Evaluates a potentially-secret boolean value and returns a single color component (eg. alpha).

`SecretArguments=AllowedWhenTainted`

### EvaluateGameCurve

```lua
C_CurveUtil.EvaluateGameCurve(curveID: number, x: number) -> y: number
```

`SecretArguments=AllowedWhenUntainted`
