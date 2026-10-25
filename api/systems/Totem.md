# Totem

Global functions · environment All · source `interface/addons/blizzard_apidocumentationgenerated/totemdocumentation.lua` (FileDataID 5559830)

## Functions

### DestroyTotem

```lua
DestroyTotem(slot: luaIndex)
```

`SecretArguments=AllowedWhenUntainted`

### GetNumTotemSlots

```lua
GetNumTotemSlots() -> numSlots: number
```

### GetTotemCannotDismiss

```lua
GetTotemCannotDismiss(slot: luaIndex) -> cannotDismiss: bool?
```

`SecretArguments=AllowedWhenUntainted`

### GetTotemDuration

```lua
GetTotemDuration(slot: luaIndex) -> duration: LuaDurationObject
```

`SecretArguments=AllowedWhenUntainted`

### GetTotemInfo

```lua
GetTotemInfo(slot: luaIndex) -> haveTotem: bool, totemName: cstring, startTime: number, duration: number, icon: fileID, modRate: number, spellID: number
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing` `SecretWhenTotemSlotSecret`

### GetTotemTimeLeft

```lua
GetTotemTimeLeft(slot: luaIndex) -> timeLeft: number?
```

`SecretArguments=AllowedWhenUntainted` `SecretWhenTotemSlotSecret`

### TargetTotem

```lua
TargetTotem(slot: luaIndex)
```

`SecretArguments=AllowedWhenUntainted`

## Types

### TotemInfoScript

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `haveTotem` | `bool` |  |
| `totemName` | `cstring` |  |
| `startTime` | `number` |  |
| `duration` | `number` |  |
| `icon` | `fileID` |  |
| `modRate` | `number` |  |
| `spellID` | `number` |  |
