# Font

Global functions · environment All · source `interface/addons/blizzard_apidocumentationgenerated/fontdocumentation.lua` (FileDataID 5200984)

## Functions

### CreateFontFamily

```lua
CreateFontFamily(name: cstring, members: CreateFontFamilyMemberInfo[]) -> fontFamily: SimpleFont
```

`SecretArguments=AllowedWhenUntainted`

### GetFontInfo

```lua
GetFontInfo(fontObject: SimpleFont) -> info: FontScriptInfo?
```

`SecretArguments=AllowedWhenUntainted`

### GetFonts

```lua
GetFonts() -> fontNames: cstring[]
```

## Types

### CreateFontFamilyMemberInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `alphabet` | `FontAlphabet` |  |
| `file` | `cstring` |  |
| `height` | `uiFontHeight` |  |
| `flags` | `TBFFlags` |  |

### FontScriptInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `color` | `colorRGBA` | `Mixin=ColorMixin` |
| `height` | `number` |  |
| `outline` | `string` |  |
| `shadow` | `FontScriptShadowInfo?` |  |
| `fontObject` | `SimpleFont` |  |
| `canBeUserScaled` | `bool` |  |

### FontScriptShadowInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `color` | `colorRGBA` | `Mixin=ColorMixin` |
| `x` | `number` |  |
| `y` | `number` |  |
