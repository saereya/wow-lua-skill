# UITimer

Namespace `C_Timer` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/uitimerdocumentation.lua` (FileDataID 4637299)

## Functions

### After

```lua
C_Timer.After(seconds: number, callback: TimerCallback)
```

`SecretArguments=AllowedWhenUntainted`

### NewTicker

```lua
C_Timer.NewTicker(seconds: number, callback: TickerCallback, iterations: number?) -> cbObject: TickerCallback
```

`SecretArguments=AllowedWhenUntainted`

### NewTimedSignalMap

```lua
C_Timer.NewTimedSignalMap(callback: TimedSignalMapCallback) -> signalMap: TimedSignalMap
```

Creates a new timed signal map that invokes the supplied callback with each key as it becomes due.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `callback` | `TimedSignalMapCallback` | Callback to execute when each entry becomes due. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `signalMap` | `TimedSignalMap` | The newly created timed signal map. |

### NewTimer

```lua
C_Timer.NewTimer(seconds: number, callback: TickerCallback) -> cbObject: TickerCallback
```

`SecretArguments=AllowedWhenUntainted`

## Types

### TickerCallback

*CallbackType*

Arguments:

| Name | Type | Notes |
|---|---|---|
| `cb` | `TimerCallback` |  |

### TimerCallback

*CallbackType*
