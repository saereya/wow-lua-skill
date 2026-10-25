# GamepadTargetingManager

Namespace `C_GamepadTargeting` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/gamepadtargetingdocumentation.lua` (FileDataID 6914158)

## Functions

### Disable

```lua
C_GamepadTargeting.Disable() -> targetAlreadySelected: bool
```

### Enable

```lua
C_GamepadTargeting.Enable()
```

### SetFilter

```lua
C_GamepadTargeting.SetFilter(filter: GamepadTargetingFilters)
```

`SecretArguments=AllowedWhenUntainted`

## Types

### GamepadTargetingFilters

*Enumeration* · 3 values, 0..2

Access values as `Enum.GamepadTargetingFilters.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Hostile` | `GamepadTargetingFilters` | = 0 |
| `Friendly` | `GamepadTargetingFilters` | = 1 |
| `All` | `GamepadTargetingFilters` | = 2 |
