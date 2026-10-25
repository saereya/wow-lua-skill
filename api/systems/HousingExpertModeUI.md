# HousingExpertModeUI

Namespace `C_HousingExpertMode` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/housingexpertmodeuidocumentation.lua` (FileDataID 7350483)

## Functions

### CancelActiveEditing

```lua
C_HousingExpertMode.CancelActiveEditing()
```

Cancels all in-progress editing of the selected target, which will reset any unsaved changes and deselect the active target; Will not reset any already-applied changes

### CommitDecorMovement

```lua
C_HousingExpertMode.CommitDecorMovement()
```

Attempt to save the changes made to the currently selected decor instance

### CommitHouseExteriorPosition

```lua
C_HousingExpertMode.CommitHouseExteriorPosition()
```

Attempt to save the changes made to the House Exterior's position within the plot

### GetHoveredDecorInfo

```lua
C_HousingExpertMode.GetHoveredDecorInfo() -> info: HousingDecorInstanceInfo?
```

Returns info for the placed decor instance currently being hovered, if there is one

### GetPrecisionSubmode

```lua
C_HousingExpertMode.GetPrecisionSubmode() -> activeSubMode: HousingPrecisionSubmode?
```

Returns the currently active Expert submode, if there is one

### GetPrecisionSubmodeRestriction

```lua
C_HousingExpertMode.GetPrecisionSubmodeRestriction(subMode: HousingPrecisionSubmode) -> restriction: HousingExpertSubmodeRestriction
```

Returns the type of restriction currently active on the submode; Will return HousingExpertSubmodeRestriction:None if submode is not currently restricted

`SecretArguments=AllowedWhenUntainted`

### GetSelectedDecorInfo

```lua
C_HousingExpertMode.GetSelectedDecorInfo() -> info: HousingDecorInstanceInfo?
```

Returns info for the placed decor instance that's currently selected, if there is one

### IsDecorSelected

```lua
C_HousingExpertMode.IsDecorSelected() -> hasSelectedDecor: bool
```

Returns true if a placed decor instance is currently selected

### IsGridVisible

```lua
C_HousingExpertMode.IsGridVisible() -> gridVisible: bool
```

### IsHouseExteriorHovered

```lua
C_HousingExpertMode.IsHouseExteriorHovered() -> isHouseExteriorHovered: bool
```

Returns true if the house's exterior is currently being hovered

### IsHouseExteriorSelected

```lua
C_HousingExpertMode.IsHouseExteriorSelected() -> isHouseExteriorSelected: bool
```

Returns true if the house's exterior is currently selected

### IsHoveringDecor

```lua
C_HousingExpertMode.IsHoveringDecor() -> isHoveringDecor: bool
```

Returns true if a placed decor instance is currently being hovered

### RemoveSelectedDecor

```lua
C_HousingExpertMode.RemoveSelectedDecor()
```

Attempt to return the currently selected decor instance back to the house chest

### ResetPrecisionChanges

```lua
C_HousingExpertMode.ResetPrecisionChanges(activeSubmodeOnly: bool)
```

Reset the selected target's transform back to default values; This is NOT an undo, meaning it will completely reset the transform value to default, NOT just recently-made changes

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `activeSubmodeOnly` | `bool` | If true, only transform values associated with the currently active submode with be reset (ex: in Scale submode, only target's scale will be reset); If false, all transform values will be reset |

### SelectNextRotationAxis

```lua
C_HousingExpertMode.SelectNextRotationAxis()
```

In the rotation submode, swaps the selected axis to the next available one, in order of X -> Y -> Z (wrapping back around to X again, etc); If no axis is selected, selects the first available one, also in that order

### SetGridVisible

```lua
C_HousingExpertMode.SetGridVisible(gridVisible: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetPrecisionIncrementingActive

```lua
C_HousingExpertMode.SetPrecisionIncrementingActive(incrementType: HousingIncrementType, active: bool)
```

Sets a specific type of incremental change active or inactive; Whilever that type is active and target stays selected, incremental changes of that type will continue to be made every frame

`SecretArguments=AllowedWhenUntainted`

### SetPrecisionSubmode

```lua
C_HousingExpertMode.SetPrecisionSubmode(subMode: HousingPrecisionSubmode)
```

Activate a specific Expert submode

`SecretArguments=AllowedWhenUntainted`

## Events

### HOUSING_DECOR_PRECISION_MANIPULATION_EVENT

```lua
HOUSING_DECOR_PRECISION_MANIPULATION_EVENT(event: TransformManipulatorEvent)
```

`SynchronousEvent`

### HOUSING_DECOR_PRECISION_MANIPULATION_STATUS_CHANGED

```lua
HOUSING_DECOR_PRECISION_MANIPULATION_STATUS_CHANGED(isManipulatingSelection: bool)
```

`SynchronousEvent`

### HOUSING_DECOR_PRECISION_SUBMODE_CHANGED

```lua
HOUSING_DECOR_PRECISION_SUBMODE_CHANGED(activeSubmode: HousingPrecisionSubmode?)
```

`SynchronousEvent`

### HOUSING_EXPERT_MODE_HOVERED_TARGET_CHANGED

```lua
HOUSING_EXPERT_MODE_HOVERED_TARGET_CHANGED(hasHoveredTarget: bool, targetType: HousingExpertModeTargetType)
```

`SynchronousEvent`

### HOUSING_EXPERT_MODE_PLACEMENT_FLAGS_UPDATED

```lua
HOUSING_EXPERT_MODE_PLACEMENT_FLAGS_UPDATED(targetType: HousingExpertModeTargetType, activeFlags: HousingDecorPlacementRestriction)
```

`SynchronousEvent`

### HOUSING_EXPERT_MODE_SELECTED_TARGET_CHANGED

```lua
HOUSING_EXPERT_MODE_SELECTED_TARGET_CHANGED(hasSelectedTarget: bool, targetType: HousingExpertModeTargetType)
```

`SynchronousEvent`

## Types

### HousingExpertModeTargetType

*Enumeration* · 3 values, 0..2

Access values as `Enum.HousingExpertModeTargetType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `HousingExpertModeTargetType` | = 0 |
| `Decor` | `HousingExpertModeTargetType` | = 1 |
| `House` | `HousingExpertModeTargetType` | = 2 |

### HousingExpertSubmodeRestriction

*Enumeration* · 4 values, 0..3

Access values as `Enum.HousingExpertSubmodeRestriction.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `HousingExpertSubmodeRestriction` | = 0 |
| `NotInExpertMode` | `HousingExpertSubmodeRestriction` | = 1 |
| `NoHouseExteriorScale` | `HousingExpertSubmodeRestriction` | = 2 |
| `NoWMOScale` | `HousingExpertSubmodeRestriction` | = 3 |

### HousingIncrementType

*Enumeration* · 10 values, 1..512

Access values as `Enum.HousingIncrementType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Left` | `HousingIncrementType` | = 1 |
| `Right` | `HousingIncrementType` | = 2 |
| `Forward` | `HousingIncrementType` | = 4 |
| `Back` | `HousingIncrementType` | = 8 |
| `Up` | `HousingIncrementType` | = 16 |
| `Down` | `HousingIncrementType` | = 32 |
| `RotateLeft` | `HousingIncrementType` | = 64 |
| `RotateRight` | `HousingIncrementType` | = 128 |
| `ScaleUp` | `HousingIncrementType` | = 256 |
| `ScaleDown` | `HousingIncrementType` | = 512 |

### HousingPrecisionSubmode

*Enumeration* · 3 values, 0..2

Access values as `Enum.HousingPrecisionSubmode.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Translate` | `HousingPrecisionSubmode` | = 0 |
| `Rotate` | `HousingPrecisionSubmode` | = 1 |
| `Scale` | `HousingPrecisionSubmode` | = 2 |
