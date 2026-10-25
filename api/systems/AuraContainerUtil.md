# AuraContainerUtil

Namespace `C_AuraContainerUtil` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/auracontainerutildocumentation.lua` (FileDataID 8245097)

## Functions

### ProcessAuraTooltipBackdropOptions

```lua
C_AuraContainerUtil.ProcessAuraTooltipBackdropOptions(options: AuraContainerTooltipBackdropOptions) -> result: AuraContainerTooltipBackdropOptions
```

`SecretArguments=AllowedWhenUntainted`

### ProcessAuraTooltipNineSliceOptions

```lua
C_AuraContainerUtil.ProcessAuraTooltipNineSliceOptions(options: AuraContainerTooltipNineSliceOptions) -> result: AuraContainerTooltipNineSliceOptions
```

`SecretArguments=AllowedWhenUntainted`

### ProcessAuraTooltipTextureSliceOptions

```lua
C_AuraContainerUtil.ProcessAuraTooltipTextureSliceOptions(options: AuraContainerTooltipTextureSliceOptions) -> result: AuraContainerTooltipTextureSliceOptions
```

`SecretArguments=AllowedWhenUntainted`

### ProcessCustomAuraButtonApplicationBarOptions

```lua
C_AuraContainerUtil.ProcessCustomAuraButtonApplicationBarOptions(options: CustomAuraButtonApplicationBarOptions) -> result: CustomAuraButtonApplicationBarOptions
```

`SecretArguments=AllowedWhenUntainted`

### ProcessCustomAuraButtonApplicationCountOptions

```lua
C_AuraContainerUtil.ProcessCustomAuraButtonApplicationCountOptions(options: CustomAuraButtonApplicationCountOptions?) -> result: CustomAuraButtonApplicationCountOptions
```

`SecretArguments=AllowedWhenUntainted`

### ProcessCustomAuraButtonCasterNameOptions

```lua
C_AuraContainerUtil.ProcessCustomAuraButtonCasterNameOptions(options: CustomAuraButtonCasterNameOptions?) -> result: CustomAuraButtonCasterNameOptions
```

`SecretArguments=AllowedWhenUntainted`

### ProcessCustomAuraButtonDispelTypeTextOptions

```lua
C_AuraContainerUtil.ProcessCustomAuraButtonDispelTypeTextOptions(options: CustomAuraButtonDispelTypeTextOptions?) -> result: CustomAuraButtonDispelTypeTextOptions
```

`SecretArguments=AllowedWhenUntainted`

### ProcessCustomAuraButtonDispelTypeTextureOptions

```lua
C_AuraContainerUtil.ProcessCustomAuraButtonDispelTypeTextureOptions(options: CustomAuraButtonDispelTypeTextureOptions?) -> result: CustomAuraButtonDispelTypeTextureOptions
```

`SecretArguments=AllowedWhenUntainted`

### ProcessCustomAuraButtonDurationBarOptions

```lua
C_AuraContainerUtil.ProcessCustomAuraButtonDurationBarOptions(options: CustomAuraButtonDurationBarOptions?) -> result: CustomAuraButtonDurationBarOptions
```

`SecretArguments=AllowedWhenUntainted`

### ProcessCustomAuraButtonDurationTextOptions

```lua
C_AuraContainerUtil.ProcessCustomAuraButtonDurationTextOptions(options: CustomAuraButtonDurationTextOptions?) -> result: CustomAuraButtonDurationTextOptions
```

`SecretArguments=AllowedWhenUntainted`

## Types

### AuraContainerTooltipAnchorOffsets

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `left` | `number` | default `0` |
| `right` | `number` | default `0` |
| `top` | `number` | default `0` |
| `bottom` | `number` | default `0` |

### AuraContainerTooltipBackdropInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `bgFile` | `TextureAssetDisk?` | Optional background texture asset. |
| `edgeFile` | `TextureAssetDisk?` | Optional edge texture asset. |
| `edgeSize` | `number?` | Optional edge size. |
| `insets` | `AuraContainerTooltipBackdropInsets?` | Optional backdrop insets. |
| `tile` | `bool?` | If true, tiles the background texture. |
| `tileEdge` | `bool?` | If true, tiles the edge texture. |
| `tileSize` | `number?` | Optional tile size used when tiling the background texture. |

### AuraContainerTooltipBackdropInsets

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `left` | `number` | default `0` |
| `right` | `number` | default `0` |
| `top` | `number` | default `0` |
| `bottom` | `number` | default `0` |

### AuraContainerTooltipBackdropOptions

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `backdropInfo` | `AuraContainerTooltipBackdropInfo` | Backdrop information used to construct the tooltip backdrop. |
| `borderColor` | `colorRGBA?` | Optional color applied to the backdrop border.; `Mixin=ColorMixin` |
| `centerColor` | `colorRGBA?` | Optional color applied to the backdrop background.; `Mixin=ColorMixin` |
| `anchorOffsets` | `AuraContainerTooltipAnchorOffsets?` | Optional offsets applied to the backdrop's TOPLEFT and BOTTOMRIGHT anchor points. |

### AuraContainerTooltipNineSliceOptions

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `layoutName` | `cstring` | Name of the NineSlice layout template to apply, such as 'TooltipDefaultLayout'. |
| `borderColor` | `colorRGBA?` | Optional color applied to the NineSlice border.; `Mixin=ColorMixin` |
| `centerColor` | `colorRGBA?` | Optional color applied to the NineSlice center region.; `Mixin=ColorMixin` |
| `anchorOffsets` | `AuraContainerTooltipAnchorOffsets?` | Optional offsets applied to the NineSlice's TOPLEFT and BOTTOMRIGHT anchor points. |

### AuraContainerTooltipTextureSliceOptions

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `asset` | `TextureAssetDisk` | Texture asset (file path or atlas name) displayed by the slice. |
| `sliceMargins` | `UITextureSliceMargins?` | Optional texture slice margins. See Texture:SetTextureSliceMargins. |
| `sliceMode` | `UITextureSliceMode?` | Optional texture slice mode. See Texture:SetTextureSliceMode. |
| `color` | `colorRGBA?` | Optional vertex color applied to the texture.; `Mixin=ColorMixin` |
| `anchorOffsets` | `AuraContainerTooltipAnchorOffsets?` | Optional offsets applied to the slice's TOPLEFT and BOTTOMRIGHT anchor points. |
| `drawLayer` | `DrawLayer?` | Draw layer used when displaying the texture. |
| `drawLayerSublevel` | `number` | default `0`; Draw layer sublevel used when displaying the texture. |

### CustomAuraButtonApplicationBarOptions

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `maxApplications` | `number` | The maximum number of aura applications represented by the bar. |
| `minApplications` | `number` | default `0`; The minimum number of aura applications represented by the bar. |
| `interpolation` | `StatusBarInterpolation?` | Optional interpolation method used when updating the bar value. |

### CustomAuraButtonApplicationCountOptions

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `formatter` | `NumericFormatter?` | Optional formatter used to display aura application counts. |

### CustomAuraButtonCasterNameOptions

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `showRealmName` | `bool` | default `false`; If true, append realm names to the displayed string. |
| `useClassColors` | `bool` | default `false`; If true, apply class coloring to the text. |

### CustomAuraButtonDispelTypeTextOptions

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `showWhenHarmful` | `bool` | default `true`; Shows the dispel type text for harmful auras. |
| `showWhenHelpful` | `bool` | default `false`; Shows the dispel type text for helpful auras. |
| `showWithoutDispelType` | `bool` | default `false`; Shows the dispel type text for auras that do not have a dispel type. |
| `customDispelTextMap` | `table<string, stringView>?` | Optional map of dispel type names to custom texts. An empty key can be used for auras without a dispel type. |

### CustomAuraButtonDispelTypeTextureAsset

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `asset` | `TextureAssetDisk` | The texture file or atlas to use. |
| `useAtlasSize` | `bool` | default `false`; Resizes the texture to the atlas dimensions. Ignored when asset does not name an atlas. |
| `texCoords` | `CustomAuraButtonDispelTypeTextureTexCoords?` | Optional texture coordinates used when asset does not name an atlas. |

### CustomAuraButtonDispelTypeTextureOptions

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `showAlways` | `bool` | default `false`; Shows the dispel type texture always, ignoring all other criteria. |
| `showWhenHarmful` | `bool` | default `true`; Shows the dispel type texture for harmful auras. |
| `showWhenHelpful` | `bool` | default `false`; Shows the dispel type texture for helpful auras. |
| `showWithoutDispelType` | `bool` | default `false`; Shows the dispel type texture for auras that do not have a dispel type. |
| `stealableFilter` | `CustomAuraButtonDispelTypeStealableFilter?` | Restricts display of the dispel type texture to either stealable or non-stealable auras. If omitted, the dispel type texture may be shown for both. |
| `style` | `CustomAuraButtonDispelTypeTextureStyle` | default `"BorderWithIcon"`; The texture style to use. |
| `customDispelAssetMap` | `table<string, CustomAuraButtonDispelTypeTextureAsset>?` | Optional map of dispel type names to custom texture assets. The "None" key represents auras without a dispel type. Only applies when using the CustomAsset style. |
| `customDispelColorMap` | `table<string, colorRGB>?` | Optional map of dispel type names to custom vertex colors. The "None" key represents auras without a dispel type. |
| `customDispelColorCurve` | `LuaColorCurveObject?` | Optional curve used to determine vertex colors from the aura's dispel type. |

### CustomAuraButtonDispelTypeTextureTexCoords

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `left` | `number` | default `0` |
| `right` | `number` | default `1` |
| `top` | `number` | default `0` |
| `bottom` | `number` | default `1` |

### CustomAuraButtonDurationBarOptions

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `interpolation` | `StatusBarInterpolation?` | The interpolation method used when updating the duration bar. |
| `direction` | `StatusBarTimerDirection?` | The direction in which the duration bar progresses. |

### CustomAuraButtonDurationTextOptions

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `binding` | `DurationTextBinding?` | Optional duration text binding to use. The binding is copied before being associated with the aura button. |
| `textFormatter` | `NumericFormatter?` | Optional formatter used to display remaining duration values. Ignored if textFormat is specified. |
| `textFormat` | `DurationTextBindingFormatOptions?` | Optional text format configuration applied to the duration text binding. Overrides textFormatter when specified. |
| `textColor` | `DurationTextBindingColorOptions?` | Optional text color configuration applied to the duration text binding. |
