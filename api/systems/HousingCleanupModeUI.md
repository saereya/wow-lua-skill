# HousingCleanupModeUI

Namespace `C_HousingCleanupMode` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/housingcleanupmodeuidocumentation.lua` (FileDataID 7384749)

## Functions

### GetHoveredDecorInfo

```lua
C_HousingCleanupMode.GetHoveredDecorInfo() -> info: HousingDecorInstanceInfo?
```

### IsHoveringDecor

```lua
C_HousingCleanupMode.IsHoveringDecor() -> isHoveringDecor: bool
```

### RemoveSelectedDecor

```lua
C_HousingCleanupMode.RemoveSelectedDecor()
```

## Events

### HOUSING_CLEANUP_MODE_HOVERED_TARGET_CHANGED

```lua
HOUSING_CLEANUP_MODE_HOVERED_TARGET_CHANGED(hasHoveredTarget: bool, targetType: HousingCleanupModeTargetType)
```

`SynchronousEvent`

### HOUSING_CLEANUP_MODE_TARGET_SELECTED

```lua
HOUSING_CLEANUP_MODE_TARGET_SELECTED()
```

`SynchronousEvent`

## Types

### HousingCleanupModeTargetType

*Enumeration* · 3 values, 0..2

Access values as `Enum.HousingCleanupModeTargetType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `HousingCleanupModeTargetType` | = 0 |
| `Decor` | `HousingCleanupModeTargetType` | = 1 |
| `HouseExterior` | `HousingCleanupModeTargetType` | = 2 |
