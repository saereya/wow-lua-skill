# SimpleHTML

Widget methods (`SimpleHTMLAPI`) · inherits [`Frame`](Frame.md), [`FontInstance`](FontInstance.md) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/simplehtmlapidocumentation.lua` (FileDataID 4637224)

## Methods

### GetContentHeight

```lua
SimpleHTML:GetContentHeight() -> height: uiUnit
```

### GetFont

```lua
SimpleHTML:GetFont(textType: HTMLTextType) -> fontFile: cstring, height: uiFontHeight, flags: TBFFlags
```

`SecretArguments=AllowedWhenUntainted` `ConstSecretAccessor`

### GetFontObject

```lua
SimpleHTML:GetFontObject(textType: HTMLTextType) -> font: SimpleFont
```

`SecretArguments=AllowedWhenUntainted` `ConstSecretAccessor`

### GetHyperlinkFormat

```lua
SimpleHTML:GetHyperlinkFormat() -> format: cstring
```

### GetIndentedWordWrap

```lua
SimpleHTML:GetIndentedWordWrap(textType: HTMLTextType) -> wordWrap: bool
```

`SecretArguments=AllowedWhenUntainted` `ConstSecretAccessor`

### GetJustifyH

```lua
SimpleHTML:GetJustifyH(textType: HTMLTextType) -> justifyH: JustifyHorizontal
```

`SecretArguments=AllowedWhenUntainted` `ConstSecretAccessor`

### GetJustifyV

```lua
SimpleHTML:GetJustifyV(textType: HTMLTextType) -> justifyV: JustifyVertical
```

`SecretArguments=AllowedWhenUntainted` `ConstSecretAccessor`

### GetShadowColor

```lua
SimpleHTML:GetShadowColor(textType: HTMLTextType) -> colorR: number, colorG: number, colorB: number, colorA: number
```

`SecretArguments=AllowedWhenUntainted` `ConstSecretAccessor`

### GetShadowOffset

```lua
SimpleHTML:GetShadowOffset(textType: HTMLTextType) -> offsetX: number, offsetY: number
```

`SecretArguments=AllowedWhenUntainted` `ConstSecretAccessor`

### GetSpacing

```lua
SimpleHTML:GetSpacing(textType: HTMLTextType) -> spacing: uiUnit
```

`SecretArguments=AllowedWhenUntainted` `ConstSecretAccessor`

### GetTextColor

```lua
SimpleHTML:GetTextColor(textType: HTMLTextType) -> colorR: number, colorG: number, colorB: number, colorA: number
```

`SecretArguments=AllowedWhenUntainted` `ConstSecretAccessor`

### GetTextData

```lua
SimpleHTML:GetTextData() -> content: HTMLContentNode[]
```

`SecretReturnsForAspect={ Enum.SecretAspect.Text }`

### SetFont

```lua
SimpleHTML:SetFont(textType: HTMLTextType, fontFile: cstring, height: uiFontHeight, flags: TBFFlags)
```

`SecretArguments=AllowedWhenUntainted` `RequiresValidFontAsset` `RequiresValidFontHeight`

### SetFontObject

```lua
SimpleHTML:SetFontObject(textType: HTMLTextType, font: SimpleFont)
```

`SecretArguments=AllowedWhenUntainted`

### SetHyperlinkFormat

```lua
SimpleHTML:SetHyperlinkFormat(format: cstring)
```

`SecretArguments=AllowedWhenUntainted`

### SetIndentedWordWrap

```lua
SimpleHTML:SetIndentedWordWrap(textType: HTMLTextType, wordWrap: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetJustifyH

```lua
SimpleHTML:SetJustifyH(textType: HTMLTextType, justifyH: JustifyHorizontal)
```

`SecretArguments=AllowedWhenUntainted`

### SetJustifyV

```lua
SimpleHTML:SetJustifyV(textType: HTMLTextType, justifyV: JustifyVertical)
```

`SecretArguments=AllowedWhenUntainted`

### SetShadowColor

```lua
SimpleHTML:SetShadowColor(textType: HTMLTextType, colorR: number, colorG: number, colorB: number, a: SingleColorValue?)
```

`SecretArguments=AllowedWhenUntainted`

### SetShadowOffset

```lua
SimpleHTML:SetShadowOffset(textType: HTMLTextType, offsetX: number, offsetY: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetSpacing

```lua
SimpleHTML:SetSpacing(textType: HTMLTextType, spacing: uiUnit)
```

`SecretArguments=AllowedWhenUntainted`

### SetText

```lua
SimpleHTML:SetText(text: cstring, ignoreMarkup: bool)
```

`SecretArguments=AllowedWhenUntainted` `SecretArgumentsAddAspect={ Enum.SecretAspect.Text }`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` |  |
| `ignoreMarkup` | `bool` | default `false` |

### SetTextColor

```lua
SimpleHTML:SetTextColor(textType: HTMLTextType, colorR: number, colorG: number, colorB: number, a: SingleColorValue?)
```

`SecretArguments=AllowedWhenUntainted`
