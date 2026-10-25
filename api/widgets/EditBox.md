# EditBox

Widget methods (`SimpleEditBoxAPI`) · inherits [`Frame`](Frame.md), [`FontInstance`](FontInstance.md) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/simpleeditboxapidocumentation.lua` (FileDataID 4637213)

## Methods

### AddHistoryLine

```lua
EditBox:AddHistoryLine(text: cstring)
```

`SecretArguments=AllowedWhenUntainted`

### ClearFocus

```lua
EditBox:ClearFocus()
```

### ClearHighlightText

```lua
EditBox:ClearHighlightText()
```

### ClearHistory

```lua
EditBox:ClearHistory()
```

### Disable

```lua
EditBox:Disable()
```

### Enable

```lua
EditBox:Enable()
```

### GetAltArrowKeyMode

```lua
EditBox:GetAltArrowKeyMode() -> altMode: bool
```

### GetBlinkSpeed

```lua
EditBox:GetBlinkSpeed() -> cursorBlinkSpeedSec: number
```

### GetCursorPosition

```lua
EditBox:GetCursorPosition() -> cursorPosition: number
```

`SecretReturnsForAspect={ Enum.SecretAspect.Cursor, Enum.SecretAspect.Text }`

### GetDisplayText

```lua
EditBox:GetDisplayText() -> displayText: string
```

`MayReturnNothing` `SecretReturnsForAspect={ Enum.SecretAspect.Text }`

### GetFont

```lua
EditBox:GetFont() -> name: cstring, fontHeight: uiUnit, flags: TBFFlags
```

### GetFontObject

```lua
EditBox:GetFontObject() -> font: SimpleFont
```

### GetHighlightColor

```lua
EditBox:GetHighlightColor() -> colorR: number, colorG: number, colorB: number, colorA: number
```

### GetHistoryLines

```lua
EditBox:GetHistoryLines() -> numHistoryLines: number
```

### GetIndentedWordWrap

```lua
EditBox:GetIndentedWordWrap() -> isIndented: bool
```

### GetInputLanguage

```lua
EditBox:GetInputLanguage() -> language: cstring
```

### GetJustifyH

```lua
EditBox:GetJustifyH() -> justifyH: JustifyHorizontal
```

### GetJustifyV

```lua
EditBox:GetJustifyV() -> justifyV: JustifyVertical
```

### GetMaxBytes

```lua
EditBox:GetMaxBytes() -> maxBytes: number
```

### GetMaxLetters

```lua
EditBox:GetMaxLetters() -> maxLetters: number
```

### GetNumber

```lua
EditBox:GetNumber() -> number: number?
```

`SecretReturnsForAspect={ Enum.SecretAspect.Text }`

### GetNumLetters

```lua
EditBox:GetNumLetters() -> numLetters: number
```

`MayReturnNothing`

### GetNumLines

```lua
EditBox:GetNumLines() -> lines: number
```

### GetShadowColor

```lua
EditBox:GetShadowColor() -> colorR: number, colorG: number, colorB: number, colorA: number
```

### GetShadowOffset

```lua
EditBox:GetShadowOffset() -> offsetX: number, offsetY: number
```

### GetSpacing

```lua
EditBox:GetSpacing() -> fontHeight: uiUnit
```

### GetText

```lua
EditBox:GetText() -> text: cstring
```

`SecretReturnsForAspect={ Enum.SecretAspect.Text }`

### GetTextColor

```lua
EditBox:GetTextColor() -> colorR: number, colorG: number, colorB: number, colorA: number
```

### GetTextInsets

```lua
EditBox:GetTextInsets() -> left: uiUnit, right: uiUnit, top: uiUnit, bottom: uiUnit
```

### GetUTF8CursorPosition

```lua
EditBox:GetUTF8CursorPosition() -> cursorPosition: number
```

`SecretReturnsForAspect={ Enum.SecretAspect.Cursor, Enum.SecretAspect.Text }`

### GetVisibleTextByteLimit

```lua
EditBox:GetVisibleTextByteLimit() -> maxVisibleBytes: number
```

### HasFocus

```lua
EditBox:HasFocus() -> hasFocus: bool
```

### HasText

```lua
EditBox:HasText() -> hasText: bool
```

### HighlightText

```lua
EditBox:HighlightText(start: number, stop: number)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `start` | `number` | default `0` |
| `stop` | `number` | default `-1` |

### Insert

```lua
EditBox:Insert(text: cstring)
```

`SecretArguments=AllowedWhenUntainted` `SecretArgumentsAddAspect={ Enum.SecretAspect.Text }`

### IsAlphabeticOnly

```lua
EditBox:IsAlphabeticOnly() -> enabled: bool
```

### IsAutoFocus

```lua
EditBox:IsAutoFocus() -> autoFocus: bool
```

### IsCountInvisibleLetters

```lua
EditBox:IsCountInvisibleLetters() -> countInvisibleLetters: bool
```

### IsEnabled

```lua
EditBox:IsEnabled() -> isEnabled: bool
```

### IsInIMECompositionMode

```lua
EditBox:IsInIMECompositionMode() -> isInIMECompositionMode: bool
```

### IsMultiLine

```lua
EditBox:IsMultiLine() -> multiline: bool
```

### IsNumeric

```lua
EditBox:IsNumeric() -> isNumeric: bool
```

### IsNumericFullRange

```lua
EditBox:IsNumericFullRange() -> isNumeric: bool
```

### IsPassword

```lua
EditBox:IsPassword() -> isPassword: bool
```

### IsSecureText

```lua
EditBox:IsSecureText() -> isSecure: bool
```

`SecretReturnsForAspect={ Enum.SecretAspect.SecureText }`

### ResetInputMode

```lua
EditBox:ResetInputMode()
```

### SetAlphabeticOnly

```lua
EditBox:SetAlphabeticOnly(enabled: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `enabled` | `bool` | default `false` |

### SetAltArrowKeyMode

```lua
EditBox:SetAltArrowKeyMode(altMode: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `altMode` | `bool` | default `false` |

### SetAutoFocus

```lua
EditBox:SetAutoFocus(autoFocus: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `autoFocus` | `bool` | default `false` |

### SetBlinkSpeed

```lua
EditBox:SetBlinkSpeed(cursorBlinkSpeedSec: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetCountInvisibleLetters

```lua
EditBox:SetCountInvisibleLetters(countInvisibleLetters: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `countInvisibleLetters` | `bool` | default `false` |

### SetCursorPosition

```lua
EditBox:SetCursorPosition(cursorPosition: number)
```

`SecretArguments=AllowedWhenUntainted` `SecretArgumentsAddAspect={ Enum.SecretAspect.Cursor }`

### SetEnabled

```lua
EditBox:SetEnabled(enabled: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `enabled` | `bool` | default `false` |

### SetFocus

```lua
EditBox:SetFocus()
```

### SetFont

```lua
EditBox:SetFont(fontFile: cstring, height: uiFontHeight, flags: TBFFlags) -> success: bool
```

`SecretArguments=AllowedWhenUntainted` `RequiresValidFontAsset` `RequiresValidFontHeight`

### SetFontObject

```lua
EditBox:SetFontObject(font: SimpleFont)
```

`SecretArguments=AllowedWhenUntainted`

### SetHighlightColor

```lua
EditBox:SetHighlightColor(colorR: number, colorG: number, colorB: number, a: SingleColorValue?)
```

`SecretArguments=AllowedWhenUntainted`

### SetHistoryLines

```lua
EditBox:SetHistoryLines(numHistoryLines: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetIndentedWordWrap

```lua
EditBox:SetIndentedWordWrap(isIndented: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `isIndented` | `bool` | default `false` |

### SetJustifyH

```lua
EditBox:SetJustifyH(justifyH: JustifyHorizontal)
```

`SecretArguments=AllowedWhenUntainted`

### SetJustifyV

```lua
EditBox:SetJustifyV(justifyV: JustifyVertical)
```

`SecretArguments=AllowedWhenUntainted`

### SetMaxBytes

```lua
EditBox:SetMaxBytes(maxBytes: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetMaxLetters

```lua
EditBox:SetMaxLetters(maxLetters: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetMultiLine

```lua
EditBox:SetMultiLine(multiline: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `multiline` | `bool` | default `false` |

### SetNumber

```lua
EditBox:SetNumber(number: number)
```

`SecretArguments=AllowedWhenUntainted` `SecretArgumentsAddAspect={ Enum.SecretAspect.Text }`

### SetNumeric

```lua
EditBox:SetNumeric(isNumeric: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `isNumeric` | `bool` | default `false` |

### SetNumericFullRange

```lua
EditBox:SetNumericFullRange(isNumeric: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `isNumeric` | `bool` | default `false` |

### SetPassword

```lua
EditBox:SetPassword(isPassword: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `isPassword` | `bool` | default `false` |

### SetSecureText

```lua
EditBox:SetSecureText(isSecure: bool)
```

`SecretArguments=AllowedWhenUntainted` `SecretArgumentsAddAspect={ Enum.SecretAspect.SecureText }`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `isSecure` | `bool` | default `false` |

### SetSecurityDisablePaste

```lua
EditBox:SetSecurityDisablePaste()
```

### SetSecurityDisableSetText

```lua
EditBox:SetSecurityDisableSetText()
```

### SetShadowColor

```lua
EditBox:SetShadowColor(colorR: number, colorG: number, colorB: number, a: SingleColorValue?)
```

`SecretArguments=AllowedWhenUntainted`

### SetShadowOffset

```lua
EditBox:SetShadowOffset(offsetX: number, offsetY: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetSpacing

```lua
EditBox:SetSpacing(fontHeight: uiUnit)
```

`SecretArguments=AllowedWhenUntainted`

### SetText

```lua
EditBox:SetText(text: cstring)
```

`SecretArguments=AllowedWhenUntainted` `SecretArgumentsAddAspect={ Enum.SecretAspect.Text }`

### SetTextColor

```lua
EditBox:SetTextColor(colorR: number, colorG: number, colorB: number, a: SingleColorValue?)
```

`SecretArguments=AllowedWhenUntainted`

### SetTextInsets

```lua
EditBox:SetTextInsets(left: uiUnit, right: uiUnit, top: uiUnit, bottom: uiUnit)
```

`SecretArguments=AllowedWhenUntainted`

### SetVisibleTextByteLimit

```lua
EditBox:SetVisibleTextByteLimit(maxVisibleBytes: number)
```

`SecretArguments=AllowedWhenUntainted`

### ToggleInputLanguage

```lua
EditBox:ToggleInputLanguage()
```
