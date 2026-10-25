# LuaDurationObject

Widget methods (`LuaDurationObjectAPI`) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/luadurationobjectapidocumentation.lua` (FileDataID 7660129)

## Methods

### Assign

```lua
LuaDurationObject:Assign(other: LuaDurationObject)
```

Copies another duration object and assigns it to this one.

`SecretArguments=AllowedWhenUntainted`

### Copy

```lua
LuaDurationObject:Copy() -> copy: LuaDurationObject
```

Returns a copy of this duration object.

`ReturnsNeverSecret`

### EvaluateElapsedDuration

```lua
LuaDurationObject:EvaluateElapsedDuration(curve: LuaCurveObjectBase, modifier: DurationTimeModifier) -> result: LuaCurveEvaluatedResult
```

Calculates the elapsed duration in seconds and evaluates it against a supplied curve.

`SecretArguments=AllowedWhenUntainted` `SecretWhenCurveSecret`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `curve` | `LuaCurveObjectBase` |  |
| `modifier` | `DurationTimeModifier` | default `"RealTime"` |

### EvaluateElapsedPercent

```lua
LuaDurationObject:EvaluateElapsedPercent(curve: LuaCurveObjectBase, modifier: DurationTimeModifier) -> result: LuaCurveEvaluatedResult
```

Calculates the elapsed duration as a percentage value and evaluates it against a supplied curve.

`SecretArguments=AllowedWhenUntainted` `SecretWhenCurveSecret`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `curve` | `LuaCurveObjectBase` |  |
| `modifier` | `DurationTimeModifier` | default `"RealTime"` |

### EvaluateRemainingDuration

```lua
LuaDurationObject:EvaluateRemainingDuration(curve: LuaCurveObjectBase, modifier: DurationTimeModifier) -> result: LuaCurveEvaluatedResult
```

Calculates the remaining duration in seconds and evaluates it against a supplied curve.

`SecretArguments=AllowedWhenUntainted` `SecretWhenCurveSecret`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `curve` | `LuaCurveObjectBase` |  |
| `modifier` | `DurationTimeModifier` | default `"RealTime"` |

### EvaluateRemainingPercent

```lua
LuaDurationObject:EvaluateRemainingPercent(curve: LuaCurveObjectBase, modifier: DurationTimeModifier) -> result: LuaCurveEvaluatedResult
```

Calculates the remaining duration as a percentage value and evaluates it against a supplied curve.

`SecretArguments=AllowedWhenUntainted` `SecretWhenCurveSecret`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `curve` | `LuaCurveObjectBase` |  |
| `modifier` | `DurationTimeModifier` | default `"RealTime"` |

### EvaluateTotalDuration

```lua
LuaDurationObject:EvaluateTotalDuration(curve: LuaCurveObjectBase, modifier: DurationTimeModifier) -> result: LuaCurveEvaluatedResult
```

Calculates the total duration in seconds and evaluates it against a supplied curve.

`SecretArguments=AllowedWhenUntainted` `SecretWhenCurveSecret`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `curve` | `LuaCurveObjectBase` |  |
| `modifier` | `DurationTimeModifier` | default `"RealTime"` |

### FormatElapsedDuration

```lua
LuaDurationObject:FormatElapsedDuration(formatter: NumericFormatter, modifier: DurationTimeModifier) -> formatted: string
```

Formats the elapsed duration of this object to a string.

`SecretArguments=AllowedWhenUntainted` `SecretWhenNumericFormatterSecret`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `formatter` | `NumericFormatter` |  |
| `modifier` | `DurationTimeModifier` | default `"RealTime"` |

### FormatRemainingDuration

```lua
LuaDurationObject:FormatRemainingDuration(formatter: NumericFormatter, modifier: DurationTimeModifier) -> formatted: string
```

Formats the remaining duration of this object to a string.

`SecretArguments=AllowedWhenUntainted` `SecretWhenNumericFormatterSecret`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `formatter` | `NumericFormatter` |  |
| `modifier` | `DurationTimeModifier` | default `"RealTime"` |

### FormatTotalDuration

```lua
LuaDurationObject:FormatTotalDuration(formatter: NumericFormatter, modifier: DurationTimeModifier) -> formatted: string
```

Formats the total duration of this object to a string.

`SecretArguments=AllowedWhenUntainted` `SecretWhenNumericFormatterSecret`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `formatter` | `NumericFormatter` |  |
| `modifier` | `DurationTimeModifier` | default `"RealTime"` |

### GetClock

```lua
LuaDurationObject:GetClock() -> clock: LuaDurationClock?
```

Returns the clock source used by this object.

Returns:

| Name | Type | Notes |
|---|---|---|
| `clock` | `LuaDurationClock?` | If nil, the duration object is using an internal default clock source equivalent to GetTime(). |

### GetClockTime

```lua
LuaDurationObject:GetClockTime() -> clockTime: FrameTime
```

Returns the current time of the clock source used by this object.

### GetElapsedDuration

```lua
LuaDurationObject:GetElapsedDuration(modifier: DurationTimeModifier) -> elapsedDuration: Seconds
```

Calculates the elapsed duration of the stored time span.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `modifier` | `DurationTimeModifier` | default `"RealTime"` |

### GetElapsedPercent

```lua
LuaDurationObject:GetElapsedPercent(modifier: DurationTimeModifier) -> elapsedPercent: number
```

Calculates the elapsed duration as a percentage value.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `modifier` | `DurationTimeModifier` | default `"RealTime"` |

### GetEndTime

```lua
LuaDurationObject:GetEndTime(modifier: DurationTimeModifier) -> endTime: FrameTime
```

Calculates the end time of the stored time span.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `modifier` | `DurationTimeModifier` | default `"RealTime"` |

### GetModRate

```lua
LuaDurationObject:GetModRate() -> modRate: number
```

Returns the divisor used to convert a duration from real time to base time.

### GetRemainingDuration

```lua
LuaDurationObject:GetRemainingDuration(modifier: DurationTimeModifier) -> remainingDuration: Seconds
```

Calculates the remaining duration of the stored time span.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `modifier` | `DurationTimeModifier` | default `"RealTime"` |

### GetRemainingPercent

```lua
LuaDurationObject:GetRemainingPercent(modifier: DurationTimeModifier) -> remainingPercent: number
```

Calculates the remaining duration as a percentage value.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `modifier` | `DurationTimeModifier` | default `"RealTime"` |

### GetStartTime

```lua
LuaDurationObject:GetStartTime(modifier: DurationTimeModifier) -> startTime: FrameTime
```

Calculates the start time of the stored time span.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `modifier` | `DurationTimeModifier` | default `"RealTime"` |

### GetTotalDuration

```lua
LuaDurationObject:GetTotalDuration(modifier: DurationTimeModifier) -> totalDuration: Seconds
```

Calculates the total duration of the stored time span.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `modifier` | `DurationTimeModifier` | default `"RealTime"` |

### HasExpired

```lua
LuaDurationObject:HasExpired(modifier: DurationTimeModifier) -> hasExpired: bool
```

Returns true once the duration has reached its end time.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `modifier` | `DurationTimeModifier` | default `"RealTime"` |

### HasSecretValues

```lua
LuaDurationObject:HasSecretValues() -> hasSecretValues: bool
```

Returns true if the duration has been configured with any secret values.

`ReturnsNeverSecret`

### HasStarted

```lua
LuaDurationObject:HasStarted(modifier: DurationTimeModifier) -> hasStarted: bool
```

Returns true once the duration has reached its start time.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `modifier` | `DurationTimeModifier` | default `"RealTime"` |

### IsActive

```lua
LuaDurationObject:IsActive(modifier: DurationTimeModifier) -> isActive: bool
```

Returns true while the duration is at or after its start time and before its end time.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `modifier` | `DurationTimeModifier` | default `"RealTime"` |

### IsZero

```lua
LuaDurationObject:IsZero() -> isZero: bool
```

Returns true if the duration object is measuring a zero duration time span.

### Reset

```lua
LuaDurationObject:Reset()
```

Resets the duration object to represent a zero duration time span.

### SetClock

```lua
LuaDurationObject:SetClock(clock: LuaDurationClock?)
```

Configures the clock source used by this object.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `clock` | `LuaDurationClock?` | If nil, the duration object will use an internal default clock source equivalent to GetTime(). |

### SetTimeFromEnd

```lua
LuaDurationObject:SetTimeFromEnd(endTime: FrameTime, duration: Seconds, modRate: number)
```

Configures the duration object to represent an end time and a duration.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `endTime` | `FrameTime` |  |
| `duration` | `Seconds` |  |
| `modRate` | `number` | default `1`; Optional divisor for converting this time span to a base time. |

### SetTimeFromStart

```lua
LuaDurationObject:SetTimeFromStart(startTime: FrameTime, duration: Seconds, modRate: number)
```

Configures the duration object to represent a start time and a duration.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `startTime` | `FrameTime` |  |
| `duration` | `Seconds` |  |
| `modRate` | `number` | default `1`; Optional divisor for converting this time span to a base time. |

### SetTimeSpan

```lua
LuaDurationObject:SetTimeSpan(startTime: FrameTime, endTime: FrameTime)
```

Configures the duration object to represent a fixed start and end time span. If the end time is earlier than the start time, the duration will clamp to zero.

`SecretArguments=AllowedWhenUntainted`

### SetToDefaults

```lua
LuaDurationObject:SetToDefaults()
```

Resets all state on the duration, and clears the secret values flag.
