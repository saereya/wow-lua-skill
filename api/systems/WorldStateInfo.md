# WorldStateInfo

Namespace `C_WorldStateInfo` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/worldstateinfodocumentation.lua` (FileDataID 4637302)

## Events

### CANCEL_PLAYER_COUNTDOWN

```lua
CANCEL_PLAYER_COUNTDOWN(initiatedBy: WOWGUID, informChat: bool, initiatedByName: string?)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

### START_PLAYER_COUNTDOWN

```lua
START_PLAYER_COUNTDOWN(initiatedBy: WOWGUID, timeRemaining: time_t, totalTime: time_t, informChat: bool, initiatedByName: string?)
```

`SecretInChatMessagingLockdown` `SynchronousEvent`

### START_TIMER

```lua
START_TIMER(timerType: StartTimerType, timeRemaining: time_t, totalTime: time_t)
```

`SynchronousEvent`

### STOP_TIMER_OF_TYPE

```lua
STOP_TIMER_OF_TYPE(timerType: StartTimerType)
```

`SynchronousEvent`

### WORLD_STATE_TIMER_START

```lua
WORLD_STATE_TIMER_START(timerID: number)
```

`SynchronousEvent`

### WORLD_STATE_TIMER_STOP

```lua
WORLD_STATE_TIMER_STOP(timerID: number)
```

`SynchronousEvent`
