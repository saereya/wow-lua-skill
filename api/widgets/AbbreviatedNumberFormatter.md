# AbbreviatedNumberFormatter

Widget methods (`AbbreviatedNumberFormatterAPI`) · environment All · source `interface/addons/blizzard_apidocumentationgenerated/abbreviatednumberformatterapidocumentation.lua` (FileDataID 7754025)

## Methods

### AddBreakpoint

```lua
AbbreviatedNumberFormatter:AddBreakpoint(breakpoint: NumberAbbreviationBreakpoint)
```

Adds a new breakpoint to the formatter.

`SecretArguments=AllowedWhenUntainted` `RequiresValidAbbreviationBreakpoints`

### ClearBreakpoints

```lua
AbbreviatedNumberFormatter:ClearBreakpoints()
```

Removes all configured breakpoints from the formatter.

### Copy

```lua
AbbreviatedNumberFormatter:Copy() -> copy: AbbreviatedNumberFormatter
```

Returns a new copy of this formatter.

`ReturnsNeverSecret`

### GetBreakpoints

```lua
AbbreviatedNumberFormatter:GetBreakpoints() -> breakpoints: NumberAbbreviationBreakpoint[]
```

Returns a list of all configured breakpoints on this formatter.

### ResetBreakpoints

```lua
AbbreviatedNumberFormatter:ResetBreakpoints()
```

Removes all configured breakpoints from the formatter and replaces them with appropriate defaults for the client locale.

### SetBreakpoints

```lua
AbbreviatedNumberFormatter:SetBreakpoints(breakpoints: NumberAbbreviationBreakpoint[])
```

Replaces all breakpoints on the formatter.

`SecretArguments=AllowedWhenUntainted` `RequiresValidAbbreviationBreakpoints`
