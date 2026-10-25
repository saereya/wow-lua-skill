# CombatLog

Namespace `C_CombatLog` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/combatlogdocumentation.lua` (FileDataID 4637055)

## Functions

### ApplyFilterSettings

```lua
C_CombatLog.ApplyFilterSettings(filterSettings: LuaValueVariant)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### AreFilteredEventsEnabled

```lua
C_CombatLog.AreFilteredEventsEnabled() -> enabled: bool
```

### ClearEntries

```lua
C_CombatLog.ClearEntries()
```

### DoesObjectMatchFilter

```lua
C_CombatLog.DoesObjectMatchFilter(mask: CombatLogObject, flags: CombatLogObject) -> matches: bool
```

`SecretArguments=AllowedWhenUntainted`

### GetEntryRetentionTime

```lua
C_CombatLog.GetEntryRetentionTime() -> retentionTime: number
```

### GetMessageLimit

```lua
C_CombatLog.GetMessageLimit() -> messageLimit: number
```

### IsCombatLogRestricted

```lua
C_CombatLog.IsCombatLogRestricted() -> restricted: bool
```

### RefilterEntries

```lua
C_CombatLog.RefilterEntries()
```

### SetEntryRetentionTime

```lua
C_CombatLog.SetEntryRetentionTime(retentionTime: number)
```

`SecretArguments=AllowedWhenUntainted`

### SetFilteredEventsEnabled

```lua
C_CombatLog.SetFilteredEventsEnabled(enabled: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetMessageLimit

```lua
C_CombatLog.SetMessageLimit(messageLimit: number)
```

`SecretArguments=AllowedWhenUntainted`

## Events

### COMBAT_LOG_ENTRIES_CLEARED

```lua
COMBAT_LOG_ENTRIES_CLEARED()
```

`SynchronousEvent`

### COMBAT_LOG_EVENT

```lua
COMBAT_LOG_EVENT()
```

`HasRestrictions` `SynchronousEvent` `CallbackEvent`

### COMBAT_LOG_EVENT_UNFILTERED

```lua
COMBAT_LOG_EVENT_UNFILTERED()
```

`HasRestrictions` `SynchronousEvent` `CallbackEvent`

### COMBAT_LOG_MESSAGE_LIMIT_CHANGED

```lua
COMBAT_LOG_MESSAGE_LIMIT_CHANGED(messageLimit: number)
```

`SynchronousEvent`
