# MessageFrame

Widget methods (`SimpleMessageFrameAPI`) · inherits [`Frame`](Frame.md), [`FontInstance`](FontInstance.md) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/simplemessageframeapidocumentation.lua` (FileDataID 4637229)

## Methods

### AddMessage

```lua
MessageFrame:AddMessage(text: cstring, colorR: number, colorG: number, colorB: number, a: SingleColorValue?, messageID: number?)
```

`SecretArguments=AllowedWhenUntainted`

### Clear

```lua
MessageFrame:Clear()
```

### GetFadeDuration

```lua
MessageFrame:GetFadeDuration() -> fadeDurationSeconds: number
```

### GetFadePower

```lua
MessageFrame:GetFadePower() -> fadePower: number
```

### GetFading

```lua
MessageFrame:GetFading() -> isFading: bool
```

### GetFont

```lua
MessageFrame:GetFont() -> fontFile: cstring, height: uiFontHeight, flags: TBFFlags
```

### GetFontObject

```lua
MessageFrame:GetFontObject() -> font: SimpleFont
```

### GetFontStringByID

```lua
MessageFrame:GetFontStringByID(messageID: number) -> fontString: SimpleFontString
```

`SecretArguments=AllowedWhenUntainted` `ConstSecretAccessor`

### GetIndentedWordWrap

```lua
MessageFrame:GetIndentedWordWrap() -> wordWrap: bool
```

### GetInsertMode

```lua
MessageFrame:GetInsertMode() -> mode: InsertMode
```

### GetJustifyH

```lua
MessageFrame:GetJustifyH() -> justifyH: JustifyHorizontal
```

### GetJustifyV

```lua
MessageFrame:GetJustifyV() -> justifyV: JustifyVertical
```

### GetShadowColor

```lua
MessageFrame:GetShadowColor() -> colorR: number, colorG: number, colorB: number, colorA: number
```

### GetShadowOffset

```lua
MessageFrame:GetShadowOffset() -> offsetX: number, offsetY: number
```

### GetSpacing

```lua
MessageFrame:GetSpacing() -> spacing: uiUnit
```

### GetTextColor

```lua
MessageFrame:GetTextColor() -> colorR: number, colorG: number, colorB: number, colorA: number
```

### GetTimeVisible

```lua
MessageFrame:GetTimeVisible() -> timeVisibleSeconds: number
```

### HasMessageByID

```lua
MessageFrame:HasMessageByID(messageID: number) -> hasMessage: bool
```

`SecretArguments=AllowedWhenUntainted`

### ResetMessageFadeByID

```lua
MessageFrame:ResetMessageFadeByID(messageID: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetFadeDuration

```lua
MessageFrame:SetFadeDuration(fadeDurationSeconds: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetFadePower

```lua
MessageFrame:SetFadePower(fadePower: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetFading

```lua
MessageFrame:SetFading(fading: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetFont

```lua
MessageFrame:SetFont(fontFile: cstring, height: uiFontHeight, flags: TBFFlags)
```

`SecretArguments=AllowedWhenUntainted` `RequiresValidFontAsset` `RequiresValidFontHeight`

### SetFontObject

```lua
MessageFrame:SetFontObject(font: SimpleFont)
```

`SecretArguments=AllowedWhenUntainted`

### SetIndentedWordWrap

```lua
MessageFrame:SetIndentedWordWrap(wordWrap: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetInsertMode

```lua
MessageFrame:SetInsertMode(mode: InsertMode)
```

`SecretArguments=AllowedWhenUntainted`

### SetJustifyH

```lua
MessageFrame:SetJustifyH(justifyH: JustifyHorizontal)
```

`SecretArguments=AllowedWhenUntainted`

### SetJustifyV

```lua
MessageFrame:SetJustifyV(justifyV: JustifyVertical)
```

`SecretArguments=AllowedWhenUntainted`

### SetShadowColor

```lua
MessageFrame:SetShadowColor(colorR: number, colorG: number, colorB: number, a: SingleColorValue?)
```

`SecretArguments=AllowedWhenUntainted`

### SetShadowOffset

```lua
MessageFrame:SetShadowOffset(offsetX: number, offsetY: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetSpacing

```lua
MessageFrame:SetSpacing(spacing: uiUnit)
```

`SecretArguments=AllowedWhenUntainted`

### SetTextColor

```lua
MessageFrame:SetTextColor(colorR: number, colorG: number, colorB: number, a: SingleColorValue?)
```

`SecretArguments=AllowedWhenUntainted`

### SetTimeVisible

```lua
MessageFrame:SetTimeVisible(timeVisibleSeconds: number)
```

`SecretArguments=AllowedWhenUntainted`
