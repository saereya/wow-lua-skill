# HousingBasicModeUI

Namespace `C_HousingBasicMode` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/housingbasicmodeuidocumentation.lua` (FileDataID 7350481)

## Functions

### CancelActiveEditing

```lua
C_HousingBasicMode.CancelActiveEditing()
```

Cancels all in-progress editing of the selected target, which will reset any unsaved changes and deselect the active target; Un-placed decor will be returned to the house chest

### CommitDecorMovement

```lua
C_HousingBasicMode.CommitDecorMovement()
```

Attempt to save the changes made to the currently selected decor instance

### CommitHouseExteriorPosition

```lua
C_HousingBasicMode.CommitHouseExteriorPosition()
```

Attempt to save the changes made to the House Exterior's position within the plot

### FinishPlacingNewDecor

```lua
C_HousingBasicMode.FinishPlacingNewDecor()
```

### GetHoveredDecorInfo

```lua
C_HousingBasicMode.GetHoveredDecorInfo() -> info: HousingDecorInstanceInfo?
```

Returns info for the placed decor instance currently being hovered, if there is one

### GetSelectedDecorInfo

```lua
C_HousingBasicMode.GetSelectedDecorInfo() -> info: HousingDecorInstanceInfo?
```

Returns info for the decor instance that's currently selected, if there is one

### IsDecorSelected

```lua
C_HousingBasicMode.IsDecorSelected() -> hasSelectedDecor: bool
```

Returns true if a decor instance is currently selected and being dragged

### IsFreePlaceEnabled

```lua
C_HousingBasicMode.IsFreePlaceEnabled() -> freePlaceEnabled: bool
```

When free place is enabled, collision checks while dragging decor/the house exterior are ignored

### IsGridSnapEnabled

```lua
C_HousingBasicMode.IsGridSnapEnabled() -> isGridSnapEnabled: bool
```

### IsGridVisible

```lua
C_HousingBasicMode.IsGridVisible() -> gridVisible: bool
```

### IsHouseExteriorHovered

```lua
C_HousingBasicMode.IsHouseExteriorHovered() -> isHouseExteriorHovered: bool
```

Returns true if the house's exterior is currently being hovered

### IsHouseExteriorSelected

```lua
C_HousingBasicMode.IsHouseExteriorSelected() -> isHouseExteriorSelected: bool
```

Returns true if the house's exterior is currently selected and being moved

### IsHoveringDecor

```lua
C_HousingBasicMode.IsHoveringDecor() -> isHoveringDecor: bool
```

Returns true if a placed decor instance is currently being hovered

### IsPlacingNewDecor

```lua
C_HousingBasicMode.IsPlacingNewDecor() -> hasPendingDecor: bool
```

### RemoveSelectedDecor

```lua
C_HousingBasicMode.RemoveSelectedDecor()
```

Attempt to return the currently selected decor instance back to the house chest

### RotateDecor

```lua
C_HousingBasicMode.RotateDecor(rotDegrees: number)
```

Rotates the currently selected decor along a single axis; For wall decor, rotates such that the object stays flat against its current wall; For all other decor, rotates around the Z (vertical) axis

`SecretArguments=AllowedWhenUntainted`

### RotateHouseExterior

```lua
C_HousingBasicMode.RotateHouseExterior(rotDegrees: number)
```

Rotates the House Exterior around the Z (vertical) axis

`SecretArguments=AllowedWhenUntainted`

### SetFreePlaceEnabled

```lua
C_HousingBasicMode.SetFreePlaceEnabled(freePlaceEnabled: bool)
```

Set whether free place is enabled; When free place is enabled, collision checks while dragging decor/the house exterior are ignored

`SecretArguments=AllowedWhenUntainted`

### SetGridSnapEnabled

```lua
C_HousingBasicMode.SetGridSnapEnabled(isGridSnapEnabled: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetGridVisible

```lua
C_HousingBasicMode.SetGridVisible(gridVisible: bool)
```

`SecretArguments=AllowedWhenUntainted`

### StartPlacingNewDecor

```lua
C_HousingBasicMode.StartPlacingNewDecor(catalogEntryVariantID: HousingCatalogEntryVariantID)
```

`SecretArguments=AllowedWhenUntainted`

### StartPlacingPreviewDecor

```lua
C_HousingBasicMode.StartPlacingPreviewDecor(decorRecordID: number, bundleCatalogShopProductID: number?)
```

`SecretArguments=AllowedWhenUntainted`

## Events

### HOUSING_BASIC_MODE_HOVERED_TARGET_CHANGED

```lua
HOUSING_BASIC_MODE_HOVERED_TARGET_CHANGED(hasHoveredTarget: bool, targetType: HousingBasicModeTargetType)
```

`SynchronousEvent`

### HOUSING_BASIC_MODE_PLACEMENT_FLAGS_UPDATED

```lua
HOUSING_BASIC_MODE_PLACEMENT_FLAGS_UPDATED(targetType: HousingBasicModeTargetType, activeFlags: HousingDecorPlacementRestriction)
```

`SynchronousEvent`

### HOUSING_BASIC_MODE_SELECTED_TARGET_CHANGED

```lua
HOUSING_BASIC_MODE_SELECTED_TARGET_CHANGED(hasSelectedTarget: bool, targetType: HousingBasicModeTargetType, isPreview: bool)
```

`SynchronousEvent`

### HOUSING_DECOR_FREE_PLACE_STATUS_CHANGED

```lua
HOUSING_DECOR_FREE_PLACE_STATUS_CHANGED(isFreePlaceEnabled: bool)
```

`SynchronousEvent`

### HOUSING_DECOR_GRID_SNAP_OCCURRED

```lua
HOUSING_DECOR_GRID_SNAP_OCCURRED()
```

`SynchronousEvent`

### HOUSING_DECOR_GRID_SNAP_STATUS_CHANGED

```lua
HOUSING_DECOR_GRID_SNAP_STATUS_CHANGED(isGridSnapEnabled: bool)
```

`SynchronousEvent`

## Types

### HousingBasicModeTargetType

*Enumeration* · 3 values, 0..2

Access values as `Enum.HousingBasicModeTargetType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `HousingBasicModeTargetType` | = 0 |
| `Decor` | `HousingBasicModeTargetType` | = 1 |
| `House` | `HousingBasicModeTargetType` | = 2 |
