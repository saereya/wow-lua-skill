# DeathInfo

Namespace `C_DeathInfo` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/deathinfodocumentation.lua` (FileDataID 4637078)

## Functions

### GetCorpseMapPosition

```lua
C_DeathInfo.GetCorpseMapPosition(uiMapID: number) -> position: vector2?
```

`SecretArguments=AllowedWhenUntainted`

Returns:

| Name | Type | Notes |
|---|---|---|
| `position` | `vector2?` | `Mixin=Vector2DMixin` |

### GetDeathReleasePosition

```lua
C_DeathInfo.GetDeathReleasePosition(uiMapID: number) -> position: vector2?
```

`SecretArguments=AllowedWhenUntainted`

Returns:

| Name | Type | Notes |
|---|---|---|
| `position` | `vector2?` | `Mixin=Vector2DMixin` |

### GetGraveyardsForMap

```lua
C_DeathInfo.GetGraveyardsForMap(uiMapID: number) -> graveyards: GraveyardMapInfo[]
```

`SecretArguments=AllowedWhenUntainted`

### GetSelfResurrectOptions

```lua
C_DeathInfo.GetSelfResurrectOptions() -> options: SelfResurrectOption[]
```

`MayReturnNothing`

### UseSelfResurrectOption

```lua
C_DeathInfo.UseSelfResurrectOption(optionType: SelfResurrectOptionType, id: number)
```

`SecretArguments=AllowedWhenUntainted`

## Events

### AREA_SPIRIT_HEALER_IN_RANGE

```lua
AREA_SPIRIT_HEALER_IN_RANGE()
```

`SynchronousEvent`

### AREA_SPIRIT_HEALER_OUT_OF_RANGE

```lua
AREA_SPIRIT_HEALER_OUT_OF_RANGE()
```

`SynchronousEvent`

### CEMETERY_PREFERENCE_UPDATED

```lua
CEMETERY_PREFERENCE_UPDATED()
```

`SynchronousEvent`

### CONFIRM_XP_LOSS

```lua
CONFIRM_XP_LOSS()
```

`SynchronousEvent`

### CORPSE_IN_INSTANCE

```lua
CORPSE_IN_INSTANCE()
```

`SynchronousEvent`

### CORPSE_IN_RANGE

```lua
CORPSE_IN_RANGE()
```

`SynchronousEvent`

### CORPSE_OUT_OF_RANGE

```lua
CORPSE_OUT_OF_RANGE()
```

`SynchronousEvent`

### PLAYER_ALIVE

```lua
PLAYER_ALIVE()
```

`SynchronousEvent`

### PLAYER_DEAD

```lua
PLAYER_DEAD()
```

`SynchronousEvent`

### PLAYER_SKINNED

```lua
PLAYER_SKINNED(hasFreeRepop: number)
```

`SynchronousEvent`

### PLAYER_UNGHOST

```lua
PLAYER_UNGHOST()
```

`SynchronousEvent`

### REQUEST_CEMETERY_LIST_RESPONSE

```lua
REQUEST_CEMETERY_LIST_RESPONSE(isGossipTriggered: bool)
```

`SynchronousEvent`

### RESURRECT_REQUEST

```lua
RESURRECT_REQUEST(inviter: cstring)
```

`SynchronousEvent`

### SELF_RES_SPELL_CHANGED

```lua
SELF_RES_SPELL_CHANGED()
```

`SynchronousEvent`

## Types

### SelfResurrectOptionType

*Enumeration* · 2 values, 0..1

Access values as `Enum.SelfResurrectOptionType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Spell` | `SelfResurrectOptionType` | = 0 |
| `Item` | `SelfResurrectOptionType` | = 1 |

### GraveyardMapInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `areaPoiID` | `number` |  |
| `position` | `vector2` | `Mixin=Vector2DMixin` |
| `name` | `cstring` |  |
| `textureIndex` | `number` |  |
| `graveyardID` | `number` |  |
| `isGraveyardSelectable` | `bool` |  |

### SelfResurrectOption

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `string` |  |
| `optionType` | `SelfResurrectOptionType` |  |
| `id` | `number` |  |
| `canUse` | `bool` |  |
| `isLimited` | `bool` |  |
| `priority` | `number` |  |
