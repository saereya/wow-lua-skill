# DurationUtil

Namespace `C_DurationUtil` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/durationutildocumentation.lua` (FileDataID 7660128)

## Functions

### CreateDuration

```lua
C_DurationUtil.CreateDuration() -> duration: LuaDurationObject
```

Creates a zero duration container that can represent a time span.

### CreateDurationTextBinding

```lua
C_DurationUtil.CreateDurationTextBinding() -> binding: DurationTextBinding
```

Creates a duration text binding, which automatically updates a font string with formatted text derived from a duration object.

### CreateManualClock

```lua
C_DurationUtil.CreateManualClock() -> clock: LuaDurationManualClock
```

Creates a manually driven time source for use with duration objects.
