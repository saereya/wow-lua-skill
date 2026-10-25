# HousingDecorUI

Namespace `C_HousingDecor` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/housingdecoruidocumentation.lua` (FileDataID 5457904)

## Functions

### AnyDecorPlacedInRoom

```lua
C_HousingDecor.AnyDecorPlacedInRoom(roomGUID: WOWGUID) -> isPlaced: bool
```

Returns true if any decor objects are placed in a given room

`SecretArguments=AllowedWhenUntainted`

### CancelActiveEditing

```lua
C_HousingDecor.CancelActiveEditing()
```

Cancels all in-progress editing of the selected target, which will reset any unsaved changes and deselect the active target

### CommitDecorMovement

```lua
C_HousingDecor.CommitDecorMovement()
```

Attempt to save the changes made to the currently selected decor instance

### EnterPreviewState

```lua
C_HousingDecor.EnterPreviewState()
```

### ExitPreviewState

```lua
C_HousingDecor.ExitPreviewState()
```

### GetAllMaxPlacementBudgets

```lua
C_HousingDecor.GetAllMaxPlacementBudgets() -> interiorMaxBudgets: table<HousingBudgetType, number>?, exteriorMaxBudgets: table<HousingBudgetType, number>?
```

Returns the interior and exterior max decor placement budgets for the current owned house interior or plot; Can be increased via house level

Returns:

| Name | Type | Notes |
|---|---|---|
| `interiorMaxBudgets` | `table<HousingBudgetType, number>?` | Map of budget type to max budget amount; Will be nil if not in an owned House or Plot |
| `exteriorMaxBudgets` | `table<HousingBudgetType, number>?` | Map of budget type to max budget amount; Will be nil if not in an owned House or Plot |

### GetAllPlacedDecor

```lua
C_HousingDecor.GetAllPlacedDecor() -> placedDecor: HousingDecorInstanceListEntry[]
```

Placed Decor List APIs currently restricted due to being potentially very expensive operations, may be reworked & opened up in the future

`HasRestrictions`

### GetAllSpentPlacementBudgets

```lua
C_HousingDecor.GetAllSpentPlacementBudgets() -> interiorSpentBudgets: table<HousingBudgetType, number>?, exteriorSpentBudgets: table<HousingBudgetType, number>?
```

Returns how much of the interior and exterior placement budgets for the current owned house interior or plot's decor budget have been spent

Returns:

| Name | Type | Notes |
|---|---|---|
| `interiorSpentBudgets` | `table<HousingBudgetType, number>?` | Map of budget type to spent budget amount; Will be nil if not in an owned House or Plot |
| `exteriorSpentBudgets` | `table<HousingBudgetType, number>?` | Map of budget type to spent budget amount; Will be nil if not in an owned House or Plot |

### GetDecorAssignedPetName

```lua
C_HousingDecor.GetDecorAssignedPetName(decorGUID: WOWGUID) -> name: string?
```

Returns pet name for the placed decor instance associated with the passed Decor GUID, if there is one

`SecretArguments=AllowedWhenUntainted`

### GetDecorCanAttachPet

```lua
C_HousingDecor.GetDecorCanAttachPet(decorID: number) -> canAttachPet: bool
```

`SecretArguments=AllowedWhenUntainted`

### GetDecorHyperlink

```lua
C_HousingDecor.GetDecorHyperlink(decorID: number) -> hyperLink: string
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetDecorIcon

```lua
C_HousingDecor.GetDecorIcon(decorID: number) -> icon: fileID
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetDecorInstanceInfoForGUID

```lua
C_HousingDecor.GetDecorInstanceInfoForGUID(decorGUID: WOWGUID) -> info: HousingDecorInstanceInfo?
```

Returns info for the placed decor instance associated with the passed Decor GUID, if there is one

`SecretArguments=AllowedWhenUntainted`

### GetDecorName

```lua
C_HousingDecor.GetDecorName(decorID: number) -> name: string
```

`SecretArguments=AllowedWhenUntainted` `MayReturnNothing`

### GetHoveredDecorInfo

```lua
C_HousingDecor.GetHoveredDecorInfo() -> info: HousingDecorInstanceInfo?
```

Returns info for the placed decor instance currently being hovered, if there is one

### GetMaxPetPlacementBudget

```lua
C_HousingDecor.GetMaxPetPlacementBudget() -> maxBudget: number?
```

Returns the max pet decor placement budget for the current owned house interior or plot

Returns:

| Name | Type | Notes |
|---|---|---|
| `maxBudget` | `number?` | Will be nil if not in an owned House or Plot |

### GetMaxPlacementBudget

```lua
C_HousingDecor.GetMaxPlacementBudget() -> maxBudget: number?
```

Returns the max decor placement budget for the current owned house interior or plot; Can be increased via house level

Returns:

| Name | Type | Notes |
|---|---|---|
| `maxBudget` | `number?` | Will be nil if not in an owned House or Plot |

### GetNumDecorPlaced

```lua
C_HousingDecor.GetNumDecorPlaced() -> numPlaced: number
```

Returns the number of individual decor objects placed in the current house or plot; This is NOT the value used in placement budget calculations, see GetSpentPlacementBudget for that

### GetNumPreviewDecor

```lua
C_HousingDecor.GetNumPreviewDecor() -> numDecor: number
```

### GetSelectedDecorInfo

```lua
C_HousingDecor.GetSelectedDecorInfo() -> info: HousingDecorInstanceInfo?
```

Returns info for the placed decor instance that's currently selected, if there is one

### GetSpentPetPlacementBudget

```lua
C_HousingDecor.GetSpentPetPlacementBudget() -> totalCost: number?
```

Returns how much of the current owned house interior or plot's pet decor placement budget has been spent

Returns:

| Name | Type | Notes |
|---|---|---|
| `totalCost` | `number?` | Will be nil if not in an owned House or Plot |

### GetSpentPlacementBudget

```lua
C_HousingDecor.GetSpentPlacementBudget() -> totalCost: number?
```

Returns how much of the current owned house interior or plot's decor placement budget has been spent; Different kinds of decor take up different budget amounts, so this value isn't an individual decor count, see GetNumDecorPlaced for that

Returns:

| Name | Type | Notes |
|---|---|---|
| `totalCost` | `number?` | Will be nil if not in an owned House or Plot |

### HasMaxPlacementBudget

```lua
C_HousingDecor.HasMaxPlacementBudget() -> hasMaxBudget: bool
```

Returns whether there's a max decor placement budget available and active for the current player, in the current house interior or plot

### IsDecorSelected

```lua
C_HousingDecor.IsDecorSelected() -> hasSelectedDecor: bool
```

Returns true if a placed decor instance is currently selected

### IsGridVisible

```lua
C_HousingDecor.IsGridVisible() -> gridVisible: bool
```

### IsHouseExteriorDoorHovered

```lua
C_HousingDecor.IsHouseExteriorDoorHovered() -> isHouseExteriorDoorHovered: bool
```

Returns true if the entry door of the house's exterior is currently being hovered

### IsHouseExteriorHovered

```lua
C_HousingDecor.IsHouseExteriorHovered() -> isHouseExteriorHovered: bool
```

Returns true if the house's exterior is currently being hovered

### IsHoveringDecor

```lua
C_HousingDecor.IsHoveringDecor() -> isHoveringDecor: bool
```

Returns true if a placed decor instance is currently being hovered

### IsModeDisabledForPreviewState

```lua
C_HousingDecor.IsModeDisabledForPreviewState(mode: HouseEditorMode) -> isModeDisabled: bool
```

`SecretArguments=AllowedWhenUntainted`

### IsPreviewState

```lua
C_HousingDecor.IsPreviewState() -> isPreviewState: bool
```

### RemovePlacedDecorEntry

```lua
C_HousingDecor.RemovePlacedDecorEntry(decorGUID: WOWGUID)
```

Placed Decor List APIs currently restricted due to being potentially very expensive operations, may be reworked & opened up in the future

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### RemoveSelectedDecor

```lua
C_HousingDecor.RemoveSelectedDecor()
```

Attempt to return the currently selected decor instance back to the house chest

### SetGridVisible

```lua
C_HousingDecor.SetGridVisible(gridVisible: bool)
```

`SecretArguments=AllowedWhenUntainted`

### SetPlacedDecorEntryHovered

```lua
C_HousingDecor.SetPlacedDecorEntryHovered(decorGUID: WOWGUID, hovered: bool)
```

Placed Decor List APIs currently restricted due to being potentially very expensive operations, may be reworked & opened up in the future

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

### SetPlacedDecorEntrySelected

```lua
C_HousingDecor.SetPlacedDecorEntrySelected(decorGUID: WOWGUID, selected: bool)
```

Placed Decor List APIs currently restricted due to being potentially very expensive operations, may be reworked & opened up in the future

`SecretArguments=AllowedWhenUntainted` `HasRestrictions`

## Events

### HOUSE_DECOR_ADDED_TO_CHEST

```lua
HOUSE_DECOR_ADDED_TO_CHEST(decorGUID: WOWGUID, decorID: number)
```

`SynchronousEvent`

### HOUSE_EXTERIOR_POSITION_FAILURE

```lua
HOUSE_EXTERIOR_POSITION_FAILURE(housingResult: HousingResult)
```

`SynchronousEvent`

### HOUSE_EXTERIOR_POSITION_SUCCESS

```lua
HOUSE_EXTERIOR_POSITION_SUCCESS()
```

`SynchronousEvent`

### HOUSING_DECOR_GRID_VISIBILITY_STATUS_CHANGED

```lua
HOUSING_DECOR_GRID_VISIBILITY_STATUS_CHANGED(isGridVisible: bool)
```

`SynchronousEvent`

### HOUSING_DECOR_PLACE_FAILURE

```lua
HOUSING_DECOR_PLACE_FAILURE(housingResult: HousingResult)
```

`SynchronousEvent`

### HOUSING_DECOR_PLACE_SUCCESS

```lua
HOUSING_DECOR_PLACE_SUCCESS(decorGUID: WOWGUID, size: HousingCatalogEntrySize, isNew: bool, isPreview: bool)
```

`SynchronousEvent`

Payload:

| Name | Type | Notes |
|---|---|---|
| `decorGUID` | `WOWGUID` |  |
| `size` | `HousingCatalogEntrySize` |  |
| `isNew` | `bool` | Will be true if the decor is newly placed from storage, false if it was already placed and just moved |
| `isPreview` | `bool` |  |

### HOUSING_DECOR_PREVIEW_STATE_CHANGED

```lua
HOUSING_DECOR_PREVIEW_STATE_CHANGED(isPreviewState: bool)
```

`SynchronousEvent`

### HOUSING_DECOR_REMOVED

```lua
HOUSING_DECOR_REMOVED(decorGUID: WOWGUID)
```

`SynchronousEvent`

### HOUSING_DECOR_SELECT_RESPONSE

```lua
HOUSING_DECOR_SELECT_RESPONSE(result: HousingResult)
```

`SynchronousEvent`

### HOUSING_NEW_DECOR_PLACE_COMPLETE

```lua
HOUSING_NEW_DECOR_PLACE_COMPLETE(decorGUID: WOWGUID)
```

`SynchronousEvent`

### HOUSING_NUM_DECOR_PLACED_CHANGED

```lua
HOUSING_NUM_DECOR_PLACED_CHANGED()
```

`SynchronousEvent`

## Types

### LightRadiusIndicatorType

*Enumeration* · 3 values, 0..2

Access values as `Enum.LightRadiusIndicatorType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `Always` | `LightRadiusIndicatorType` | = 0 |
| `Overlap` | `LightRadiusIndicatorType` | = 1 |
| `Never` | `LightRadiusIndicatorType` | = 2 |

### HousingDecorInstanceListEntry

*Structure*

Smaller structs with the minimum fields from HousingDecorInstanceInfo needed to identify/display a slim list of placed decor

Fields:

| Name | Type | Notes |
|---|---|---|
| `decorGUID` | `WOWGUID` |  |
| `name` | `cstring` |  |
