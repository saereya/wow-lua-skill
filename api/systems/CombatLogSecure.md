# CombatLogSecure

Namespace `C_CombatLogSecure` · environment SecureOnly · source `interface/addons/blizzard_apidocumentationgenerated/combatlogsecuredocumentation.lua` (FileDataID 7036077)

## Functions

### AddEventFilter

```lua
C_CombatLogSecure.AddEventFilter()
```

`HasRestrictions`

### ClearEventFilters

```lua
C_CombatLogSecure.ClearEventFilters()
```

`HasRestrictions`

### CreateCombatLogMessage

```lua
C_CombatLogSecure.CreateCombatLogMessage(message: string, colorR: number, colorG: number, colorB: number, order: CombatLogMessageOrder)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### GetCurrentEntryInfo

```lua
C_CombatLogSecure.GetCurrentEntryInfo()
```

`HasRestrictions`

### GetCurrentEventInfo

```lua
C_CombatLogSecure.GetCurrentEventInfo()
```

`HasRestrictions`

### GetEntryCount

```lua
C_CombatLogSecure.GetEntryCount(ignoreFilter: bool) -> count: number
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `ignoreFilter` | `bool` | default `false` |

### SeekToNewestEntry

```lua
C_CombatLogSecure.SeekToNewestEntry(ignoreFilter: bool) -> isValidEntry: bool
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `ignoreFilter` | `bool` | default `false` |

### SeekToPreviousEntry

```lua
C_CombatLogSecure.SeekToPreviousEntry(ignoreFilter: bool) -> isValidEntry: bool
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `ignoreFilter` | `bool` | default `false` |

### ShouldShowCurrentEntry

```lua
C_CombatLogSecure.ShouldShowCurrentEntry() -> shouldShow: bool
```

`HasRestrictions`

## Events

### COMBAT_LOG_APPLY_FILTER_SETTINGS

```lua
COMBAT_LOG_APPLY_FILTER_SETTINGS(filterSettings: LuaValueVariant)
```

`HasRestrictions` `CallbackEvent`

### COMBAT_LOG_MESSAGE

```lua
COMBAT_LOG_MESSAGE(message: string, colorR: number, colorG: number, colorB: number, order: CombatLogMessageOrder)
```

`SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `message` | `string` | A preformatted combat log message protected by a \|K string wrapper. |
| `colorR` | `number` |  |
| `colorG` | `number` |  |
| `colorB` | `number` |  |
| `order` | `CombatLogMessageOrder` |  |

### COMBAT_LOG_REFILTER_ENTRIES

```lua
COMBAT_LOG_REFILTER_ENTRIES()
```

`HasRestrictions` `CallbackEvent`
