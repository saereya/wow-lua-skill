# LuaMathExtensions

Namespace `math` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/luamathextensionsdocumentation.lua` (FileDataID 8293697)

## Functions

### clamp

```lua
math.clamp(value: number, minimum: number, maximum: number) -> clampedValue: number
```

Clamps a value to the inclusive range defined by the minimum and maximum values.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `value` | `number` | The value to clamp. |
| `minimum` | `number` | The inclusive lower bound. |
| `maximum` | `number` | The inclusive upper bound. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `clampedValue` | `number` | The clamped value. |

### isfinite

```lua
math.isfinite(value: number) -> finite: bool
```

Returns whether a value is finite.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `value` | `number` | The value to inspect. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `finite` | `bool` | True if the value is neither infinite nor NaN; otherwise false. |

### isinf

```lua
math.isinf(value: number) -> infinite: bool
```

Returns whether a value is positive or negative infinity.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `value` | `number` | The value to inspect. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `infinite` | `bool` | True if the value is positive or negative infinity; otherwise false. |

### isnan

```lua
math.isnan(value: number) -> nan: bool
```

Returns whether a value is NaN.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `value` | `number` | The value to inspect. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `nan` | `bool` | True if the value is NaN; otherwise false. |

### lerp

```lua
math.lerp(startValue: number, endValue: number, amount: number) -> interpolatedValue: number
```

Linearly interpolates between two values.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `startValue` | `number` | The value returned when the interpolation amount is 0. |
| `endValue` | `number` | The value returned when the interpolation amount is 1. |
| `amount` | `number` | The interpolation amount. Values outside [0, 1] extrapolate beyond the two values. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `interpolatedValue` | `number` | The interpolated value. |

### normalize

```lua
math.normalize(value: number, minimum: number, maximum: number) -> normalizedValue: number
```

Returns the relative position of a value within a range, where the minimum maps to 0 and the maximum maps to 1.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `value` | `number` | The value to normalize. |
| `minimum` | `number` | The value that maps to 0. |
| `maximum` | `number` | The value that maps to 1. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `normalizedValue` | `number` | The normalized value. Values outside the input range produce results outside [0, 1]. |

### remap

```lua
math.remap(value: number, sourceMinimum: number, sourceMaximum: number, destinationMinimum: number, destinationMaximum: number) -> remappedValue: number
```

Maps a value from one range to the corresponding position in another range.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `value` | `number` | The value to map. |
| `sourceMinimum` | `number` | The lower endpoint of the source range. |
| `sourceMaximum` | `number` | The upper endpoint of the source range. |
| `destinationMinimum` | `number` | The lower endpoint of the destination range. |
| `destinationMaximum` | `number` | The upper endpoint of the destination range. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `remappedValue` | `number` | The mapped value. Values outside the source range are extrapolated beyond the destination range. |

### round

```lua
math.round(value: number, decimalPlaces: number) -> roundedValue: number
```

Rounds a value to the specified number of decimal places, with halfway values rounded away from zero.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `value` | `number` | The value to round. |
| `decimalPlaces` | `number` | default `0`; The number of decimal places to preserve. Negative values round to positions left of the decimal point. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `roundedValue` | `number` | The rounded value. |

### saturate

```lua
math.saturate(value: number) -> saturatedValue: number
```

Clamps a value to the inclusive range [0, 1].

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `value` | `number` | The value to clamp. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `saturatedValue` | `number` | The value clamped to the inclusive range [0, 1]. |

### sign

```lua
math.sign(value: number) -> sign: number
```

Returns -1 for negative values, 0 for zero, and 1 for positive values.

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `value` | `number` | The value whose sign will be returned. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `sign` | `number` | The sign of the value. |

### wrap

```lua
math.wrap(value: number, minimum: number, maximum: number) -> wrapped: number
```

Wraps a value into the half-open range [minimum, maximum).

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `value` | `number` | The value to wrap. |
| `minimum` | `number` | The inclusive lower bound of the range. |
| `maximum` | `number` | The exclusive upper bound of the range. |

Returns:

| Name | Type | Notes |
|---|---|---|
| `wrapped` | `number` | The wrapped value, greater than or equal to minimum and less than maximum. If minimum equals maximum, returns minimum. |
