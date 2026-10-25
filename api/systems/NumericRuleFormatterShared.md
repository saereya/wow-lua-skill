# NumericRuleFormatterShared

source `interface/addons/blizzard_apidocumentationgenerated/numericruleformattershareddocumentation.lua` (FileDataID 7754020)

## Types

### NumericRuleFormatRounding

*Enumeration* · 3 values, 0..2

Access values as `Enum.NumericRuleFormatRounding.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Nearest` | `NumericRuleFormatRounding` | = 0 |
| `Up` | `NumericRuleFormatRounding` | = 1 |
| `Down` | `NumericRuleFormatRounding` | = 2 |

### NumericRuleFormatBreakpoint

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `threshold` | `number` | Minimum input value that this rule applies to. |
| `step` | `number?` | If specified, the input value is rounded to multiples of this step before processing. |
| `rounding` | `NumericRuleFormatRounding` | default `"Nearest"`; If specified, the rounding mode to apply to the step. |
| `min` | `number?` | If specified, clamps the input value to this value if lesser after rounding. |
| `max` | `number?` | If specified, clamps the input value to this value if greater after rounding. |
| `format` | `string` | The format string to apply at this threshold. If no components are specified, this can include at-most one numeric format specifier - else, should contain an equal number of format specifiers to elements in the components array. |
| `components` | `NumericRuleFormatComponent[]?` | Vector of component descriptions for this rule. |

### NumericRuleFormatComponent

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `div` | `number?` | If specified, divide the value by this amount and use the resulting quotient. This is applied before modulo division. |
| `mod` | `number?` | If specified, divide the value by this amount and use the resulting remainder. This is applied after quotient division. |
| `step` | `number?` | If specified, round the value to multiples of this step. This is applied after all division. |
| `rounding` | `NumericRuleFormatRounding` | default `"Nearest"`; If specified, rounding mode to apply to the step. |
