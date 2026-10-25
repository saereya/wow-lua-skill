# Cinematic

Global functions · environment All · source `interface/addons/blizzard_apidocumentationgenerated/cinematicdocumentation.lua` (FileDataID 4637047)

## Functions

### CinematicFinished

```lua
CinematicFinished(movieType: CinematicType, userCanceled: bool, didError: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `movieType` | `CinematicType` |  |
| `userCanceled` | `bool` | default `false` |
| `didError` | `bool` | default `false` |

### CinematicStarted

```lua
CinematicStarted(movieType: CinematicType, movieID: number, canCancel: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `movieType` | `CinematicType` |  |
| `movieID` | `number` |  |
| `canCancel` | `bool` | default `true` |

### GetCurrentCinematicSummary

```lua
GetCurrentCinematicSummary() -> summary: cstring
```

### InCinematic

```lua
InCinematic() -> inCinematic: bool
```

### MouseOverrideCinematicDisable

```lua
MouseOverrideCinematicDisable(doOverride: bool)
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `doOverride` | `bool` | default `false` |

### OpeningCinematic

```lua
OpeningCinematic()
```

### StopCinematic

```lua
StopCinematic()
```

## Events

### CINEMATIC_START

```lua
CINEMATIC_START(canBeCancelled: bool, forcedAspectRatio: CameraModeAspectRatio)
```

`SynchronousEvent`

### CINEMATIC_STOP

```lua
CINEMATIC_STOP()
```

`SynchronousEvent`

### HIDE_SUBTITLE

```lua
HIDE_SUBTITLE()
```

`SynchronousEvent`

### PLAY_MOVIE

```lua
PLAY_MOVIE(movieID: number)
```

`SynchronousEvent`

### SHOW_SUBTITLE

```lua
SHOW_SUBTITLE(subtitle: cstring, sender: cstring?)
```

`SynchronousEvent`

### STOP_MOVIE

```lua
STOP_MOVIE()
```

`SynchronousEvent`
