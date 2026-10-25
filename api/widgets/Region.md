# Region

Widget methods (`SimpleRegionAPI`) · inherits [`ScriptRegion`](ScriptRegion.md) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/simpleregionapidocumentation.lua` (FileDataID 4637228)

## Methods

### GetAlpha

```lua
Region:GetAlpha() -> alpha: SingleColorValue
```

`SecretReturnsForAspect={ Enum.SecretAspect.Alpha }`

### GetDrawLayer

```lua
Region:GetDrawLayer() -> layer: DrawLayer, sublayer: number
```

### GetEffectiveScale

```lua
Region:GetEffectiveScale() -> effectiveScale: number
```

`SecretReturnsForAspect={ Enum.SecretAspect.Scale }`

### GetScale

```lua
Region:GetScale() -> scale: number
```

`SecretReturnsForAspect={ Enum.SecretAspect.Scale }`

### GetVertexColor

```lua
Region:GetVertexColor() -> colorR: number, colorG: number, colorB: number, colorA: number
```

`MayReturnNothing` `SecretReturnsForAspect={ Enum.SecretAspect.VertexColor, Enum.SecretAspect.Alpha }`

### IsIgnoringParentAlpha

```lua
Region:IsIgnoringParentAlpha() -> isIgnoring: bool
```

### IsIgnoringParentScale

```lua
Region:IsIgnoringParentScale() -> isIgnoring: bool
```

### IsObjectLoaded

```lua
Region:IsObjectLoaded() -> isLoaded: bool
```

### SetAlpha

```lua
Region:SetAlpha(alpha: SingleColorValue)
```

`SecretArguments=AllowedWhenTainted` `SecretArgumentsAddAspect={ Enum.SecretAspect.Alpha }`

### SetAlphaFromBoolean

```lua
Region:SetAlphaFromBoolean(value: bool, alphaIfTrue: SingleColorValue, alphaIfFalse: SingleColorValue)
```

`SecretArguments=AllowedWhenTainted` `SecretArgumentsAddAspect={ Enum.SecretAspect.Alpha }`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `value` | `bool` |  |
| `alphaIfTrue` | `SingleColorValue` | default `255` |
| `alphaIfFalse` | `SingleColorValue` | default `0` |

### SetDrawLayer

```lua
Region:SetDrawLayer(layer: DrawLayer, sublevel: number)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `layer` | `DrawLayer` |  |
| `sublevel` | `number` | default `0` |

### SetIgnoreParentAlpha

```lua
Region:SetIgnoreParentAlpha(ignore: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetIgnoreParentScale

```lua
Region:SetIgnoreParentScale(ignore: bool)
```

`SecretArguments=NotAllowed` `IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

### SetScale

```lua
Region:SetScale(scale: number)
```

`SecretArguments=AllowedWhenUntainted` `IsProtectedFunction` `SecretArgumentsAddAspect={ Enum.SecretAspect.Scale }`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

### SetVertexColor

```lua
Region:SetVertexColor(colorR: number, colorG: number, colorB: number, a: SingleColorValue?)
```

`SecretArguments=AllowedWhenTainted` `SecretArgumentsAddAspect={ Enum.SecretAspect.VertexColor, Enum.SecretAspect.Alpha }`

### SetVertexColorFromBoolean

```lua
Region:SetVertexColorFromBoolean(value: bool, colorIfTrue: colorRGBA, colorIfFalse: colorRGBA)
```

`SecretArguments=AllowedWhenTainted` `SecretArgumentsAddAspect={ Enum.SecretAspect.VertexColor, Enum.SecretAspect.Alpha }`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `value` | `bool` |  |
| `colorIfTrue` | `colorRGBA` | `Mixin=ColorMixin` |
| `colorIfFalse` | `colorRGBA` | `Mixin=ColorMixin` |
