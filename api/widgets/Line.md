# Line

Widget methods (`SimpleLineAPI`) · inherits [`TextureBase`](TextureBase.md) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/simplelineapidocumentation.lua` (FileDataID 4637221)

## Methods

### ClearAllPoints

```lua
Line:ClearAllPoints()
```

`IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

### GetEndPoint

```lua
Line:GetEndPoint() -> relativePoint: FramePoint, relativeTo: ScriptRegion, offsetX: uiUnit, offsetY: uiUnit
```

### GetHitRectThickness

```lua
Line:GetHitRectThickness() -> thickness: uiUnit
```

### GetStartPoint

```lua
Line:GetStartPoint() -> relativePoint: FramePoint, relativeTo: ScriptRegion, offsetX: uiUnit, offsetY: uiUnit
```

### GetThickness

```lua
Line:GetThickness() -> thickness: uiUnit
```

### SetEndPoint

```lua
Line:SetEndPoint(relativePoint: FramePoint, relativeTo: ScriptRegion, offsetX: uiUnit, offsetY: uiUnit)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `relativePoint` | `FramePoint` |  |
| `relativeTo` | `ScriptRegion` |  |
| `offsetX` | `uiUnit` | default `0` |
| `offsetY` | `uiUnit` | default `0` |

### SetHitRectThickness

```lua
Line:SetHitRectThickness(thickness: uiUnit)
```

`SecretArguments=AllowedWhenUntainted`

### SetStartPoint

```lua
Line:SetStartPoint(relativePoint: FramePoint, relativeTo: ScriptRegion, offsetX: uiUnit, offsetY: uiUnit)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `relativePoint` | `FramePoint` |  |
| `relativeTo` | `ScriptRegion` |  |
| `offsetX` | `uiUnit` | default `0` |
| `offsetY` | `uiUnit` | default `0` |

### SetThickness

```lua
Line:SetThickness(thickness: uiUnit)
```

`SecretArguments=AllowedWhenUntainted`
