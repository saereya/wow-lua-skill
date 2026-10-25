# SecondsFormatterShared

source `interface/addons/blizzard_apidocumentationgenerated/secondsformattershareddocumentation.lua` (FileDataID 7754023)

## Types

### SecondsFormatterAbbreviation

*Enumeration* · 3 values, 0..2

Access values as `Enum.SecondsFormatterAbbreviation.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `SecondsFormatterAbbreviation` | = 0 |
| `Truncate` | `SecondsFormatterAbbreviation` | = 1 |
| `OneLetter` | `SecondsFormatterAbbreviation` | = 2 |

### SecondsFormatterInterval

*Enumeration* · 4 values, 0..3

Access values as `Enum.SecondsFormatterInterval.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Seconds` | `SecondsFormatterInterval` | = 0 |
| `Minutes` | `SecondsFormatterInterval` | = 1 |
| `Hours` | `SecondsFormatterInterval` | = 2 |
| `Days` | `SecondsFormatterInterval` | = 3 |

### SecondsFormatterIntervalWhitespace

*Enumeration* · 3 values, 0..2

Access values as `Enum.SecondsFormatterIntervalWhitespace.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Preserve` | `SecondsFormatterIntervalWhitespace` | = 0; Do not strip any whitespace from interval unit strings. |
| `Strip` | `SecondsFormatterIntervalWhitespace` | = 1; Strip whitespace from interval unit strings. Some locales override this setting (eg. deDE, ruRU). |
| `StripIgnoreLocale` | `SecondsFormatterIntervalWhitespace` | = 2; Always strip whitespace from interval unit strings even if the client locale should normally preserve whitespace. |

### SecondsFormatterRounding

*Enumeration* · 2 values, 0..1

Access values as `Enum.SecondsFormatterRounding.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `RoundUp` | `SecondsFormatterRounding` | = 0; Round fractional seconds up to the next whole second when not displaying milliseconds. |
| `Truncate` | `SecondsFormatterRounding` | = 1; Truncate fractional seconds to the current whole second when not displaying milliseconds. |
