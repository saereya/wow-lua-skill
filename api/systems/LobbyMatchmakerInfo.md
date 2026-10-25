# LobbyMatchmakerInfo

Namespace `C_LobbyMatchmakerInfo` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/lobbymatchmakerinfodocumentation.lua` (FileDataID 6321045)

## Functions

### AbandonQueue

```lua
C_LobbyMatchmakerInfo.AbandonQueue()
```

### EnterQueue

```lua
C_LobbyMatchmakerInfo.EnterQueue(playlistEntry: PartyPlaylistEntry)
```

`SecretArguments=AllowedWhenUntainted`

### GetCurrQueuePlaylistEntry

```lua
C_LobbyMatchmakerInfo.GetCurrQueuePlaylistEntry() -> playlistEntry: PartyPlaylistEntry
```

### GetCurrQueueState

```lua
C_LobbyMatchmakerInfo.GetCurrQueueState() -> queueState: PlunderstormQueueState
```

### GetQueueFromMainlineEnabled

```lua
C_LobbyMatchmakerInfo.GetQueueFromMainlineEnabled() -> queueFromMainlineEnabled: bool
```

### GetQueueStartTime

```lua
C_LobbyMatchmakerInfo.GetQueueStartTime() -> queueStartTime: number
```

### IsInQueue

```lua
C_LobbyMatchmakerInfo.IsInQueue() -> isInQueue: bool
```

### RespondToQueuePop

```lua
C_LobbyMatchmakerInfo.RespondToQueuePop(acceptQueue: bool)
```

`SecretArguments=AllowedWhenUntainted`

## Events

### LOBBY_MATCHMAKER_QUEUE_ABANDONED

```lua
LOBBY_MATCHMAKER_QUEUE_ABANDONED()
```

`SynchronousEvent`

### LOBBY_MATCHMAKER_QUEUE_ERROR

```lua
LOBBY_MATCHMAKER_QUEUE_ERROR()
```

`SynchronousEvent`

### LOBBY_MATCHMAKER_QUEUE_EXPIRED

```lua
LOBBY_MATCHMAKER_QUEUE_EXPIRED()
```

`SynchronousEvent`

### LOBBY_MATCHMAKER_QUEUE_POPPED

```lua
LOBBY_MATCHMAKER_QUEUE_POPPED()
```

`SynchronousEvent`

### LOBBY_MATCHMAKER_QUEUE_STATUS_UPDATE

```lua
LOBBY_MATCHMAKER_QUEUE_STATUS_UPDATE()
```

`SynchronousEvent`

## Types

### PlunderstormQueueState

*Enumeration* · 4 values, 0..3

Access values as `Enum.PlunderstormQueueState.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `PlunderstormQueueState` | = 0 |
| `Queued` | `PlunderstormQueueState` | = 1 |
| `Proposed` | `PlunderstormQueueState` | = 2 |
| `Suspended` | `PlunderstormQueueState` | = 3 |

### LobbyMatchmakerQueueInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `isQueueActive` | `bool` | default `false` |
| `playlistEntryID` | `PartyPlaylistEntry` |  |
| `queueState` | `PlunderstormQueueState` |  |
| `queueStartTime` | `number` |  |
