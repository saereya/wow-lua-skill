# ColorOverrides

Namespace `C_ColorOverrides` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/coloroverridesdocumentation.lua` (FileDataID 6725188)

## Functions

### ClearColorOverrides

```lua
C_ColorOverrides.ClearColorOverrides()
```

### GetColorForQuality

```lua
C_ColorOverrides.GetColorForQuality(quality: ItemQuality) -> color: colorRGBA
```

`SecretArguments=AllowedWhenUntainted`

Returns:

| Name | Type | Notes |
|---|---|---|
| `color` | `colorRGBA` | `Mixin=ColorMixin` |

### GetColorOverrideInfo

```lua
C_ColorOverrides.GetColorOverrideInfo(overrideType: ColorOverride) -> overrideInfo: ColorOverrideInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetDefaultColorForQuality

```lua
C_ColorOverrides.GetDefaultColorForQuality(quality: ItemQuality) -> color: colorRGBA
```

`SecretArguments=AllowedWhenUntainted`

Returns:

| Name | Type | Notes |
|---|---|---|
| `color` | `colorRGBA` | `Mixin=ColorMixin` |

### RemoveColorOverride

```lua
C_ColorOverrides.RemoveColorOverride(overrideType: ColorOverride)
```

`SecretArguments=AllowedWhenUntainted`

### SetColorOverride

```lua
C_ColorOverrides.SetColorOverride(overrideType: ColorOverride, color: colorRGBA)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `overrideType` | `ColorOverride` |  |
| `color` | `colorRGBA` | `Mixin=ColorMixin` |

## Events

### COLOR_OVERRIDES_RESET

```lua
COLOR_OVERRIDES_RESET()
```

`SynchronousEvent`

### COLOR_OVERRIDE_UPDATED

```lua
COLOR_OVERRIDE_UPDATED(overrideType: ColorOverride)
```

`SynchronousEvent`

## Types

### ColorOverrideInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `overrideType` | `ColorOverride` |  |
| `overrideColor` | `colorRGB` | `Mixin=ColorMixin` |
| `overrideColorString` | `string` |  |
