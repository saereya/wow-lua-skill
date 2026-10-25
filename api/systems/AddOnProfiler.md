# AddOnProfiler

Namespace `C_AddOnProfiler` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/addonprofilerdocumentation.lua` (FileDataID 6315781)

## Functions

### AddMeasuredCallEvent

```lua
C_AddOnProfiler.AddMeasuredCallEvent(name: stringView)
```

Adds a measured event to any ongoing measured calls. If no such calls are currently taking place, this function does nothing.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `name` | `stringView` | User-defined string describing the measured event. This should be kept under 48 bytes to avoid memory allocations. |

### AddPerformanceMessageShown

```lua
C_AddOnProfiler.AddPerformanceMessageShown(msg: AddOnPerformanceMessage)
```

Internal API for telemetry.

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### CheckForPerformanceMessage

```lua
C_AddOnProfiler.CheckForPerformanceMessage() -> msg: AddOnPerformanceMessage
```

Optimized check for determining if AddOns are severely impacting UI performance.

`MayReturnNothing`

### GetAddOnMetric

```lua
C_AddOnProfiler.GetAddOnMetric(name: cstring, metric: AddOnProfilerMetric) -> result: number
```

Gets an AddOn profiler value - all times returned are in milliseconds.

`SecretArguments=AllowedWhenUntainted`

### GetApplicationMetric

```lua
C_AddOnProfiler.GetApplicationMetric(metric: AddOnProfilerMetric) -> result: number
```

Overall profiling data for the entire application (not just the UI)

`SecretArguments=AllowedWhenUntainted`

### GetOverallMetric

```lua
C_AddOnProfiler.GetOverallMetric(metric: AddOnProfilerMetric) -> result: number
```

Overall profiling data for all addons

`SecretArguments=AllowedWhenUntainted`

### GetTicksPerSecond

```lua
C_AddOnProfiler.GetTicksPerSecond() -> frequency: BigInteger
```

Returns the number of profiling clock ticks that occur within a single real-time second.

### GetTopKAddOnsForMetric

```lua
C_AddOnProfiler.GetTopKAddOnsForMetric(metric: AddOnProfilerMetric, k: number) -> results: AddOnProfilerResult[]
```

Gets top K AddOns for a given metric.

`SecretArguments=AllowedWhenUntainted`

### IsEnabled

```lua
C_AddOnProfiler.IsEnabled() -> enabled: bool
```

AddOn profiler will be enabled for all users, but this will return false if it ever isn't

### MeasureCall

```lua
C_AddOnProfiler.MeasureCall(func: LuaValueVariant, arguments: LuaValueVariant) -> results: AddOnProfilerCallResults, returns: LuaValueVariant
```

Performs a profiled measurement of a single function call with any supplied arguments.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `func` | `LuaValueVariant` |  |
| `arguments` | `LuaValueVariant` | `NilableContents`; `StrideIndex=1` |

Returns:

| Name | Type | Notes |
|---|---|---|
| `results` | `AddOnProfilerCallResults` |  |
| `returns` | `LuaValueVariant` | `NilableContents`; `StrideIndex=1` |

## Types

### AddOnPerformanceMessage

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `type` | `AddOnPerformanceMessageType` |  |
| `metric` | `AddOnProfilerMetric` |  |
| `addOnName` | `string?` |  |
| `metricValue` | `number` |  |
| `thresholdValue` | `number` |  |

### AddOnProfilerCallEvent

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `string` | User-defined string describing the measured event. |
| `allocatedBytes` | `BigUInteger` | Snapshot of the allocated byte count when this event was recorded. |
| `deallocatedBytes` | `BigUInteger` | Snapshot of the deallocated byte count when this event was recorded. |
| `elapsedMilliseconds` | `number` | Snapshot of the elapsed milliseconds when this event was recorded. |
| `elapsedTicks` | `BigInteger` | Snapshot of the elapsed tick count when this event was recorded. |

### AddOnProfilerCallResults

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `elapsedMilliseconds` | `number` | Total number of milliseconds spent executing the function. |
| `elapsedTicks` | `BigInteger` | Total number of profiling clock ticks spent executing the function. |
| `allocatedBytes` | `BigUInteger` | Total number of bytes allocated during call execution. |
| `deallocatedBytes` | `BigUInteger` | Total number of bytes deallocated during call execution. |
| `events` | `AddOnProfilerCallEvent[]` | Events recorded by any AddMeasuredCallEvent calls that took place during function execution. |

### AddOnProfilerResult

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `addOnName` | `cstring` |  |
| `metricValue` | `number` |  |
