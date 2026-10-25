# FontString

Widget methods (`SimpleFontStringAPI`) · inherits [`Region`](Region.md), [`FontInstance`](FontInstance.md) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/simplefontstringapidocumentation.lua` (FileDataID 4637227)

## Methods

### CalculateScreenAreaFromCharacterSpan

```lua
FontString:CalculateScreenAreaFromCharacterSpan(leftIndex: luaIndex, rightIndex: luaIndex) -> areas: uiBoundsRect[]?
```

`SecretArguments=AllowedWhenUntainted` `RequiresFontStringTextAccess` `SecretWhenAnchoringSecret` `SecretReturnsForAspect={ Enum.SecretAspect.Text }`

### CanNonSpaceWrap

```lua
FontString:CanNonSpaceWrap() -> wrap: bool
```

### CanWordWrap

```lua
FontString:CanWordWrap() -> wrap: bool
```

### ClearAlphaGradient

```lua
FontString:ClearAlphaGradient()
```

### ClearText

```lua
FontString:ClearText()
```

Sets text to an empty string and removes the Text secret aspect.

### FindCharacterIndexAtCoordinate

```lua
FontString:FindCharacterIndexAtCoordinate(x: uiUnit, y: uiUnit) -> characterIndex: luaIndex, inside: bool
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `RequiresFontStringTextAccess` `SecretWhenAnchoringSecret` `SecretReturnsForAspect={ Enum.SecretAspect.Text }`

### GetAlphaGradient

```lua
FontString:GetAlphaGradient() -> start: number, length: number
```

### GetFieldSize

```lua
FontString:GetFieldSize() -> fieldSize: number
```

### GetFont

```lua
FontString:GetFont() -> fontFile: FontAsset?, fontHeight: uiUnit, flags: TBFFlags
```

### GetFontHeight

```lua
FontString:GetFontHeight(calculated: bool) -> height: uiUnit
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `calculated` | `bool` | default `true` |

### GetFontObject

```lua
FontString:GetFontObject() -> font: SimpleFont
```

### GetIndentedWordWrap

```lua
FontString:GetIndentedWordWrap() -> wrap: bool
```

### GetJustifyH

```lua
FontString:GetJustifyH() -> justifyH: JustifyHorizontal
```

### GetJustifyV

```lua
FontString:GetJustifyV() -> justifyV: JustifyVertical
```

### GetLineHeight

```lua
FontString:GetLineHeight() -> lineHeight: uiUnit
```

### GetMaxLines

```lua
FontString:GetMaxLines() -> maxLines: number
```

### GetNumLines

```lua
FontString:GetNumLines() -> numLines: number
```

`SecretWhenAnchoringSecret`

### GetRotation

```lua
FontString:GetRotation() -> radians: number
```

### GetScaleAnimationMode

```lua
FontString:GetScaleAnimationMode() -> scaleAnimationMode: FontStringScaleAnimationMode
```

### GetShadowColor

```lua
FontString:GetShadowColor() -> colorR: number, colorG: number, colorB: number, colorA: number
```

### GetShadowOffset

```lua
FontString:GetShadowOffset() -> offsetX: number, offsetY: number
```

### GetSmoothScaling

```lua
FontString:GetSmoothScaling() -> smoothScaling: bool
```

### GetSpacing

```lua
FontString:GetSpacing() -> spacing: uiUnit
```

### GetStringHeight

```lua
FontString:GetStringHeight() -> height: uiUnit
```

`SecretWhenAnchoringSecret`

### GetStringWidth

```lua
FontString:GetStringWidth() -> width: uiUnit
```

`SecretWhenAnchoringSecret`

### GetText

```lua
FontString:GetText() -> text: cstring
```

`SecretReturnsForAspect={ Enum.SecretAspect.Text }`

### GetTextColor

```lua
FontString:GetTextColor() -> colorR: number, colorG: number, colorB: number, colorA: number
```

`MayReturnNothing` `SecretReturnsForAspect={ Enum.SecretAspect.VertexColor, Enum.SecretAspect.Alpha }`

### GetTextScale

```lua
FontString:GetTextScale() -> textScale: number
```

### GetUnboundedStringWidth

```lua
FontString:GetUnboundedStringWidth() -> width: uiUnit
```

`SecretWhenAnchoringSecret`

### GetUnboundedStringWidthForText

```lua
FontString:GetUnboundedStringWidthForText(text: cstring) -> width: uiUnit
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenAnchoringSecret`

### GetWrappedWidth

```lua
FontString:GetWrappedWidth() -> width: uiUnit
```

`SecretWhenAnchoringSecret`

### IsTruncated

```lua
FontString:IsTruncated() -> isTruncated: bool
```

`SecretWhenAnchoringSecret`

### OnColorsUpdated

```lua
FontString:OnColorsUpdated()
```

### SetAlphaGradient

```lua
FontString:SetAlphaGradient(start: number, length: number) -> isWithinText: bool
```

`SecretArguments=AllowedWhenUntainted`

### SetDesaturateEmbeddedTextures

```lua
FontString:SetDesaturateEmbeddedTextures(desaturate: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetFixedColor

```lua
FontString:SetFixedColor(fixedColor: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetFont

```lua
FontString:SetFont(fontFile: FontAsset, fontHeight: uiFontHeight, flags: TBFFlags?) -> success: bool
```

`SecretArguments=AllowedWhenUntainted` `RequiresValidFontAsset` `RequiresValidFontHeight`

### SetFontHeight

```lua
FontString:SetFontHeight(height: uiUnit)
```

`SecretArguments=AllowedWhenUntainted`

### SetFontObject

```lua
FontString:SetFontObject(font: SimpleFont)
```

`SecretArguments=AllowedWhenUntainted`

### SetFormattedText

```lua
FontString:SetFormattedText(text: cstring)
```

`SecretArguments=AllowedWhenTainted` `SecretArgumentsAddAspect={ Enum.SecretAspect.Text }`

### SetIndentedWordWrap

```lua
FontString:SetIndentedWordWrap(wrap: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetJustifyH

```lua
FontString:SetJustifyH(justifyH: JustifyHorizontal)
```

`SecretArguments=AllowedWhenUntainted`

### SetJustifyV

```lua
FontString:SetJustifyV(justifyV: JustifyVertical)
```

`SecretArguments=AllowedWhenUntainted`

### SetMaxLines

```lua
FontString:SetMaxLines(maxLines: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetNonSpaceWrap

```lua
FontString:SetNonSpaceWrap(wrap: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetRotation

```lua
FontString:SetRotation(radians: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetScaleAnimationMode

```lua
FontString:SetScaleAnimationMode(scaleAnimationMode: FontStringScaleAnimationMode)
```

`SecretArguments=NotAllowed`

### SetShadowColor

```lua
FontString:SetShadowColor(colorR: number, colorG: number, colorB: number, a: SingleColorValue?)
```

`SecretArguments=AllowedWhenUntainted`

### SetShadowOffset

```lua
FontString:SetShadowOffset(offsetX: number, offsetY: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetSmoothScaling

```lua
FontString:SetSmoothScaling(smoothScaling: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `smoothScaling` | `bool` | If true, text height will not snap to nearest whole numbers for scaled font strings. |

### SetSpacing

```lua
FontString:SetSpacing(spacing: uiUnit)
```

`SecretArguments=AllowedWhenUntainted`

### SetText

```lua
FontString:SetText(text: cstring)
```

`SecretArguments=AllowedWhenTainted` `SecretArgumentsAddAspect={ Enum.SecretAspect.Text }`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` | default `""` |

### SetTextColor

```lua
FontString:SetTextColor(colorR: number, colorG: number, colorB: number, a: SingleColorValue?)
```

`SecretArguments=AllowedWhenTainted` `SecretArgumentsAddAspect={ Enum.SecretAspect.VertexColor, Enum.SecretAspect.Alpha }`

### SetTextHeight

```lua
FontString:SetTextHeight(height: uiUnit)
```

`SecretArguments=AllowedWhenUntainted`

### SetTextScale

```lua
FontString:SetTextScale(textScale: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetTextToFit

```lua
FontString:SetTextToFit(text: cstring)
```

`SecretArguments=AllowedWhenTainted` `SecretArgumentsAddAspect={ Enum.SecretAspect.Text }`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` | default `""` |

### SetWordWrap

```lua
FontString:SetWordWrap(wrap: bool)
```

`SecretArguments=AllowedWhenUntainted`
