# ItemSocketInfo

Namespace `C_ItemSocketInfo` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/itemsocketinfodocumentation.lua` (FileDataID 4637124)

## Functions

### AcceptSockets

```lua
C_ItemSocketInfo.AcceptSockets()
```

### ClickSocketButton

```lua
C_ItemSocketInfo.ClickSocketButton(index: luaIndex)
```

`SecretArguments=AllowedWhenUntainted`

### CloseSocketInfo

```lua
C_ItemSocketInfo.CloseSocketInfo()
```

### CompleteSocketing

```lua
C_ItemSocketInfo.CompleteSocketing()
```

### GetCurrUIType

```lua
C_ItemSocketInfo.GetCurrUIType() -> uiType: ItemSocketInfoUIType
```

### GetExistingSocketInfo

```lua
C_ItemSocketInfo.GetExistingSocketInfo(index: luaIndex) -> name: string?, icon: fileID?, gemMatchesSocket: bool
```

`SecretArguments=AllowedWhenUntainted`

### GetExistingSocketLink

```lua
C_ItemSocketInfo.GetExistingSocketLink(index: luaIndex) -> existingSocketLink: string?
```

`SecretArguments=AllowedWhenUntainted`

### GetNewSocketInfo

```lua
C_ItemSocketInfo.GetNewSocketInfo(index: luaIndex) -> name: string?, icon: fileID?, gemMatchesSocket: bool
```

`SecretArguments=AllowedWhenUntainted`

### GetNewSocketLink

```lua
C_ItemSocketInfo.GetNewSocketLink(index: luaIndex) -> newSocketLink: string?
```

`SecretArguments=AllowedWhenUntainted`

### GetNumSockets

```lua
C_ItemSocketInfo.GetNumSockets() -> numSockets: number
```

### GetSocketItemBoundTradeable

```lua
C_ItemSocketInfo.GetSocketItemBoundTradeable() -> socketItemTradeable: bool
```

### GetSocketItemInfo

```lua
C_ItemSocketInfo.GetSocketItemInfo() -> name: string?, icon: fileID?, quality: ItemQuality
```

### GetSocketItemRefundable

```lua
C_ItemSocketInfo.GetSocketItemRefundable() -> socketItemRefundable: bool
```

### GetSocketTypes

```lua
C_ItemSocketInfo.GetSocketTypes(index: luaIndex) -> socketType: string?
```

`SecretArguments=AllowedWhenUntainted`

### HasBoundGemProposed

```lua
C_ItemSocketInfo.HasBoundGemProposed() -> hasBoundGemProposed: bool
```

### IsArtifactRelicItem

```lua
C_ItemSocketInfo.IsArtifactRelicItem(info: ItemInfo) -> isArtifactRelicItem: bool
```

`SecretArguments=AllowedWhenUntainted`

## Events

### SOCKET_INFO_ACCEPT

```lua
SOCKET_INFO_ACCEPT()
```

`SynchronousEvent`

### SOCKET_INFO_BIND_CONFIRM

```lua
SOCKET_INFO_BIND_CONFIRM()
```

`SynchronousEvent`

### SOCKET_INFO_CLOSE

```lua
SOCKET_INFO_CLOSE()
```

`SynchronousEvent`

### SOCKET_INFO_FAILURE

```lua
SOCKET_INFO_FAILURE()
```

`SynchronousEvent`

### SOCKET_INFO_REFUNDABLE_CONFIRM

```lua
SOCKET_INFO_REFUNDABLE_CONFIRM()
```

`SynchronousEvent`

### SOCKET_INFO_SUCCESS

```lua
SOCKET_INFO_SUCCESS()
```

`SynchronousEvent`

### SOCKET_INFO_UI_EVENT_REGISTRATION_UPDATE

```lua
SOCKET_INFO_UI_EVENT_REGISTRATION_UPDATE(uiType: ItemSocketInfoUIType)
```

`SynchronousEvent`

### SOCKET_INFO_UPDATE

```lua
SOCKET_INFO_UPDATE()
```

`SynchronousEvent`

## Types

### ItemSocketInfoUIType

*Enumeration* · 1 values, 0..0

Access values as `Enum.ItemSocketInfoUIType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Default` | `ItemSocketInfoUIType` | = 0 |

### SocketInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `string?` |  |
| `icon` | `fileID?` |  |
| `gemMatchesSocket` | `bool` |  |

### SocketItemInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `string?` |  |
| `icon` | `fileID?` |  |
| `quality` | `ItemQuality` |  |
