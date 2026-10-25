# LuaLocaleContext

Widget methods (`LuaLocaleContextAPI`) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/lualocalecontextapidocumentation.lua` (FileDataID 8281693)

## Methods

### CompareStrings

```lua
LuaLocaleContext:CompareStrings(left: cstring, right: cstring, strength: CollationStrength) -> result: number
```

Compares two UTF-8 strings using the options specified on a collator.

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `left` | `cstring` | The first UTF-8 string passed to collation comparison. |
| `right` | `cstring` | The second UTF-8 string passed to collation comparison. |
| `strength` | `CollationStrength` | The comparison level used by the collator for ordering and equality. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `result` | `number` | The comparison result: less than, equal to, or greater than zero. |

### FindBreaks

```lua
LuaLocaleContext:FindBreaks(text: cstring, breakType: BreakType) -> byteOffsets: luaIndex[]
```

Opens a break iterator for locating text boundaries in the context locale.

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` | The UTF-8 text whose boundary offsets are requested. |
| `breakType` | `BreakType` | The break iterator kind to use for boundary analysis. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `byteOffsets` | `luaIndex[]` | The native UTF-8 string indices for the text boundaries (returned with 1-based indexes for lua convenience). |

### FindStringMatches

```lua
LuaLocaleContext:FindStringMatches(text: cstring, pattern: cstring, strength: CollationStrength) -> byteOffsets: luaIndex[]
```

Creates a string search iterator using a collator and returns every match position.

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` | The UTF-8 text scanned by the string search iterator. |
| `pattern` | `cstring` | The UTF-8 pattern whose collation-aware matches are returned. |
| `strength` | `CollationStrength` | The comparison level used by the collator while searching for matches. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `byteOffsets` | `luaIndex[]` | The UTF-8 byte offsets of matches in the text (returned with 1-based indexes for lua convenience). |

### FoldCase

```lua
LuaLocaleContext:FoldCase(text: cstring) -> result: string
```

Case-folds the characters in a string; case-folding is locale-independent and not context-sensitive.

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` | The UTF-8 text converted with locale-independent case folding. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `result` | `string` | The case-folded string, which may be longer or shorter than the original. |

### FormatCurrency

```lua
LuaLocaleContext:FormatCurrency(number: number, currencyCode: cstring) -> result: string
```

Formats a double as a localized currency value using the provided ISO 4217 currency code.

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `number` | `number` | The double value formatted by the locale currency formatter. |
| `currencyCode` | `cstring` | The 3-letter null-terminated ISO 4217 currency code for currency formatting. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `result` | `string` | The localized currency text produced by the formatter. |

### FormatDate

```lua
LuaLocaleContext:FormatDate(unixTimeSeconds: number, style: DateTimeStyle, timeZone: cstring) -> result: string
```

Formats Unix time as localized date text using locale date patterns, symbols, style, and optional time zone.

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `unixTimeSeconds` | `number` | The date as seconds since the Unix epoch; this API converts it to milliseconds. |
| `style` | `DateTimeStyle` | The date format length; None omits the date portion. |
| `timeZone` | `cstring` | The time zone ID applied to the formatter; empty strings keep the formatter default. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `result` | `string` | The formatted date string. |

### FormatDateTime

```lua
LuaLocaleContext:FormatDateTime(unixTimeSeconds: number, dateStyle: DateTimeStyle, timeStyle: DateTimeStyle, timeZone: cstring) -> result: string
```

Formats Unix time as localized date and time text using locale patterns, symbols, styles, and optional time zone.

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `unixTimeSeconds` | `number` | The date and time as seconds since the Unix epoch; this API converts it to milliseconds. |
| `dateStyle` | `DateTimeStyle` | The date format length; None omits the date portion. |
| `timeStyle` | `DateTimeStyle` | The time format length; None omits the time portion. |
| `timeZone` | `cstring` | The time zone ID applied to the formatter; empty strings keep the formatter default. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `result` | `string` | The formatted date and time string. |

### FormatNumber

```lua
LuaLocaleContext:FormatNumber(number: number, style: NumberStyle) -> result: string
```

Formats a double with locale number formatting using locale symbols, grouping, and the selected non-currency style.

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `number` | `number` | The double value formatted according to the selected number formatter. |
| `style` | `NumberStyle` | The number style to format with; Currency is not accepted here, use FormatCurrency instead. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `result` | `string` | The localized number text produced by the formatter. |

### FormatTime

```lua
LuaLocaleContext:FormatTime(unixTimeSeconds: number, style: DateTimeStyle, timeZone: cstring) -> result: string
```

Formats Unix time as localized time text using locale time patterns, symbols, style, and optional time zone.

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `unixTimeSeconds` | `number` | The time as seconds since the Unix epoch; this API converts it to milliseconds. |
| `style` | `DateTimeStyle` | The time format length; None omits the time portion. |
| `timeZone` | `cstring` | The time zone ID applied to the formatter; empty strings keep the formatter default. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `result` | `string` | The formatted time string. |

### GetCurrencyName

```lua
LuaLocaleContext:GetCurrencyName(currencyCode: cstring, style: CurrencyNameStyle) -> result: string
```

Returns the display name for a currency in the context locale.

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `currencyCode` | `cstring` | The null-terminated 3-letter ISO 4217 currency code. |
| `style` | `CurrencyNameStyle` | The selector for which kind of currency name to return. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `result` | `string` | The display string for the currency, or the currency code itself if no localized name is available. |

### GetDisplayName

```lua
LuaLocaleContext:GetDisplayName(displayLocale: cstring) -> result: string
```

Gets a display name suitable for the specified locale.

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `displayLocale` | `cstring` | The locale whose language conventions are used for the display name |

Returns:

| Name | Type | Notes |
|---|---|---|
| `result` | `string` | The displayable name for the locale. |

### GetLocale

```lua
LuaLocaleContext:GetLocale() -> result: string
```

Gets the locale used by this locale context.

Returns:

| Name | Type | Notes |
|---|---|---|
| `result` | `string` | The locale ID of this locale context. |

### GetSortKey

```lua
LuaLocaleContext:GetSortKey(text: cstring, strength: CollationStrength) -> result: string
```

Transforms a string into a collation sort key.

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` | The UTF-8 text converted into collation sort-key bytes. |
| `strength` | `CollationStrength` | The comparison level used by the collator; lower strengths ignore later-level differences. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `result` | `string` | The sort key bytes excluding the terminating zero byte. |

### Length

```lua
LuaLocaleContext:Length(text: cstring) -> result: number
```

Counts character break boundaries in UTF-8 text.

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` | The UTF-8 text counted by character break iteration. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `result` | `number` | The number of character boundaries minus the initial boundary. |

### ParseCurrency

```lua
LuaLocaleContext:ParseCurrency(text: cstring) -> result: CurrencyParseResult
```

Parses an entire localized currency string into a double amount and ISO 4217 currency code.

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` | The localized currency text to parse for both amount and ISO 4217 code. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `result` | `CurrencyParseResult` | The numeric amount and ISO 4217 currency code parsed from the localized currency text. |

### ParseNumber

```lua
LuaLocaleContext:ParseNumber(text: cstring, style: NumberStyle) -> result: number
```

Parses an entire localized number string into a double using the selected non-currency number formatter.

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` | The localized numeric text to parse with the selected style. |
| `style` | `NumberStyle` | The number style to parse with; Currency is not accepted here, use ParseCurrency instead. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `result` | `number` | The numeric value parsed from the localized number text. |

### SelectPlural

```lua
LuaLocaleContext:SelectPlural(number: number, pluralType: PluralType) -> result: string
```

Returns the keyword of the first plural rule that applies to a number.

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `number` | `number` | The number for which the plural rule has to be determined. |
| `pluralType` | `PluralType` | The plural rule type, cardinal or ordinal. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `result` | `string` | The plural keyword for the rule that applies to the number. |

### SetLocale

```lua
LuaLocaleContext:SetLocale(locale: cstring) -> success: bool
```

Sets the locale used by this locale context.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `locale` | `cstring` | The locale ID used by subsequent locale context calls. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `success` | `bool` | True if the locale was updated. |

### ToLower

```lua
LuaLocaleContext:ToLower(text: cstring) -> result: string
```

Lowercases the characters in a string; casing is locale-dependent and context-sensitive.

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` | The UTF-8 text whose characters are lowercased. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `result` | `string` | The lowercased string, which may be longer or shorter than the original. |

### ToTitle

```lua
LuaLocaleContext:ToTitle(text: cstring) -> result: string
```

Titlecases a string using titlecase positions determined by the default Unicode algorithm.

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` | The UTF-8 text whose titlecase positions are mapped. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `result` | `string` | The titlecased string, which may be longer or shorter than the original. |

### ToUpper

```lua
LuaLocaleContext:ToUpper(text: cstring) -> result: string
```

Uppercases the characters in a string; casing is locale-dependent and context-sensitive.

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `text` | `cstring` | The UTF-8 text whose characters are uppercased. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `result` | `string` | The uppercased string, which may be longer or shorter than the original. |

### TransformLocale

```lua
LuaLocaleContext:TransformLocale(transform: LocaleTransform) -> result: string
```

Applies a locale transform to the context locale and returns the transformed locale string.

`SecretArguments=AllowedWhenTainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `transform` | `LocaleTransform` | The locale transform to apply. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `result` | `string` | The transformed locale string. |
