# Localization

Global functions · environment All · source `interface/addons/blizzard_apidocumentationgenerated/localizationdocumentation.lua` (FileDataID 5200992)

## Functions

### AbbreviateLargeNumbers

```lua
AbbreviateLargeNumbers(number: number, options: NumberAbbrevOptions?) -> result: string
```

`SecretArguments=AllowedWhenTainted`

### AbbreviateNumbers

```lua
AbbreviateNumbers(number: number, options: NumberAbbrevOptions?) -> result: string
```

`SecretArguments=AllowedWhenTainted`

### BreakUpLargeNumbers

```lua
BreakUpLargeNumbers(largeNumber: number, natural: bool) -> result: string
```

`SecretArguments=AllowedWhenTainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `largeNumber` | `number` |  |
| `natural` | `bool` | default `false`; `NeverSecret` |

### CaseAccentInsensitiveParse

```lua
CaseAccentInsensitiveParse(name: cstring) -> result: string
```

`SecretArguments=AllowedWhenUntainted`

### CreateAbbreviateConfig

```lua
CreateAbbreviateConfig(data: NumberAbbreviationBreakpoint[]) -> config: AbbreviateConfig
```

`SecretArguments=NotAllowed` `RequiresRestrictedAbbreviationBreakpoints`

### DeclineName

```lua
DeclineName(name: cstring, gender: UnitSex?, declensionSet: luaIndex, namePartType: NamePartType?) -> declinedNames: string
```

`SecretArguments=AllowedWhenUntainted`

Returns:

| Name | Type | Notes |
|---|---|---|
| `declinedNames` | `string` | `StrideIndex=1` |

### GetDefaultAbbreviationBreakpoints

```lua
GetDefaultAbbreviationBreakpoints(locale: WowLocale?) -> breakpoints: NumberAbbreviationBreakpoint[]
```

`SecretArguments=AllowedWhenUntainted` `Namespace=C_StringUtil`

### GetNumDeclensionSets

```lua
GetNumDeclensionSets(name: cstring, gender: UnitSex?, namePartType: NamePartType?) -> numDeclensionSets: number
```

`SecretArguments=AllowedWhenUntainted`

### IsEuropeanNumbers

```lua
IsEuropeanNumbers() -> enabled: bool
```

### LocalizedClassList

```lua
LocalizedClassList(isFemale: bool) -> result: LuaValueVariant
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `isFemale` | `bool` | default `false` |

### SetEuropeanNumbers

```lua
SetEuropeanNumbers(enabled: bool)
```

`SecretArguments=AllowedWhenUntainted`

## Types

### NumberAbbrevOptions

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `breakpointData` | `NumberAbbreviationBreakpoint[]?` | Order these from largest to smallest. |
| `locale` | `cstring?` | Locale controls whether standard asian abbreviation data will be used along with a small change in behavior for large number abbreviation when fractionDivisor is greater than zero. |
| `config` | `AbbreviateConfig?` | Provides a cached config object for optimal performance when calling abbreviation functions multiple times with the same options. |
