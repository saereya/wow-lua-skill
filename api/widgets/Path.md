# Path

Widget methods (`SimpleAnimPathAPI`) · inherits [`Animation`](Animation.md) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/simpleanimpathapidocumentation.lua` (FileDataID 4637206)

## Methods

### CreateControlPoint

```lua
Path:CreateControlPoint(name: cstring?, templateName: cstring?, order: number?) -> point: SimpleControlPoint
```

`SecretArguments=NotAllowed`

### GetControlPoints

```lua
Path:GetControlPoints() -> points: SimpleControlPoint
```

Returns:

| Name | Type | Notes |
|---|---|---|
| `points` | `SimpleControlPoint` | `StrideIndex=1` |

### GetCurveType

```lua
Path:GetCurveType() -> curveType: CurveType
```

### GetMaxControlPointOrder

```lua
Path:GetMaxControlPointOrder() -> maxOrder: number
```

### SetCurveType

```lua
Path:SetCurveType(curveType: CurveType)
```

`SecretArguments=AllowedWhenUntainted`
