# ConnectionScript

Global functions · environment All · source `interface/addons/blizzard_apidocumentationgenerated/connectiondocumentation.lua` (FileDataID 5535950)

## Functions

### CancelLogout

```lua
CancelLogout()
```

### ForceLogout

```lua
ForceLogout()
```

### ForceQuit

```lua
ForceQuit()
```

### GetNativeRealmID

```lua
GetNativeRealmID() -> nativeRealmID: number
```

### GetNetIpTypes

```lua
GetNetIpTypes() -> ipTypes: ConnectionIptype
```

Returns:

| Name | Type | Notes |
|---|---|---|
| `ipTypes` | `ConnectionIptype` | `StrideIndex=1` |

### GetNetStats

```lua
GetNetStats() -> in: number, out: number, latencyList: number
```

Returns:

| Name | Type | Notes |
|---|---|---|
| `in` | `number` |  |
| `out` | `number` |  |
| `latencyList` | `number` | `StrideIndex=1` |

### GetProtocolTypes

```lua
GetProtocolTypes() -> protocolTypes: ConnectionProtocol
```

Returns:

| Name | Type | Notes |
|---|---|---|
| `protocolTypes` | `ConnectionProtocol` | `StrideIndex=1` |

### GetRealmID

```lua
GetRealmID() -> realmID: number
```

### GetRealmName

```lua
GetRealmName() -> realmName: cstring
```

### IsOnTournamentRealm

```lua
IsOnTournamentRealm() -> result: bool
```

### Logout

```lua
Logout()
```

### Quit

```lua
Quit()
```

### SelectedRealmName

```lua
SelectedRealmName() -> selectedRealmName: cstring
```
