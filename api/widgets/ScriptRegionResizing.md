# ScriptRegionResizing

Widget methods (`SimpleScriptRegionResizingAPI`) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/simplescriptregionresizingapidocumentation.lua` (FileDataID 4637241)

## Methods

### AdjustPointsOffset

```lua
ScriptRegionResizing:AdjustPointsOffset(x: uiUnit, y: uiUnit)
```

`SecretArguments=AllowedWhenUntainted` `IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

### ClearAllPoints

```lua
ScriptRegionResizing:ClearAllPoints()
```

Clears all points and immediately invalidates the rect. (Prior to 11.2.0, this would only invalidate rect immediately for AnchoringRestricted regions.)

`IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

### ClearPoint

```lua
ScriptRegionResizing:ClearPoint(point: FramePoint)
```

`SecretArguments=AllowedWhenUntainted` `IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

### ClearPointsOffset

```lua
ScriptRegionResizing:ClearPointsOffset()
```

`IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

### GetNumPoints

```lua
ScriptRegionResizing:GetNumPoints() -> numPoints: number
```

### GetPoint

```lua
ScriptRegionResizing:GetPoint(anchorIndex: luaIndex, resolveCollapsed: bool) -> point: FramePoint, relativeTo: ScriptRegion, relativePoint: FramePoint, offsetX: uiUnit, offsetY: uiUnit
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `SecretWhenAnchoringSecret` `ConstSecretAccessor`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `anchorIndex` | `luaIndex` | default `0` |
| `resolveCollapsed` | `bool` | default `false` |

### GetPointByName

```lua
ScriptRegionResizing:GetPointByName(point: FramePoint, resolveCollapsed: bool) -> point: FramePoint, relativeTo: ScriptRegion, relativePoint: FramePoint, offsetX: uiUnit, offsetY: uiUnit
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `SecretWhenAnchoringSecret` `ConstSecretAccessor`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `point` | `FramePoint` |  |
| `resolveCollapsed` | `bool` | default `false` |

### SetAllPoints

```lua
ScriptRegionResizing:SetAllPoints(relativeTo: ScriptRegion, doResize: bool)
```

`SecretArguments=AllowedWhenUntainted` `IsProtectedFunction` `CheckAllowInheritForbiddenLayoutAspects`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

Arguments:

| Name | Type | Notes |
|---|---|---|
| `relativeTo` | `ScriptRegion` |  |
| `doResize` | `bool` | default `true` |

### SetHeight

```lua
ScriptRegionResizing:SetHeight(height: uiUnit)
```

`SecretArguments=AllowedWhenUntainted` `IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

### SetPoint

```lua
ScriptRegionResizing:SetPoint(point: FramePoint, relativeTo: ScriptRegion, relativePoint: FramePoint, offsetX: uiUnit, offsetY: uiUnit)
```

`SecretArguments=AllowedWhenUntainted` `IsProtectedFunction` `CheckAllowInheritForbiddenLayoutAspects`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

### SetPointsOffset

```lua
ScriptRegionResizing:SetPointsOffset(x: uiUnit, y: uiUnit)
```

`SecretArguments=AllowedWhenUntainted` `IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

### SetSize

```lua
ScriptRegionResizing:SetSize(x: uiUnit, y: uiUnit)
```

`SecretArguments=AllowedWhenUntainted` `IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

### SetWidth

```lua
ScriptRegionResizing:SetWidth(width: uiUnit)
```

`SecretArguments=AllowedWhenUntainted` `IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.
