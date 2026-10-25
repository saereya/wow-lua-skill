# SecondsFormatter

Widget methods (`SecondsFormatterAPI`) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/secondsformatterapidocumentation.lua` (FileDataID 7754022)

## Methods

### CanApproximate

```lua
SecondsFormatter:CanApproximate(seconds: Seconds) -> canApproximate: bool
```

Returns true if the given number of seconds is within an appropriate range for approximated formatting.

`SecretArguments=AllowedWhenUntainted` `ConstSecretAccessor`

### CanRoundUpIntervals

```lua
SecondsFormatter:CanRoundUpIntervals() -> canRound: bool
```

Returns true if the formatter can promote values to higher interval bands.

### CanRoundUpLastUnit

```lua
SecondsFormatter:CanRoundUpLastUnit() -> canRound: bool
```

Returns true if the formatter should round the final unit up rather than down.

### EvaluateDesiredUnitCount

```lua
SecondsFormatter:EvaluateDesiredUnitCount(seconds: Seconds) -> count: number
```

Returns the unit count that a given number of seconds will use for formatting.

`SecretArguments=AllowedWhenUntainted` `ConstSecretAccessor`

### EvaluateMaxInterval

```lua
SecondsFormatter:EvaluateMaxInterval(seconds: Seconds) -> interval: SecondsFormatterInterval
```

Returns the maximum interval band that a given number of seconds will use for formatting.

`SecretArguments=AllowedWhenUntainted` `ConstSecretAccessor`

### EvaluateMinInterval

```lua
SecondsFormatter:EvaluateMinInterval(seconds: Seconds) -> interval: SecondsFormatterInterval
```

Returns the minimum interval band that a given number of seconds will use for formatting.

`SecretArguments=AllowedWhenUntainted` `ConstSecretAccessor`

### Format

```lua
SecondsFormatter:Format(seconds: Seconds, abbreviation: SecondsFormatterAbbreviation?) -> formattedSeconds: string
```

Formats a number of seconds and returns the resulting string.

`SecretArguments=AllowedWhenUntainted` `ConstSecretAccessor`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `seconds` | `Seconds` |  |
| `abbreviation` | `SecondsFormatterAbbreviation?` | Optional abbreviation mode to use in-place of the default. |

### FormatZero

```lua
SecondsFormatter:FormatZero(abbreviation: SecondsFormatterAbbreviation?) -> formattedSeconds: string
```

Returns formatted string representing a zero second duration.

`SecretArguments=AllowedWhenUntainted` `ConstSecretAccessor`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `abbreviation` | `SecondsFormatterAbbreviation?` | Optional abbreviation mode to use in-place of the default. |

### GetApproximationSeconds

```lua
SecondsFormatter:GetApproximationSeconds() -> approximationSeconds: Seconds
```

Returns the threshold below which numeric values are formatted as approximated strings.

### GetConvertToLower

```lua
SecondsFormatter:GetConvertToLower() -> convert: bool
```

Returns true if the formatter should lowercase all unit format strings.

### GetDefaultAbbreviation

```lua
SecondsFormatter:GetDefaultAbbreviation() -> abbreviation: SecondsFormatterAbbreviation?
```

Returns the default abbreviation mode used for formatting.

### GetDesiredUnitCount

```lua
SecondsFormatter:GetDesiredUnitCount() -> count: number?
```

Returns the desired unit count for formatting.

Returns:

| Name | Type | Notes |
|---|---|---|
| `count` | `number?` | Nil if configured to use a curve. |

### GetDesiredUnitCountCurve

```lua
SecondsFormatter:GetDesiredUnitCountCurve() -> curve: LuaCurveObject?
```

Returns the desired unit count curve for formatting.

Returns:

| Name | Type | Notes |
|---|---|---|
| `curve` | `LuaCurveObject?` | Nil if configured to static unit count. |

### GetMaxInterval

```lua
SecondsFormatter:GetMaxInterval() -> interval: SecondsFormatterInterval?
```

Returns the maximum interval band permitted for formatting.

Returns:

| Name | Type | Notes |
|---|---|---|
| `interval` | `SecondsFormatterInterval?` | Nil if configured to use a curve. |

### GetMaxIntervalCurve

```lua
SecondsFormatter:GetMaxIntervalCurve() -> curve: LuaCurveObject?
```

Returns the maximum interval band curve permitted for formatting.

Returns:

| Name | Type | Notes |
|---|---|---|
| `curve` | `LuaCurveObject?` | Nil if configured to static interval band. |

### GetMillisecondsThreshold

```lua
SecondsFormatter:GetMillisecondsThreshold() -> threshold: Seconds
```

Returns the threshold below which a value will be formatted as a decimal number of seconds with one place for milliseconds (eg. '3.4')

### GetMinInterval

```lua
SecondsFormatter:GetMinInterval() -> interval: SecondsFormatterInterval?
```

Returns the minimum interval band permitted for formatting.

Returns:

| Name | Type | Notes |
|---|---|---|
| `interval` | `SecondsFormatterInterval?` | Nil if configured to use a curve. |

### GetMinIntervalCurve

```lua
SecondsFormatter:GetMinIntervalCurve() -> curve: LuaCurveObject?
```

Returns the minimum interval band curve permitted for formatting.

Returns:

| Name | Type | Notes |
|---|---|---|
| `curve` | `LuaCurveObject?` | Nil if configured to static interval band. |

### GetRounding

```lua
SecondsFormatter:GetRounding() -> rounding: SecondsFormatterRounding
```

Returns how fractional seconds are rounded when not displaying milliseconds.

Returns:

| Name | Type | Notes |
|---|---|---|
| `rounding` | `SecondsFormatterRounding` | The configured rounding mode. |

### GetStripIntervalWhitespace

```lua
SecondsFormatter:GetStripIntervalWhitespace() -> strip: SecondsFormatterIntervalWhitespace
```

Returns the whitespace stripping mode of the formatter.

### Reset

```lua
SecondsFormatter:Reset()
```

Resets all stored configuration of the formatter.

### SetApproximationSeconds

```lua
SecondsFormatter:SetApproximationSeconds(seconds: Seconds)
```

Configures the formatter to render numeric values between zero and this value as approximated strings (eg. '< 1m').

`SecretArguments=AllowedWhenUntainted`

### SetCanRoundUpIntervals

```lua
SecondsFormatter:SetCanRoundUpIntervals(canRound: bool)
```

Configures the formatter to promote intervals if values are large enough (eg. '60m' -> '1h').

`SecretArguments=AllowedWhenUntainted`

### SetCanRoundUpLastUnit

```lua
SecondsFormatter:SetCanRoundUpLastUnit(canRound: bool)
```

Configures the formatter to round the last formatted unit up, rather than down.

`SecretArguments=AllowedWhenUntainted`

### SetConvertToLower

```lua
SecondsFormatter:SetConvertToLower(convert: bool)
```

Configures the formatter to convert all interval format strings to lowercase.

`SecretArguments=AllowedWhenUntainted`

### SetDefaultAbbreviation

```lua
SecondsFormatter:SetDefaultAbbreviation(abbreviation: SecondsFormatterAbbreviation)
```

Sets the default abbreviation mode used for formatting.

`SecretArguments=AllowedWhenUntainted`

### SetDesiredUnitCount

```lua
SecondsFormatter:SetDesiredUnitCount(count: number)
```

Sets the desired unit count used for formatting.

`SecretArguments=AllowedWhenUntainted`

### SetDesiredUnitCountCurve

```lua
SecondsFormatter:SetDesiredUnitCountCurve(curve: LuaCurveObject)
```

Sets the desired unit count used for formatting to a curve that will be evaluated with seconds values to produce a desired unit count.

`SecretArguments=AllowedWhenUntainted`

### SetMaxInterval

```lua
SecondsFormatter:SetMaxInterval(interval: SecondsFormatterInterval)
```

Sets the maximum interval band used for formatting.

`SecretArguments=AllowedWhenUntainted`

### SetMaxIntervalCurve

```lua
SecondsFormatter:SetMaxIntervalCurve(curve: LuaCurveObject)
```

Sets the maximum interval band used for formatting to a curve that will be evaluated with seconds values to produce a value matching a SecondsFormatterInterval enum member.

`SecretArguments=AllowedWhenUntainted`

### SetMillisecondsThreshold

```lua
SecondsFormatter:SetMillisecondsThreshold(threshold: Seconds)
```

Sets the threshold below which a value will be formatted as a decimal number of seconds with one place for milliseconds (eg. '3.4')

`SecretArguments=AllowedWhenUntainted`

### SetMinInterval

```lua
SecondsFormatter:SetMinInterval(interval: SecondsFormatterInterval)
```

Sets the minimum interval band used for formatting.

`SecretArguments=AllowedWhenUntainted`

### SetMinIntervalCurve

```lua
SecondsFormatter:SetMinIntervalCurve(curve: LuaCurveObject)
```

Sets the minimum interval band used for formatting to a curve that will be evaluated with seconds values to produce a value matching a SecondsFormatterInterval enum member.

`SecretArguments=AllowedWhenUntainted`

### SetRounding

```lua
SecondsFormatter:SetRounding(rounding: SecondsFormatterRounding)
```

Sets how fractional seconds are rounded when not displaying milliseconds.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `rounding` | `SecondsFormatterRounding` | The rounding mode to use. |

### SetStripIntervalWhitespace

```lua
SecondsFormatter:SetStripIntervalWhitespace(strip: SecondsFormatterIntervalWhitespace)
```

Sets the whitespace stripping mode for the formatter.

`SecretArguments=AllowedWhenUntainted`
