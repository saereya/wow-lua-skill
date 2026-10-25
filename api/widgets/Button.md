# Button

Widget methods (`SimpleButtonAPI`) · inherits [`Frame`](Frame.md) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/simplebuttonapidocumentation.lua` (FileDataID 4637219)

## Methods

### ClearDisabledTexture

```lua
Button:ClearDisabledTexture()
```

### ClearHighlightTexture

```lua
Button:ClearHighlightTexture()
```

### ClearNormalTexture

```lua
Button:ClearNormalTexture()
```

### ClearPushedTexture

```lua
Button:ClearPushedTexture()
```

### Click

```lua
Button:Click(button: cstring, isDown: bool)
```

`SecretArguments=NotAllowed`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `button` | `cstring` | default `"LeftButton"` |
| `isDown` | `bool` | default `false` |

### Disable

```lua
Button:Disable()
```

`IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

### Enable

```lua
Button:Enable()
```

`IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

### GetButtonState

```lua
Button:GetButtonState() -> buttonState: SimpleButtonStateToken
```

`SecretReturnsForAspect={ Enum.SecretAspect.ButtonState }`

### GetDisabledFontObject

```lua
Button:GetDisabledFontObject() -> font: SimpleFont
```

### GetDisabledTexture

```lua
Button:GetDisabledTexture() -> texture: SimpleTexture
```

### GetFontString

```lua
Button:GetFontString() -> fontString: SimpleFontString
```

### GetHighlightFontObject

```lua
Button:GetHighlightFontObject() -> font: SimpleFont
```

### GetHighlightTexture

```lua
Button:GetHighlightTexture() -> texture: SimpleTexture
```

### GetMotionScriptsWhileDisabled

```lua
Button:GetMotionScriptsWhileDisabled() -> motionScriptsWhileDisabled: bool
```

### GetNormalFontObject

```lua
Button:GetNormalFontObject() -> font: SimpleFont
```

### GetNormalTexture

```lua
Button:GetNormalTexture() -> texture: SimpleTexture
```

### GetPushedTextOffset

```lua
Button:GetPushedTextOffset() -> offsetX: uiUnit, offsetY: uiUnit
```

### GetPushedTexture

```lua
Button:GetPushedTexture() -> texture: SimpleTexture
```

### GetText

```lua
Button:GetText() -> text: cstring
```

`SecretReturnsForAspect={ Enum.SecretAspect.Text }`

### GetTextHeight

```lua
Button:GetTextHeight() -> height: uiUnit
```

### GetTextWidth

```lua
Button:GetTextWidth() -> width: uiUnit
```

### IsEnabled

```lua
Button:IsEnabled() -> isEnabled: bool
```

`SecretReturnsForAspect={ Enum.SecretAspect.ButtonState }`

### RegisterForClicks

```lua
Button:RegisterForClicks(buttons: ClickButton)
```

`SecretArguments=NotAllowed` `IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

Arguments:

| Name | Type | Notes |
|---|---|---|
| `buttons` | `ClickButton` | `StrideIndex=1` |

### RegisterForMouse

```lua
Button:RegisterForMouse(buttons: ClickButton)
```

`SecretArguments=NotAllowed` `IsProtectedFunction`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

Arguments:

| Name | Type | Notes |
|---|---|---|
| `buttons` | `ClickButton` | `StrideIndex=1` |

### SetButtonState

```lua
Button:SetButtonState(buttonState: SimpleButtonStateToken, lock: bool)
```

`SecretArguments=AllowedWhenUntainted` `SecretArgumentsAddAspect={ Enum.SecretAspect.ButtonState }`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `buttonState` | `SimpleButtonStateToken` |  |
| `lock` | `bool` | default `false` |

### SetDisabledAtlas

```lua
Button:SetDisabledAtlas(atlas: textureAtlas)
```

`SecretArguments=AllowedWhenUntainted`

### SetDisabledFontObject

```lua
Button:SetDisabledFontObject(font: SimpleFont)
```

`SecretArguments=AllowedWhenUntainted`

### SetDisabledTexture

```lua
Button:SetDisabledTexture(asset: TextureAsset)
```

`SecretArguments=AllowedWhenUntainted` `CheckAllowChangeParent`

### SetEnabled

```lua
Button:SetEnabled(enabled: bool)
```

`SecretArguments=AllowedWhenUntainted` `IsProtectedFunction` `SecretArgumentsAddAspect={ Enum.SecretAspect.ButtonState }`

> Protected: only callable from Blizzard secure code or in response to a hardware event.

Arguments:

| Name | Type | Notes |
|---|---|---|
| `enabled` | `bool` | default `false` |

### SetFontString

```lua
Button:SetFontString(fontString: SimpleFontString)
```

`SecretArguments=AllowedWhenUntainted` `CheckAllowChangeParent`

### SetFormattedText

```lua
Button:SetFormattedText(text: cstring)
```

`SecretArguments=AllowedWhenUntainted` `SecretArgumentsAddAspect={ Enum.SecretAspect.Text }`

### SetHighlightAtlas

```lua
Button:SetHighlightAtlas(atlas: textureAtlas, blendMode: BlendMode?)
```

`SecretArguments=AllowedWhenUntainted`

### SetHighlightFontObject

```lua
Button:SetHighlightFontObject(font: SimpleFont)
```

`SecretArguments=AllowedWhenUntainted`

### SetHighlightTexture

```lua
Button:SetHighlightTexture(asset: TextureAsset, blendMode: BlendMode?)
```

`SecretArguments=AllowedWhenUntainted` `CheckAllowChangeParent`

### SetMotionScriptsWhileDisabled

```lua
Button:SetMotionScriptsWhileDisabled(motionScriptsWhileDisabled: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetNormalAtlas

```lua
Button:SetNormalAtlas(atlas: textureAtlas)
```

`SecretArguments=AllowedWhenUntainted`

### SetNormalFontObject

```lua
Button:SetNormalFontObject(font: SimpleFont)
```

`SecretArguments=AllowedWhenUntainted`

### SetNormalTexture

```lua
Button:SetNormalTexture(asset: TextureAsset)
```

`SecretArguments=AllowedWhenUntainted` `CheckAllowChangeParent`

### SetPushedAtlas

```lua
Button:SetPushedAtlas(atlas: textureAtlas)
```

`SecretArguments=AllowedWhenUntainted`

### SetPushedTextOffset

```lua
Button:SetPushedTextOffset(offsetX: uiUnit, offsetY: uiUnit)
```

`SecretArguments=AllowedWhenUntainted`

### SetPushedTexture

```lua
Button:SetPushedTexture(asset: TextureAsset)
```

`SecretArguments=AllowedWhenUntainted` `CheckAllowChangeParent`

### SetText

```lua
Button:SetText(text: cstring)
```

`SecretArguments=AllowedWhenUntainted` `SecretArgumentsAddAspect={ Enum.SecretAspect.Text }`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` | default `""` |
