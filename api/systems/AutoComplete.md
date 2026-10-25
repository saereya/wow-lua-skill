# AutoComplete

Namespace `C_AutoComplete` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/autocompletedocumentation.lua` (FileDataID 7733453)

## Functions

### GetAutoCompletePresenceID

```lua
C_AutoComplete.GetAutoCompletePresenceID(name: cstring) -> presenceID: number?
```

`SecretArguments=AllowedWhenUntainted`

### GetAutoCompleteRealms

```lua
C_AutoComplete.GetAutoCompleteRealms() -> realms: string[]
```

### GetAutoCompleteResults

```lua
C_AutoComplete.GetAutoCompleteResults(name: cstring, numResults: number, cursorPosition: number, allowFullMatch: bool, includeFlags: number, excludeFlags: number) -> results: AutoCompleteResult[]
```

`SecretArguments=AllowedWhenUntainted`

### IsRecognizedName

```lua
C_AutoComplete.IsRecognizedName(name: cstring, includeFlags: number, excludeFlags: number) -> isRecognizedName: bool
```

`SecretArguments=AllowedWhenUntainted`

## Types

### AutoCompleteResult

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `string` |  |
| `priority` | `AutoCompletePriority` |  |
| `bnetID` | `number` |  |
