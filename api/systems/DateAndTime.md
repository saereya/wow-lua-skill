# DateAndTime

Namespace `C_DateAndTime` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/dateandtimedocumentation.lua` (FileDataID 4637098)

## Functions

### AdjustTimeByDays

```lua
C_DateAndTime.AdjustTimeByDays(date: CalendarTime, days: number) -> newDate: CalendarTime
```

`SecretArguments=AllowedWhenUntainted`

### AdjustTimeByMinutes

```lua
C_DateAndTime.AdjustTimeByMinutes(date: CalendarTime, minutes: number) -> newDate: CalendarTime
```

`SecretArguments=AllowedWhenUntainted`

### AdjustTimeByMonths

```lua
C_DateAndTime.AdjustTimeByMonths(date: CalendarTime, months: number) -> newDate: CalendarTime
```

`SecretArguments=AllowedWhenUntainted`

### CompareCalendarTime

```lua
C_DateAndTime.CompareCalendarTime(lhsCalendarTime: CalendarTime, rhsCalendarTime: CalendarTime) -> comparison: number
```

`SecretArguments=AllowedWhenUntainted`

Returns:

| Name | Type | Notes |
|---|---|---|
| `comparison` | `number` | -1 if rhsCalendarTime < lhsCalendarTime, 0 if rhsCalendarTime == lhsCalendarTime, 1 if rhsCalendarTime > lhsCalendarTime |

### GetCalendarTimeFromEpoch

```lua
C_DateAndTime.GetCalendarTimeFromEpoch(epoch: BigUInteger) -> date: CalendarTime
```

`SecretArguments=AllowedWhenUntainted`

### GetCurrentCalendarTime

```lua
C_DateAndTime.GetCurrentCalendarTime() -> date: CalendarTime
```

### GetSecondsUntilDailyReset

```lua
C_DateAndTime.GetSecondsUntilDailyReset() -> seconds: time_t
```

### GetSecondsUntilWeeklyReset

```lua
C_DateAndTime.GetSecondsUntilWeeklyReset() -> seconds: time_t
```

### GetServerTimeLocal

```lua
C_DateAndTime.GetServerTimeLocal() -> serverTimeLocal: time_t
```

### GetWeeklyResetStartTime

```lua
C_DateAndTime.GetWeeklyResetStartTime() -> seconds: time_t
```

### IsDayTime

```lua
C_DateAndTime.IsDayTime() -> isDayTime: bool
```

## Events

### DIEL_CYCLE_CHANGED

```lua
DIEL_CYCLE_CHANGED(isDayTime: bool)
```

Signaled when the game time transitions between day and night.

`SynchronousEvent`

## Types

### TimeEventFlag

*Enumeration* · 3 values, 1..4

Access values as `Enum.TimeEventFlag.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `GlueScreenShortcut` | `TimeEventFlag` | = 1 |
| `WeeklyReset` | `TimeEventFlag` | = 2 |
| `GlobalLaunch` | `TimeEventFlag` | = 4 |
