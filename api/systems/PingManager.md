# PingManager

Namespace `C_Ping` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/pingmanagerdocumentation.lua` (FileDataID 5279564)

## Functions

### GetCooldownInfo

```lua
C_Ping.GetCooldownInfo() -> cooldownInfo: PingCooldownInfo
```

### GetDefaultPingOptions

```lua
C_Ping.GetDefaultPingOptions() -> pingTypes: PingTypeInfo[]
```

### GetTextureKitForType

```lua
C_Ping.GetTextureKitForType(type: PingSubjectType) -> uiTextureKitID: textureKit
```

`SecretArguments=AllowedWhenUntainted`

### IsPingSystemEnabled

```lua
C_Ping.IsPingSystemEnabled() -> isEnabled: bool
```

### SendMacroPing

```lua
C_Ping.SendMacroPing(macroInfo: PingMacroInfo)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### TogglePingListener

```lua
C_Ping.TogglePingListener(down: bool)
```

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

## Events

### PING_SYSTEM_ERROR

```lua
PING_SYSTEM_ERROR(error: cstring)
```

`SynchronousEvent`

## Types

### PingTypeInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `orderIndex` | `number` |  |
| `type` | `PingSubjectType` |  |
| `uiTextureKitID` | `textureKit` |  |
