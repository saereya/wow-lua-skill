# StringUtil

Namespace `C_StringUtil` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/stringutildocumentation.lua` (FileDataID 5145178)

## Functions

### CreateAbbreviatedNumberFormatter

```lua
C_StringUtil.CreateAbbreviatedNumberFormatter() -> formatter: AbbreviatedNumberFormatter
```

Creates a numeric formatter that converts numbers to abbreviated strings, eg. 123456 -> '123k'.

### CreateNumericRuleFormatter

```lua
C_StringUtil.CreateNumericRuleFormatter() -> formatter: NumericRuleFormatter
```

Creates a numeric formatter that converts numbers to strings with flexible rulesets.

### CreateSecondsFormatter

```lua
C_StringUtil.CreateSecondsFormatter() -> formatter: SecondsFormatter
```

Creates a numeric formatter that converts numbers measuring durations in seconds to strings, eg. 93 -> '1m 33s'.

### EscapeDecimalNonPrintables

```lua
C_StringUtil.EscapeDecimalNonPrintables(text: stringView) -> escapedText: string
```

Returns a string with ASCII control characters (except \n, \r, and \t) and invalid UTF-8 bytes replaced by decimal escape sequences (e.g. \127).

`SecretArguments=AllowedWhenTainted`

### EscapeLuaFormatString

```lua
C_StringUtil.EscapeLuaFormatString(text: string) -> escapedText: stringView
```

Returns a string with Lua format string tokens ('%') escaped.

`SecretArguments=AllowedWhenTainted`

### EscapeLuaPatterns

```lua
C_StringUtil.EscapeLuaPatterns(text: stringView) -> escapedText: string
```

Returns a string with all Lua pattern characters escaped.

`SecretArguments=AllowedWhenTainted`

### EscapeQuotedCodes

```lua
C_StringUtil.EscapeQuotedCodes(text: string) -> escaped: stringView
```

Returns a string with all quoted code sequences ('|' characters) escaped.

`SecretArguments=AllowedWhenTainted`

### FloorToNearestString

```lua
C_StringUtil.FloorToNearestString(number: number) -> text: string
```

`SecretArguments=AllowedWhenTainted`

### RemoveContiguousSpaces

```lua
C_StringUtil.RemoveContiguousSpaces(text: stringView, maxAllowedSpaces: number) -> trimmedText: string
```

Returns a string with all contiguous occurrences of ASCII space characters truncated.

`SecretArguments=AllowedWhenTainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `text` | `stringView` |  |
| `maxAllowedSpaces` | `number` | Maximum number of permitted contiguous space characters; excessive spaces will be truncated to this count.; `NeverSecret` |

### RoundToNearestString

```lua
C_StringUtil.RoundToNearestString(number: number) -> text: string
```

`SecretArguments=AllowedWhenTainted`

### StripHyperlinks

```lua
C_StringUtil.StripHyperlinks(text: string, maintainColor: bool, maintainBrackets: bool, stripNewlines: bool, maintainAtlases: bool, maintainTextures: bool) -> stripped: stringView
```

`SecretArguments=AllowedWhenTainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `text` | `string` |  |
| `maintainColor` | `bool` | default `false`; If true, preserve all '\|c' and '\|r' quoted code sequences. |
| `maintainBrackets` | `bool` | default `false`; If true, preserve all '[' and ']' characters. |
| `stripNewlines` | `bool` | default `false`; If true, remove all '\|n' quoted code sequences. |
| `maintainAtlases` | `bool` | default `false`; If true, preserve all balanced '\|A' and '\|a' quoted code sequences. |
| `maintainTextures` | `bool` | default `false`; If true, preserve all balanced '\|T' and '\|t' quoted code sequences. |

### StripTextureMarkupForLooseFiles

```lua
C_StringUtil.StripTextureMarkupForLooseFiles(text: string) -> stripped: stringView
```

`SecretArguments=AllowedWhenTainted`

### TruncateWhenZero

```lua
C_StringUtil.TruncateWhenZero(number: number) -> text: string
```

Formats the given number to a string as an integer (rounding down). If the integer is zero, returns an empty string.

`SecretArguments=AllowedWhenTainted`

### WrapString

```lua
C_StringUtil.WrapString(infix: stringView, prefix: stringView?, suffix: stringView?) -> text: string
```

Returns a string with 'prefix' and 'suffix' joined to 'infix' iif 'infix' is not an empty string. Else, an empty string is returned.

`SecretArguments=AllowedWhenTainted`

## Types

### StripHyperlinkOptions

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `maintainColor` | `bool` | default `false`; If true, preserve all '\|c' and '\|r' quoted code sequences. |
| `maintainBrackets` | `bool` | default `false`; If true, preserve all '[' and ']' characters. |
| `stripNewlines` | `bool` | default `false`; If true, remove all '\|n' quoted code sequences. |
| `maintainAtlases` | `bool` | default `false`; If true, preserve all balanced '\|A' and '\|a' quoted code sequences. |
| `maintainTextures` | `bool` | default `false`; If true, preserve all balanced '\|T' and '\|t' quoted code sequences. |
