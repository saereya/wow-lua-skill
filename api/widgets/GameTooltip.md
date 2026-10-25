# GameTooltip

Widget methods (`FrameAPITooltip`) · inherits [`Frame`](Frame.md) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/frameapitooltipdocumentation.lua` (FileDataID 7449379)

## Methods

### AddFontStrings

```lua
GameTooltip:AddFontStrings(leftFontString: SimpleFontString, rightFontString: SimpleFontString)
```

`SecretArguments=AllowedWhenUntainted` `CheckAllowChangeParent`

### ClearPadding

```lua
GameTooltip:ClearPadding()
```

Set all padding values to 0.0 and remove the Padding SecretAspect.

### GetLeftLine

```lua
GameTooltip:GetLeftLine(line: luaIndex) -> leftFontString: SimpleFontString
```

`SecretArguments=AllowedWhenUntainted`

### GetMinimumWidth

```lua
GameTooltip:GetMinimumWidth() -> width: number, forced: bool
```

`SecretReturnsForAspect={ Enum.SecretAspect.MinimumWidth }`

### GetPadding

```lua
GameTooltip:GetPadding() -> right: number, bottom: number, left: number, top: number
```

`SecretReturnsForAspect={ Enum.SecretAspect.Padding }`

### GetRightLine

```lua
GameTooltip:GetRightLine(line: luaIndex) -> rightFontString: SimpleFontString
```

`SecretArguments=AllowedWhenUntainted`

### SetMinimumWidth

```lua
GameTooltip:SetMinimumWidth(width: number, force: bool)
```

`SecretArguments=AllowedWhenUntainted` `SecretArgumentsAddAspect={ Enum.SecretAspect.MinimumWidth }`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `width` | `number` |  |
| `force` | `bool` | default `false` |

### SetPadding

```lua
GameTooltip:SetPadding(right: number, bottom: number, left: number?, top: number?)
```

`SecretArguments=AllowedWhenUntainted` `SecretArgumentsAddAspect={ Enum.SecretAspect.Padding }`

### SetText

```lua
GameTooltip:SetText(text: cstring, colorR: number, colorG: number, colorB: number, alpha: number, wrap: bool)
```

`SecretArguments=AllowedWhenTainted` `SecretArgumentsAddAspect={ Enum.SecretAspect.Text }`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` | `ConditionalSecret` |
| `colorR` | `number` |  |
| `colorG` | `number` |  |
| `colorB` | `number` |  |
| `alpha` | `number` | default `1`; `ConditionalSecret` |
| `wrap` | `bool` | default `false`; `ConditionalSecret` |
