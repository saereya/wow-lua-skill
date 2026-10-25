# TextureBase

Widget methods (`SimpleTextureBaseAPI`) · inherits [`Region`](Region.md) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/simpletexturebaseapidocumentation.lua` (FileDataID 4637238)

## Methods

### ClearRadialProgressBar

```lua
TextureBase:ClearRadialProgressBar()
```

Disable radial progress bar rendering and restore standard texture display.

### ClearSVG

```lua
TextureBase:ClearSVG()
```

### ClearTextureSlice

```lua
TextureBase:ClearTextureSlice()
```

Disable shader based nineslice texture rendering. Since SetAtlas will automatically load slice data for the atlas from the DB, can be useful if you want to disable nineslice after setting an atlas.

### ClearVertexOffsets

```lua
TextureBase:ClearVertexOffsets()
```

### GetAtlas

```lua
TextureBase:GetAtlas() -> atlas: textureAtlas
```

### GetBlendMode

```lua
TextureBase:GetBlendMode() -> blendMode: BlendMode
```

### GetDesaturation

```lua
TextureBase:GetDesaturation() -> desaturation: normalizedValue
```

`SecretReturnsForAspect={ Enum.SecretAspect.Desaturation }`

### GetHorizTile

```lua
TextureBase:GetHorizTile() -> tiling: bool
```

### GetRadialProgressBarEndOffset

```lua
TextureBase:GetRadialProgressBarEndOffset() -> offset: normalizedValue
```

Returns the end angle offset of the radial progress bar as a normalized value (0 to 1).

### GetRadialProgressBarFeather

```lua
TextureBase:GetRadialProgressBarFeather() -> feather: normalizedValue
```

Returns the feather/blur amount applied to the radial progress bar edge.

### GetRadialProgressBarPercent

```lua
TextureBase:GetRadialProgressBarPercent() -> percent: normalizedValue
```

Returns the fill percentage of the radial progress bar (0 to 1).

`SecretReturnsForAspect={ Enum.SecretAspect.RadialProgress }`

### GetRadialProgressBarReverse

```lua
TextureBase:GetRadialProgressBarReverse() -> reverse: bool
```

Returns whether the radial progress bar fills in reverse (counterclockwise) direction.

### GetRadialProgressBarStartOffset

```lua
TextureBase:GetRadialProgressBarStartOffset() -> offset: normalizedValue
```

Returns the start angle offset of the radial progress bar as a normalized value (0 to 1).

### GetRotation

```lua
TextureBase:GetRotation() -> radians: number, normalizedRotationPoint: vector2
```

`SecretReturnsForAspect={ Enum.SecretAspect.Rotation }`

Returns:

| Name | Type | Notes |
|---|---|---|
| `radians` | `number` |  |
| `normalizedRotationPoint` | `vector2` | `Mixin=Vector2DMixin` |

### GetTexCoord

```lua
TextureBase:GetTexCoord() -> ulX: number, ulY: number, llX: number, llY: number, urX: number, urY: number, lrX: number, lrY: number
```

`SecretReturnsForAspect={ Enum.SecretAspect.TexCoords }`

### GetTexelSnappingBias

```lua
TextureBase:GetTexelSnappingBias() -> bias: normalizedValue
```

### GetTexture

```lua
TextureBase:GetTexture() -> textureFile: cstring?
```

### GetTextureFileID

```lua
TextureBase:GetTextureFileID() -> textureFile: fileID
```

### GetTextureFilePath

```lua
TextureBase:GetTextureFilePath() -> textureFile: cstring?
```

### GetTextureSliceMargins

```lua
TextureBase:GetTextureSliceMargins() -> left: number, top: number, right: number, bottom: number
```

`MayReturnNothing`

### GetTextureSliceMode

```lua
TextureBase:GetTextureSliceMode() -> sliceMode: UITextureSliceMode
```

`MayReturnNothing`

### GetVertexOffset

```lua
TextureBase:GetVertexOffset(vertexIndex: luaIndex) -> offsetX: uiUnit, offsetY: uiUnit
```

`SecretArguments=AllowedWhenUntainted` `ConstSecretAccessor`

### GetVertTile

```lua
TextureBase:GetVertTile() -> tiling: bool
```

### IsBlockingLoadRequested

```lua
TextureBase:IsBlockingLoadRequested() -> blocking: bool
```

### IsDesaturated

```lua
TextureBase:IsDesaturated() -> desaturated: bool
```

`RequiresScriptObjectDesaturationAccess` `SecretReturnsForAspect={ Enum.SecretAspect.Desaturation }`

### IsSnappingToPixelGrid

```lua
TextureBase:IsSnappingToPixelGrid() -> snap: bool
```

### ResetTexCoord

```lua
TextureBase:ResetTexCoord()
```

### SetAtlas

```lua
TextureBase:SetAtlas(atlas: textureAtlas, useAtlasSize: bool, filterMode: FilterMode?, resetTexCoords: bool?, wrapModeHorizontal: cstring?, wrapModeVertical: cstring?)
```

`SecretArguments=AllowedWhenTainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `atlas` | `textureAtlas` |  |
| `useAtlasSize` | `bool` | default `false`; `NeverSecret` |
| `filterMode` | `FilterMode?` | `NeverSecret` |
| `resetTexCoords` | `bool?` | `NeverSecret` |
| `wrapModeHorizontal` | `cstring?` | `NeverSecret` |
| `wrapModeVertical` | `cstring?` | `NeverSecret` |

### SetBlendMode

```lua
TextureBase:SetBlendMode(blendMode: BlendMode)
```

`SecretArguments=AllowedWhenUntainted`

### SetBlockingLoadsRequested

```lua
TextureBase:SetBlockingLoadsRequested(blocking: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `blocking` | `bool` | default `false` |

### SetColorTexture

```lua
TextureBase:SetColorTexture(colorR: number, colorG: number, colorB: number, a: SingleColorValue?)
```

`SecretArguments=AllowedWhenTainted`

### SetDesaturated

```lua
TextureBase:SetDesaturated(desaturated: bool)
```

`SecretArguments=AllowedWhenTainted` `SecretArgumentsAddAspect={ Enum.SecretAspect.Desaturation }`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `desaturated` | `bool` | default `false` |

### SetDesaturation

```lua
TextureBase:SetDesaturation(desaturation: normalizedValue)
```

`SecretArguments=AllowedWhenTainted` `SecretArgumentsAddAspect={ Enum.SecretAspect.Desaturation }`

### SetGradient

```lua
TextureBase:SetGradient(orientation: Orientation, minColor: colorRGBA, maxColor: colorRGBA)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `orientation` | `Orientation` |  |
| `minColor` | `colorRGBA` | `Mixin=ColorMixin` |
| `maxColor` | `colorRGBA` | `Mixin=ColorMixin` |

### SetHorizTile

```lua
TextureBase:SetHorizTile(tiling: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `tiling` | `bool` | default `false` |

### SetMask

```lua
TextureBase:SetMask(file: cstring)
```

`SecretArguments=AllowedWhenUntainted`

### SetRadialProgressBarEndOffset

```lua
TextureBase:SetRadialProgressBarEndOffset(offset: normalizedValue)
```

Sets the end angle offset of the radial progress bar as a normalized value (0 to 1).

`SecretArguments=AllowedWhenUntainted`

### SetRadialProgressBarFeather

```lua
TextureBase:SetRadialProgressBarFeather(feather: normalizedValue)
```

Sets the feather/blur amount applied to the radial progress bar edge (higher = more gradual falloff).

`SecretArguments=AllowedWhenUntainted`

### SetRadialProgressBarPercent

```lua
TextureBase:SetRadialProgressBarPercent(percent: normalizedValue)
```

Sets the fill percentage of the radial progress bar (0 to 1).

`SecretArguments=AllowedWhenTainted` `SecretArgumentsAddAspect={ Enum.SecretAspect.RadialProgress }`

### SetRadialProgressBarReverse

```lua
TextureBase:SetRadialProgressBarReverse(reverse: bool)
```

Sets whether the radial progress bar fills in reverse (counterclockwise) direction.

`SecretArguments=AllowedWhenUntainted`

### SetRadialProgressBarStartOffset

```lua
TextureBase:SetRadialProgressBarStartOffset(offset: normalizedValue)
```

Sets the start angle offset of the radial progress bar as a normalized value (0 to 1), where 0 is at the bottom.

`SecretArguments=AllowedWhenUntainted`

### SetRotation

```lua
TextureBase:SetRotation(radians: number, normalizedRotationPoint: vector2?)
```

`SecretArguments=AllowedWhenTainted` `SecretArgumentsAddAspect={ Enum.SecretAspect.Rotation }`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `radians` | `number` |  |
| `normalizedRotationPoint` | `vector2?` | `Mixin=Vector2DMixin` |

### SetSnapToPixelGrid

```lua
TextureBase:SetSnapToPixelGrid(snap: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `snap` | `bool` | default `false` |

### SetSpriteSheetCell

```lua
TextureBase:SetSpriteSheetCell(cell: luaIndex, numRows: number, numColumns: number, cellWidth: number?, cellHeight: number?)
```

`SecretArguments=AllowedWhenTainted` `SecretArgumentsAddAspect={ Enum.SecretAspect.TexCoords }`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `cell` | `luaIndex` | `ConditionalSecret` |
| `numRows` | `number` | `NeverSecret` |
| `numColumns` | `number` | `NeverSecret` |
| `cellWidth` | `number?` | `NeverSecret` |
| `cellHeight` | `number?` | `NeverSecret` |

### SetSVG

```lua
TextureBase:SetSVG(svgAsset: FileAsset) -> success: bool
```

`SecretArguments=AllowedWhenTainted`

### SetTexCoord

```lua
TextureBase:SetTexCoord(left: number, right: number, bottom: number, top: number)
```

`SecretArguments=AllowedWhenTainted` `SecretArgumentsAddAspect={ Enum.SecretAspect.TexCoords }`

### SetTexelSnappingBias

```lua
TextureBase:SetTexelSnappingBias(bias: normalizedValue)
```

`SecretArguments=AllowedWhenUntainted`

### SetTexture

```lua
TextureBase:SetTexture(textureAsset: cstring?, wrapModeHorizontal: cstring?, wrapModeVertical: cstring?, filterMode: cstring?) -> success: bool
```

`SecretArguments=AllowedWhenTainted`

### SetTextureSliceMargins

```lua
TextureBase:SetTextureSliceMargins(left: number, top: number, right: number, bottom: number)
```

Enables nineslice texture rendering using the specified pixel margins. Preferred over legacy nineslice approach that uses 9 separate textures.

`SecretArguments=AllowedWhenUntainted`

### SetTextureSliceMode

```lua
TextureBase:SetTextureSliceMode(sliceMode: UITextureSliceMode)
```

Controls whether the center and sides are Stretched or Tiled when using nineslice texture rendering. Defaults to Stretched.

`SecretArguments=AllowedWhenUntainted`

### SetVertexOffset

```lua
TextureBase:SetVertexOffset(vertexIndex: luaIndex, offsetX: uiUnit, offsetY: uiUnit)
```

`SecretArguments=AllowedWhenUntainted`

### SetVertTile

```lua
TextureBase:SetVertTile(tiling: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `tiling` | `bool` | default `false` |
