# StatusBar

Widget methods (`SimpleStatusBarAPI`) · inherits [`Frame`](Frame.md) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/simplestatusbarapidocumentation.lua` (FileDataID 4637240)

## Methods

### GetFillStyle

```lua
StatusBar:GetFillStyle() -> fillStyle: StatusBarFillStyle
```

### GetInterpolatedValue

```lua
StatusBar:GetInterpolatedValue() -> value: number
```

Returns the current interpolated value displayed by the bar.

`SecretReturnsForAspect={ Enum.SecretAspect.BarValue }`

### GetMinMaxValues

```lua
StatusBar:GetMinMaxValues() -> minValue: number, maxValue: number
```

`SecretReturnsForAspect={ Enum.SecretAspect.BarValue }`

### GetOrientation

```lua
StatusBar:GetOrientation() -> orientation: Orientation
```

### GetRenderMode

```lua
StatusBar:GetRenderMode() -> renderMode: StatusBarRenderMode
```

### GetReverseFill

```lua
StatusBar:GetReverseFill() -> isReverseFill: bool
```

### GetRotatesTexture

```lua
StatusBar:GetRotatesTexture() -> rotatesTexture: bool
```

### GetStatusBarColor

```lua
StatusBar:GetStatusBarColor() -> colorR: number, colorG: number, colorB: number, colorA: number
```

`SecretReturnsForAspect={ Enum.SecretAspect.VertexColor, Enum.SecretAspect.Alpha }`

### GetStatusBarDesaturation

```lua
StatusBar:GetStatusBarDesaturation() -> desaturation: normalizedValue
```

`SecretReturnsForAspect={ Enum.SecretAspect.Desaturation }`

### GetStatusBarTexture

```lua
StatusBar:GetStatusBarTexture() -> texture: SimpleTexture
```

### GetTimerDuration

```lua
StatusBar:GetTimerDuration() -> duration: LuaDurationObject
```

### GetValue

```lua
StatusBar:GetValue() -> value: number
```

`SecretReturnsForAspect={ Enum.SecretAspect.BarValue }`

### IsInterpolating

```lua
StatusBar:IsInterpolating() -> isInterpolating: bool
```

Returns true if the status bar is currently interpolating toward a target value.

`SecretReturnsForAspect={ Enum.SecretAspect.BarValue }`

### IsStatusBarDesaturated

```lua
StatusBar:IsStatusBarDesaturated() -> desaturated: bool
```

`RequiresStatusBarDesaturationAccess` `SecretReturnsForAspect={ Enum.SecretAspect.Desaturation }`

### SetColorFill

```lua
StatusBar:SetColorFill(colorR: number, colorG: number, colorB: number, a: SingleColorValue?)
```

`SecretArguments=AllowedWhenUntainted`

### SetFillStyle

```lua
StatusBar:SetFillStyle(fillStyle: StatusBarFillStyle)
```

`SecretArguments=AllowedWhenUntainted`

### SetMinMaxValues

```lua
StatusBar:SetMinMaxValues(minValue: number, maxValue: number, interpolation: StatusBarInterpolation)
```

`SecretArguments=AllowedWhenTainted` `SecretArgumentsAddAspect={ Enum.SecretAspect.BarValue }`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `minValue` | `number` |  |
| `maxValue` | `number` |  |
| `interpolation` | `StatusBarInterpolation` | default `"Immediate"`; `NeverSecret` |

### SetOrientation

```lua
StatusBar:SetOrientation(orientation: Orientation)
```

`SecretArguments=AllowedWhenUntainted`

### SetRenderMode

```lua
StatusBar:SetRenderMode(renderMode: StatusBarRenderMode)
```

`SecretArguments=AllowedWhenUntainted`

### SetReverseFill

```lua
StatusBar:SetReverseFill(isReverseFill: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetRotatesTexture

```lua
StatusBar:SetRotatesTexture(rotatesTexture: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetStatusBarColor

```lua
StatusBar:SetStatusBarColor(colorR: number, colorG: number, colorB: number, a: SingleColorValue?)
```

`SecretArguments=AllowedWhenTainted` `SecretArgumentsAddAspect={ Enum.SecretAspect.VertexColor, Enum.SecretAspect.Alpha }`

### SetStatusBarDesaturated

```lua
StatusBar:SetStatusBarDesaturated(desaturated: bool)
```

`SecretArguments=AllowedWhenTainted` `SecretArgumentsAddAspect={ Enum.SecretAspect.Desaturation }`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `desaturated` | `bool` | default `false` |

### SetStatusBarDesaturation

```lua
StatusBar:SetStatusBarDesaturation(desaturation: normalizedValue)
```

`SecretArguments=AllowedWhenTainted` `SecretArgumentsAddAspect={ Enum.SecretAspect.Desaturation }`

### SetStatusBarTexture

```lua
StatusBar:SetStatusBarTexture(asset: TextureAsset) -> success: bool
```

`SecretArguments=AllowedWhenUntainted` `CheckAllowChangeParent`

### SetTimerDuration

```lua
StatusBar:SetTimerDuration(duration: LuaDurationObject, interpolation: StatusBarInterpolation, direction: StatusBarTimerDirection)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `duration` | `LuaDurationObject` |  |
| `interpolation` | `StatusBarInterpolation` | default `"Immediate"` |
| `direction` | `StatusBarTimerDirection` | default `"ElapsedTime"` |

### SetToTargetValue

```lua
StatusBar:SetToTargetValue()
```

Immediately finishes any interpolation of the bar and snaps it to the target value.

### SetValue

```lua
StatusBar:SetValue(value: number, interpolation: StatusBarInterpolation)
```

`SecretArguments=AllowedWhenTainted` `SecretArgumentsAddAspect={ Enum.SecretAspect.BarValue }`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `value` | `number` |  |
| `interpolation` | `StatusBarInterpolation` | default `"Immediate"`; `NeverSecret` |
