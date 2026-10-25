# DurationTextBindingShared

source `interface/addons/blizzard_apidocumentationgenerated/durationtextbindingshareddocumentation.lua` (FileDataID 8015794)

## Types

### DurationTextBindingProperty

*Enumeration* · 7 values, 0..6

Access values as `Enum.DurationTextBindingProperty.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `RemainingDuration` | `DurationTextBindingProperty` | = 0 |
| `RemainingPercent` | `DurationTextBindingProperty` | = 1 |
| `ElapsedDuration` | `DurationTextBindingProperty` | = 2 |
| `ElapsedPercent` | `DurationTextBindingProperty` | = 3 |
| `TotalDuration` | `DurationTextBindingProperty` | = 4 |
| `StartTime` | `DurationTextBindingProperty` | = 5 |
| `EndTime` | `DurationTextBindingProperty` | = 6 |

### DurationTextBindingColorOptions

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `curve` | `LuaColorCurveObject` |  |
| `property` | `DurationTextBindingProperty` |  |

### DurationTextBindingFormatComponent

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `property` | `DurationTextBindingProperty` | The duration property sampled for this format component. |
| `formatter` | `NumericFormatter` | The numeric formatter used to convert the sampled duration property into text. |

### DurationTextBindingFormatOptions

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `formatString` | `stringView` |  |
| `components` | `DurationTextBindingFormatComponent[]` |  |
