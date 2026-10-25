# PlayerLocationInfo

Namespace `C_PlayerInfo` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/playerlocationdocumentation.lua` (FileDataID 4637164)

## Functions

### GetClass

```lua
C_PlayerInfo.GetClass(playerLocation: PlayerLocation) -> className: cstring?, classFilename: cstring?, classID: number?
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `playerLocation` | `PlayerLocation` | `Mixin=PlayerLocationMixin` |

### GetName

```lua
C_PlayerInfo.GetName(playerLocation: PlayerLocation) -> name: string
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `playerLocation` | `PlayerLocation` | `Mixin=PlayerLocationMixin` |

### GetRace

```lua
C_PlayerInfo.GetRace(playerLocation: PlayerLocation) -> raceID: number?
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `playerLocation` | `PlayerLocation` | `Mixin=PlayerLocationMixin` |

### GetSex

```lua
C_PlayerInfo.GetSex(playerLocation: PlayerLocation) -> sex: UnitSex?
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `playerLocation` | `PlayerLocation` | `Mixin=PlayerLocationMixin` |

### GUIDIsPlayer

```lua
C_PlayerInfo.GUIDIsPlayer(guid: WOWGUID) -> isPlayer: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsConnected

```lua
C_PlayerInfo.IsConnected(playerLocation: PlayerLocation?) -> isConnected: bool?
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `playerLocation` | `PlayerLocation?` | `Mixin=PlayerLocationMixin` |

### UnitIsSameServer

```lua
C_PlayerInfo.UnitIsSameServer(playerLocation: PlayerLocation) -> unitIsSameServer: bool
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `playerLocation` | `PlayerLocation` | `Mixin=PlayerLocationMixin` |
