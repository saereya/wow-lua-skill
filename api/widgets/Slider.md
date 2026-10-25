# Slider

Widget methods (`SimpleSliderAPI`) · inherits [`Frame`](Frame.md) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/simplesliderapidocumentation.lua` (FileDataID 4637234)

## Methods

### Disable

```lua
Slider:Disable()
```

### Enable

```lua
Slider:Enable()
```

### GetMinMaxValues

```lua
Slider:GetMinMaxValues() -> minValue: number, maxValue: number
```

### GetObeyStepOnDrag

```lua
Slider:GetObeyStepOnDrag() -> isObeyStepOnDrag: bool
```

### GetOrientation

```lua
Slider:GetOrientation() -> orientation: Orientation
```

### GetStepsPerPage

```lua
Slider:GetStepsPerPage() -> stepsPerPage: number
```

### GetThumbTexture

```lua
Slider:GetThumbTexture() -> texture: SimpleTexture
```

### GetValue

```lua
Slider:GetValue() -> value: number
```

### GetValueStep

```lua
Slider:GetValueStep() -> valueStep: number
```

### IsDraggingThumb

```lua
Slider:IsDraggingThumb() -> isDraggingThumb: bool
```

### IsEnabled

```lua
Slider:IsEnabled() -> enabled: bool
```

### SetEnabled

```lua
Slider:SetEnabled(enabled: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetMinMaxValues

```lua
Slider:SetMinMaxValues(minValue: number, maxValue: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetObeyStepOnDrag

```lua
Slider:SetObeyStepOnDrag(obeyStepOnDrag: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetOrientation

```lua
Slider:SetOrientation(orientation: Orientation)
```

`SecretArguments=AllowedWhenUntainted`

### SetStepsPerPage

```lua
Slider:SetStepsPerPage(stepsPerPage: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetThumbTexture

```lua
Slider:SetThumbTexture(asset: TextureAsset)
```

`SecretArguments=AllowedWhenUntainted` `CheckAllowChangeParent`

### SetValue

```lua
Slider:SetValue(value: number, treatAsMouseEvent: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `value` | `number` |  |
| `treatAsMouseEvent` | `bool` | default `false` |

### SetValueStep

```lua
Slider:SetValueStep(valueStep: number)
```

`SecretArguments=AllowedWhenUntainted`
