# PerformanceScript

Global functions · environment All · source `interface/addons/blizzard_apidocumentationgenerated/performancedocumentation.lua` (FileDataID 5555480)

## Functions

### GetAddOnCPUUsage

```lua
GetAddOnCPUUsage(name: uiAddon) -> result: number
```

`SecretArguments=AllowedWhenUntainted`

### GetAddOnMemoryUsage

```lua
GetAddOnMemoryUsage(name: uiAddon) -> result: number
```

`SecretArguments=AllowedWhenUntainted`

### GetEventCPUUsage

```lua
GetEventCPUUsage() -> call_time: number, call_count: number
```

### GetFrameCPUUsage

```lua
GetFrameCPUUsage(frame: SimpleFrame, includeChildren: bool) -> call_time: number, call_count: number
```

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `frame` | `SimpleFrame` |  |
| `includeChildren` | `bool` | default `false` |

### GetFunctionCPUUsage

```lua
GetFunctionCPUUsage() -> call_time: number, call_count: number
```

### GetScriptCPUUsage

```lua
GetScriptCPUUsage() -> result: number
```

### ResetCPUUsage

```lua
ResetCPUUsage()
```

### UpdateAddOnCPUUsage

```lua
UpdateAddOnCPUUsage()
```

### UpdateAddOnMemoryUsage

```lua
UpdateAddOnMemoryUsage()
```
