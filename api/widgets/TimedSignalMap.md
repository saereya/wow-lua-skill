# TimedSignalMap

Widget methods (`TimedSignalMapAPI`) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/timedsignalmapapidocumentation.lua` (FileDataID 8312417)

An object that manages a collection of integer keys, each scheduled to signal at a specific time.

When a key's time arrives it is removed from the map and passed to the map's callback, letting you track many keyed deadlines through a single callback rather than scheduling each one individually.

## Methods

### CancelAllSignals

```lua
TimedSignalMap:CancelAllSignals()
```

Cancels all scheduled signals.

`RequiresTimedSignalMapAccess`

### CancelSignal

```lua
TimedSignalMap:CancelSignal(key: number)
```

Cancels the scheduled signal for the specified key, if one exists.

`SecretArguments=AllowedWhenUntainted` `RequiresTimedSignalMapAccess`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `key` | `number` | Key to cancel. No effect if the key is not scheduled. |

### GetNextSignal

```lua
TimedSignalMap:GetNextSignal() -> key: number, time: FrameTime
```

Returns the next key due to signal along with its scheduled time.

`RequiresTimedSignalMapAccess`

Returns:

| Name | Type | Notes |
|---|---|---|
| `key` | `number` | The key that has been scheduled. |
| `time` | `FrameTime` | Absolute time, on the same clock as GetTime(), at which the key is scheduled to signal. |

### GetSignalCount

```lua
TimedSignalMap:GetSignalCount() -> count: size
```

Returns the number of keys currently scheduled to signal.

`RequiresTimedSignalMapAccess`

Returns:

| Name | Type | Notes |
|---|---|---|
| `count` | `size` | Count of scheduled keys. |

### GetSignalTime

```lua
TimedSignalMap:GetSignalTime(key: number) -> time: FrameTime?
```

Returns the absolute time at which the specified key is scheduled to signal.

`SecretArguments=AllowedWhenUntainted` `RequiresTimedSignalMapAccess` `ConstSecretAccessor`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `key` | `number` | Key to query. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `time` | `FrameTime?` | Absolute time the key will signal; nil if not scheduled. |

### HasSignal

```lua
TimedSignalMap:HasSignal(key: number) -> hasSignal: bool
```

Returns whether the specified key is currently scheduled to signal.

`SecretArguments=AllowedWhenUntainted` `RequiresTimedSignalMapAccess` `ConstSecretAccessor`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `key` | `number` | Key to test. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `hasSignal` | `bool` | True if the key is scheduled to signal. |

### SignalAfter

```lua
TimedSignalMap:SignalAfter(key: number, secondsFromNow: Seconds)
```

Schedules the specified key to signal after a delay from the current time, replacing any existing schedule for that key.

`SecretArguments=AllowedWhenUntainted` `RequiresTimedSignalMapAccess`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `key` | `number` | Key to signal. Re-scheduling an existing key replaces its time. |
| `secondsFromNow` | `Seconds` | Delay in seconds from now, converted to an absolute time when scheduled. |

### SignalAt

```lua
TimedSignalMap:SignalAt(key: number, time: FrameTime)
```

Schedules the specified key to signal at an absolute time, replacing any existing schedule for that key.

`SecretArguments=AllowedWhenUntainted` `RequiresTimedSignalMapAccess`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `key` | `number` | Key to signal. Re-scheduling an existing key replaces its time. |
| `time` | `FrameTime` | Absolute time at which to signal, on the same clock as GetTime(). |
