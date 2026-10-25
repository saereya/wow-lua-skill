# QuestSession

Namespace `C_QuestSession` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/questsessiondocumentation.lua` (FileDataID 4637176)

## Functions

### CanStart

```lua
C_QuestSession.CanStart() -> allowed: bool
```

### CanStop

```lua
C_QuestSession.CanStop() -> allowed: bool
```

### Exists

```lua
C_QuestSession.Exists() -> exists: bool
```

### GetAvailableSessionCommand

```lua
C_QuestSession.GetAvailableSessionCommand() -> command: QuestSessionCommand
```

### GetPendingCommand

```lua
C_QuestSession.GetPendingCommand() -> command: QuestSessionCommand
```

### GetProposedMaxLevelForSession

```lua
C_QuestSession.GetProposedMaxLevelForSession() -> proposedMaxLevel: number
```

### GetSessionBeginDetails

```lua
C_QuestSession.GetSessionBeginDetails() -> details: QuestSessionPlayerDetails?
```

### GetSuperTrackedQuest

```lua
C_QuestSession.GetSuperTrackedQuest() -> questID: number?
```

### HasJoined

```lua
C_QuestSession.HasJoined() -> hasJoined: bool
```

### HasPendingCommand

```lua
C_QuestSession.HasPendingCommand() -> hasPendingCommand: bool
```

### RequestSessionStart

```lua
C_QuestSession.RequestSessionStart()
```

### RequestSessionStop

```lua
C_QuestSession.RequestSessionStop()
```

### SendSessionBeginResponse

```lua
C_QuestSession.SendSessionBeginResponse(beginSession: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetQuestIsSuperTracked

```lua
C_QuestSession.SetQuestIsSuperTracked(questID: number, superTrack: bool)
```

`SecretArguments=AllowedWhenUntainted`

## Events

### QUEST_SESSION_CREATED

```lua
QUEST_SESSION_CREATED()
```

`UniqueEvent`

### QUEST_SESSION_DESTROYED

```lua
QUEST_SESSION_DESTROYED()
```

`UniqueEvent`

### QUEST_SESSION_ENABLED_STATE_CHANGED

```lua
QUEST_SESSION_ENABLED_STATE_CHANGED(enabled: bool)
```

`SynchronousEvent`

### QUEST_SESSION_JOINED

```lua
QUEST_SESSION_JOINED()
```

`UniqueEvent`

### QUEST_SESSION_LEFT

```lua
QUEST_SESSION_LEFT()
```

`UniqueEvent`

### QUEST_SESSION_MEMBER_CONFIRM

```lua
QUEST_SESSION_MEMBER_CONFIRM()
```

`SynchronousEvent`

### QUEST_SESSION_MEMBER_START_RESPONSE

```lua
QUEST_SESSION_MEMBER_START_RESPONSE(guid: WOWGUID, response: bool)
```

`SynchronousEvent`

### QUEST_SESSION_NOTIFICATION

```lua
QUEST_SESSION_NOTIFICATION(result: QuestSessionResult, guid: WOWGUID)
```

`SynchronousEvent`

## Types

### QuestSessionPlayerDetails

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `string` |  |
| `guid` | `WOWGUID` |  |
