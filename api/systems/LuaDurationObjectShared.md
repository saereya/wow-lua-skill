# LuaDurationObjectShared

source `interface/addons/blizzard_apidocumentationgenerated/luadurationobjectshareddocumentation.lua` (FileDataID 7660127)

## Types

### DurationTimeModifier

*Enumeration* · 2 values, 0..1

Access values as `Enum.DurationTimeModifier.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `RealTime` | `DurationTimeModifier` | = 0; Use real time for duration calculations. Durations will speed up or slow down based on the applied mod time. |
| `BaseTime` | `DurationTimeModifier` | = 1; Use base time for duration calculations. Durations will be unaffected the applied mod time. |
