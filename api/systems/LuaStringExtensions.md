# LuaStringExtensions

Namespace `string` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/luastringextensionsdocumentation.lua` (FileDataID 8293695)

## Functions

### contains

```lua
string.contains(str: stringView, substring: stringView) -> contains: bool
```

Returns true if a string contains the specified literal substring.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `str` | `stringView` | The string to search. |
| `substring` | `stringView` | The literal substring for which to search. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `contains` | `bool` | True if the string contains the specified substring; otherwise false. |

### endswith

```lua
string.endswith(str: stringView, suffix: stringView) -> endsWith: bool
```

Returns true if a string ends with the specified suffix.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `str` | `stringView` | The string to inspect. |
| `suffix` | `stringView` | The suffix for which to search. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `endsWith` | `bool` | True if the string ends with the specified suffix; otherwise false. |

### ltrim

```lua
string.ltrim(str: stringView, characters: stringView) -> trimmed: stringView
```

Returns a string with all bytes in the specified character set removed from the start.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `str` | `stringView` | The string to trim. |
| `characters` | `stringView` | default `" \\r\\n\\t"`; The set of bytes to remove. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `trimmed` | `stringView` | The left-trimmed string. |

### rtrim

```lua
string.rtrim(str: stringView, characters: stringView) -> trimmed: stringView
```

Returns a string with all bytes in the specified character set removed from the end.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `str` | `stringView` | The string to trim. |
| `characters` | `stringView` | default `" \\r\\n\\t"`; The set of bytes to remove. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `trimmed` | `stringView` | The right-trimmed string. |

### startswith

```lua
string.startswith(str: stringView, prefix: stringView) -> startsWith: bool
```

Returns true if a string starts with the specified prefix.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `str` | `stringView` | The string to inspect. |
| `prefix` | `stringView` | The prefix for which to search. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `startsWith` | `bool` | True if the string starts with the specified prefix; otherwise false. |

### trim

```lua
string.trim(str: stringView, characters: stringView) -> trimmed: stringView
```

Returns a string with all bytes in the specified character set removed from both ends.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `str` | `stringView` | The string to trim. |
| `characters` | `stringView` | default `" \\r\\n\\t"`; The set of bytes to remove. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `trimmed` | `stringView` | The trimmed string. |
