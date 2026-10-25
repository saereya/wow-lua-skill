# Locale

Global functions · environment All · source `interface/addons/blizzard_apidocumentationgenerated/localedocumentation.lua` (FileDataID 5200990)

## Functions

### GetAvailableLocaleInfo

```lua
GetAvailableLocaleInfo(ignoreLocaleRestrictions: bool) -> localeInfos: LocaleInfo[]
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `ignoreLocaleRestrictions` | `bool` | default `false` |

### GetAvailableLocales

```lua
GetAvailableLocales(ignoreLocaleRestrictions: bool) -> localeName: cstring
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `ignoreLocaleRestrictions` | `bool` | default `false` |

Returns:

| Name | Type | Notes |
|---|---|---|
| `localeName` | `cstring` | `StrideIndex=1` |

### GetCurrentRegion

```lua
GetCurrentRegion() -> region: number
```

### GetLocale

```lua
GetLocale() -> localeName: cstring
```

### GetOSLocale

```lua
GetOSLocale() -> localeName: cstring
```

## Types

### LocaleInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `localeId` | `number` |  |
| `localeName` | `cstring` |  |
