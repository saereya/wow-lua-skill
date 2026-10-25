# FontInstance

Widget methods (`SimpleFontAPI`) · inherits [`Object`](Object.md) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/simplefontapidocumentation.lua` (FileDataID 4637217)

## Methods

### CopyFontObject

```lua
FontInstance:CopyFontObject(sourceFont: SimpleFont)
```

`SecretArguments=AllowedWhenUntainted`

### GetAlpha

```lua
FontInstance:GetAlpha() -> alpha: SingleColorValue
```

### GetFont

```lua
FontInstance:GetFont() -> fontFile: cstring, height: uiFontHeight, flags: TBFFlags
```

### GetFontHeight

```lua
FontInstance:GetFontHeight() -> height: number
```

Return is either in uiUnits or internal height due to fixedHeight.

### GetFontObject

```lua
FontInstance:GetFontObject() -> font: SimpleFont
```

### GetFontObjectForAlphabet

```lua
FontInstance:GetFontObjectForAlphabet(alphabet: FontAlphabet) -> font: SimpleFont
```

`SecretArguments=AllowedWhenUntainted` `ConstSecretAccessor`

### GetIndentedWordWrap

```lua
FontInstance:GetIndentedWordWrap() -> wordWrap: bool
```

### GetJustifyH

```lua
FontInstance:GetJustifyH() -> justifyH: JustifyHorizontal
```

### GetJustifyV

```lua
FontInstance:GetJustifyV() -> justifyV: JustifyVertical
```

### GetShadowColor

```lua
FontInstance:GetShadowColor() -> colorR: number, colorG: number, colorB: number, colorA: number
```

### GetShadowOffset

```lua
FontInstance:GetShadowOffset() -> offsetX: number, offsetY: number
```

### GetSpacing

```lua
FontInstance:GetSpacing() -> spacing: uiUnit
```

### GetTextColor

```lua
FontInstance:GetTextColor() -> colorR: number, colorG: number, colorB: number, colorA: number
```

### SetAlpha

```lua
FontInstance:SetAlpha(alpha: SingleColorValue)
```

`SecretArguments=AllowedWhenUntainted`

### SetFont

```lua
FontInstance:SetFont(fontFile: cstring, height: uiFontHeight, flags: TBFFlags)
```

`SecretArguments=AllowedWhenUntainted` `RequiresValidFontAsset` `RequiresValidFontHeight`

### SetFontHeight

```lua
FontInstance:SetFontHeight(height: number)
```

Preserves all flags, does correct height conversion due to fixedHeight.

`SecretArguments=AllowedWhenUntainted`

### SetFontObject

```lua
FontInstance:SetFontObject(font: SimpleFont)
```

`SecretArguments=AllowedWhenUntainted`

### SetIndentedWordWrap

```lua
FontInstance:SetIndentedWordWrap(wordWrap: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetJustifyH

```lua
FontInstance:SetJustifyH(justifyH: JustifyHorizontal)
```

`SecretArguments=AllowedWhenUntainted`

### SetJustifyV

```lua
FontInstance:SetJustifyV(justifyV: JustifyVertical)
```

`SecretArguments=AllowedWhenUntainted`

### SetShadowColor

```lua
FontInstance:SetShadowColor(colorR: number, colorG: number, colorB: number, a: SingleColorValue?)
```

`SecretArguments=AllowedWhenUntainted`

### SetShadowOffset

```lua
FontInstance:SetShadowOffset(offsetX: number, offsetY: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetSpacing

```lua
FontInstance:SetSpacing(spacing: uiUnit)
```

`SecretArguments=AllowedWhenUntainted`

### SetTextColor

```lua
FontInstance:SetTextColor(colorR: number, colorG: number, colorB: number, a: SingleColorValue?)
```

`SecretArguments=AllowedWhenUntainted`
