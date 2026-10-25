# DurationTextBindingObject

Widget methods (`DurationTextBindingObjectAPI`) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/durationtextbindingobjectapidocumentation.lua` (FileDataID 8015795)

## Methods

### Assign

```lua
DurationTextBindingObject:Assign(other: DurationTextBinding)
```

Copies another duration text binding and assigns it to this one.

`SecretArguments=AllowedWhenUntainted`

### CanFormatText

```lua
DurationTextBindingObject:CanFormatText() -> canFormatText: bool
```

Returns true if this binding has enough configuration to produce formatted text.

### CanUpdateFontString

```lua
DurationTextBindingObject:CanUpdateFontString() -> canUpdateText: bool
```

Returns true if this binding has enough configuration to update its font string with formatted text.

### ClearTextColorCurve

```lua
DurationTextBindingObject:ClearTextColorCurve()
```

Clears the text color curve used by this binding.

### Copy

```lua
DurationTextBindingObject:Copy() -> copy: DurationTextBinding
```

Returns a copy of this duration text binding.

`ReturnsNeverSecret`

### Disable

```lua
DurationTextBindingObject:Disable()
```

Disables automatic updates for this duration text binding.

### Enable

```lua
DurationTextBindingObject:Enable()
```

Enables automatic updates for this duration text binding.

### GetDuration

```lua
DurationTextBindingObject:GetDuration() -> duration: LuaDurationObject?
```

Returns the duration object used by this duration text binding.

### GetExpiredText

```lua
DurationTextBindingObject:GetExpiredText() -> text: string?
```

Returns the text shown when the duration has fully expired.

### GetFontString

```lua
DurationTextBindingObject:GetFontString() -> fontString: SimpleFontString?
```

Returns the font string updated by this duration text binding.

### GetFormattedText

```lua
DurationTextBindingObject:GetFormattedText() -> text: string
```

Returns the text that would currently be assigned to the configured font string.

Returns:

| Name | Type | Notes |
|---|---|---|
| `text` | `string` | `ConditionalSecret` |

### GetFormattedTextColor

```lua
DurationTextBindingObject:GetFormattedTextColor() -> color: colorRGBA
```

Returns the text color that would currently be assigned to the configured font string.

`MayReturnNothing`

Returns:

| Name | Type | Notes |
|---|---|---|
| `color` | `colorRGBA` | `Mixin=ColorMixin`; `ConditionalSecret` |

### GetTextColorCurve

```lua
DurationTextBindingObject:GetTextColorCurve() -> curve: LuaColorCurveObject, property: DurationTextBindingProperty
```

Returns the text color curve used by this binding.

`MayReturnNothing`

### GetTimeModifier

```lua
DurationTextBindingObject:GetTimeModifier() -> modifier: DurationTimeModifier
```

Returns the time modifier used when sampling duration values for this binding.

### GetUpdateInterval

```lua
DurationTextBindingObject:GetUpdateInterval() -> updateInterval: number
```

Returns the minimum number of seconds between automatic text updates. A value of zero updates every game tick.

### GetZeroDurationText

```lua
DurationTextBindingObject:GetZeroDurationText() -> text: string?
```

Returns the text shown when the duration is not configured, or represents a zero-duration time span.

### HasSecretValues

```lua
DurationTextBindingObject:HasSecretValues() -> hasSecretValues: bool
```

Returns true if the duration text binding has been configured with any secret values.

`ReturnsNeverSecret`

### IsEnabled

```lua
DurationTextBindingObject:IsEnabled() -> enabled: bool
```

Returns true if this duration text binding updates its font string automatically.

### SetDuration

```lua
DurationTextBindingObject:SetDuration(duration: LuaDurationObject)
```

Configures the duration object used by this duration text binding.

`SecretArguments=AllowedWhenUntainted`

### SetEnabled

```lua
DurationTextBindingObject:SetEnabled(enabled: bool)
```

Configures whether this duration text binding updates its font string automatically.

`SecretArguments=AllowedWhenUntainted`

### SetExpiredText

```lua
DurationTextBindingObject:SetExpiredText(text: string?)
```

Configures the text shown when the duration has fully expired.

`SecretArguments=AllowedWhenUntainted`

### SetFontString

```lua
DurationTextBindingObject:SetFontString(fontString: SimpleFontString)
```

Configures the font string updated by this duration text binding.

`SecretArguments=AllowedWhenUntainted`

### SetFormatter

```lua
DurationTextBindingObject:SetFormatter(formatter: NumericFormatter)
```

Configures the text format used by this duration text binding to display the remaining duration using the supplied formatter.

`SecretArguments=AllowedWhenUntainted`

### SetTextColorCurve

```lua
DurationTextBindingObject:SetTextColorCurve(curve: LuaColorCurveObject, property: DurationTextBindingProperty)
```

Configures this duration text binding to adjust fontstring text color by evaluating a duration property through a curve.

`SecretArguments=AllowedWhenUntainted`

### SetTextFormat

```lua
DurationTextBindingObject:SetTextFormat(formatString: stringView, components: DurationTextBindingFormatComponent[])
```

Configures the text format used by this duration text binding. The format string may contain '{}' placeholders, each of which is substituted by the corresponding component in the supplied array.

`SecretArguments=AllowedWhenUntainted`

### SetTimeModifier

```lua
DurationTextBindingObject:SetTimeModifier(modifier: DurationTimeModifier)
```

Configures the time modifier used when sampling duration values for this binding.

`SecretArguments=AllowedWhenUntainted`

### SetToDefaults

```lua
DurationTextBindingObject:SetToDefaults()
```

Resets this duration text binding to its default state, clearing the configured font string, duration, format, formatter, and fallback text.

### SetUpdateInterval

```lua
DurationTextBindingObject:SetUpdateInterval(updateInterval: number)
```

Configures the minimum number of seconds between automatic text updates. A value of zero updates every game tick.

`SecretArguments=AllowedWhenUntainted`

### SetZeroDurationText

```lua
DurationTextBindingObject:SetZeroDurationText(text: string?)
```

Configures the text shown when the duration is not configured, or represents a zero-duration time span.

`SecretArguments=AllowedWhenUntainted`

### UpdateFontString

```lua
DurationTextBindingObject:UpdateFontString()
```

Immediately updates the configured font string from the current duration state.
