# NumericRuleFormatter

Widget methods (`NumericRuleFormatterAPI`) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/numericruleformatterapidocumentation.lua` (FileDataID 7754024)

## Methods

### AddBreakpoint

```lua
NumericRuleFormatter:AddBreakpoint(breakpoint: NumericRuleFormatBreakpoint)
```

Adds a new breakpoint to the formatter.

`SecretArguments=AllowedWhenUntainted`

### ClearBreakpoints

```lua
NumericRuleFormatter:ClearBreakpoints()
```

Removes all configured breakpoints from the formatter.

### Copy

```lua
NumericRuleFormatter:Copy() -> copy: NumericRuleFormatter
```

Returns a new copy of this formatter.

`ReturnsNeverSecret`

### GetBreakpoints

```lua
NumericRuleFormatter:GetBreakpoints() -> breakpoints: NumericRuleFormatBreakpoint[]
```

Returns a list of all configured breakpoints on this formatter.

### SetBreakpoints

```lua
NumericRuleFormatter:SetBreakpoints(breakpoints: NumericRuleFormatBreakpoint[])
```

Replaces all breakpoints on the formatter.

`SecretArguments=AllowedWhenUntainted`
