# SystemInfo

Namespace `C_System` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/systemdocumentation.lua` (FileDataID 4637256)

## Functions

### GetFrameStack

```lua
C_System.GetFrameStack() -> objects: ScriptRegion[]
```

## Events

### CAPTUREFRAMES_FAILED

```lua
CAPTUREFRAMES_FAILED()
```

`SynchronousEvent`

### CAPTUREFRAMES_SUCCEEDED

```lua
CAPTUREFRAMES_SUCCEEDED()
```

`SynchronousEvent`

### DISABLE_TAXI_BENCHMARK

```lua
DISABLE_TAXI_BENCHMARK()
```

`SynchronousEvent`

### ENABLE_TAXI_BENCHMARK

```lua
ENABLE_TAXI_BENCHMARK()
```

`SynchronousEvent`

### FIRST_FRAME_RENDERED

```lua
FIRST_FRAME_RENDERED()
```

`UniqueEvent`

### GENERIC_ERROR

```lua
GENERIC_ERROR(errorMessage: cstring)
```

`SynchronousEvent`

### GLOBAL_MOUSE_DOWN

```lua
GLOBAL_MOUSE_DOWN(button: cstring)
```

`SynchronousEvent`

### GLOBAL_MOUSE_UP

```lua
GLOBAL_MOUSE_UP(button: cstring)
```

`SynchronousEvent`

### GLOBAL_REGION_MOUSE_DOWN

```lua
GLOBAL_REGION_MOUSE_DOWN(region: ScriptRegion, button: cstring)
```

`SynchronousEvent`

### GLOBAL_REGION_MOUSE_UP

```lua
GLOBAL_REGION_MOUSE_UP(region: ScriptRegion, button: cstring)
```

`SynchronousEvent`

### INITIAL_HOTFIXES_APPLIED

```lua
INITIAL_HOTFIXES_APPLIED()
```

`SynchronousEvent`

### LOC_RESULT

```lua
LOC_RESULT(result: cstring)
```

`SynchronousEvent`

### LOGOUT_CANCEL

```lua
LOGOUT_CANCEL()
```

`SynchronousEvent`

### PLAYER_CAMPING

```lua
PLAYER_CAMPING()
```

`SynchronousEvent`

### PLAYER_ENTERING_WORLD

```lua
PLAYER_ENTERING_WORLD(isInitialLogin: bool, isReloadingUi: bool)
```

`SynchronousEvent`

### PLAYER_LEAVING_WORLD

```lua
PLAYER_LEAVING_WORLD()
```

`SynchronousEvent`

### PLAYER_LOGIN

```lua
PLAYER_LOGIN()
```

`SynchronousEvent`

### PLAYER_LOGOUT

```lua
PLAYER_LOGOUT()
```

`SynchronousEvent`

### PLAYER_QUITING

```lua
PLAYER_QUITING()
```

`SynchronousEvent`

### SEARCH_DB_LOADED

```lua
SEARCH_DB_LOADED()
```

`SynchronousEvent`

### SHARD_TRANSFER

```lua
SHARD_TRANSFER()
```

`SynchronousEvent`

### SHARD_TRANSFER_CANCELLED

```lua
SHARD_TRANSFER_CANCELLED()
```

`SynchronousEvent`

### SHARD_TRANSFER_IMMINENT

```lua
SHARD_TRANSFER_IMMINENT()
```

`SynchronousEvent`

### STREAMING_ICON

```lua
STREAMING_ICON(streamingStatus: number)
```

`SynchronousEvent`

### SYSMSG

```lua
SYSMSG(string: cstring, r: number, g: number, b: number)
```

`SynchronousEvent`

### TIME_PLAYED_MSG

```lua
TIME_PLAYED_MSG(totalTimePlayed: number, timePlayedThisLevel: number)
```

`SynchronousEvent`

### UI_ERROR_MESSAGE

```lua
UI_ERROR_MESSAGE(errorType: luaIndex, message: string)
```

`UniqueEvent`

### UI_ERROR_POPUP

```lua
UI_ERROR_POPUP(errorType: luaIndex, message: string)
```

`UniqueEvent`

### UI_INFO_MESSAGE

```lua
UI_INFO_MESSAGE(errorType: luaIndex, message: string)
```

`UniqueEvent`

### VARIABLES_LOADED

```lua
VARIABLES_LOADED()
```

`SynchronousEvent`

### WOW_MOUSE_NOT_FOUND

```lua
WOW_MOUSE_NOT_FOUND()
```

`SynchronousEvent`
