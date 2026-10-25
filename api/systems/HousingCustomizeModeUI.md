# HousingCustomizeModeUI

Namespace `C_HousingCustomizeMode` · environment All · source `interface/addons/blizzard_apidocumentationgenerated/housingcustomizemodeuidocumentation.lua` (FileDataID 7350482)

## Functions

### ApplyDyeToSelectedDecor

```lua
C_HousingCustomizeMode.ApplyDyeToSelectedDecor(dyeSlotID: number, dyeColorID: number?)
```

If a dyeable decor is selected, applies a specific dye color in a specific slot as a preview; See CommitDyesForSelectedDecor to actually save applied dye changes

`SecretArguments=AllowedWhenUntainted`

Arguments:

| Name | Type | Notes |
|---|---|---|
| `dyeSlotID` | `number` |  |
| `dyeColorID` | `number?` | If not provided, clears the dye from the specified dye slot, returning that part of the decor asset to its default color |

### ApplyPetToSelectedDecor

```lua
C_HousingCustomizeMode.ApplyPetToSelectedDecor(petID: WOWGUID?, petBehavior: HousingPetBehaviorType)
```

If a decor is selected that supports pets, applies a specific petID to be shown on that decor

`SecretArguments=AllowedWhenUntainted`

### ApplyThemeToRoom

```lua
C_HousingCustomizeMode.ApplyThemeToRoom(themeSetID: number)
```

Attempt to apply a specific theme set (aka style) to all applicable room components in the current room

`SecretArguments=AllowedWhenUntainted`

### ApplyThemeToSelectedRoomComponent

```lua
C_HousingCustomizeMode.ApplyThemeToSelectedRoomComponent(themeSetID: number)
```

Attempt to apply a specific theme set (aka style) to the currently selected room component only

`SecretArguments=AllowedWhenUntainted`

### ApplyWallpaperToAllWalls

```lua
C_HousingCustomizeMode.ApplyWallpaperToAllWalls(roomComponentTextureRecID: number)
```

Attempt to apply a specific wallpaper (aka material/texture) to all applicable room components in the current room

`SecretArguments=AllowedWhenUntainted`

### ApplyWallpaperToSelectedRoomComponent

```lua
C_HousingCustomizeMode.ApplyWallpaperToSelectedRoomComponent(roomComponentTextureRecID: number)
```

Attempt to apply a specific wallpaper (aka material/texture) to the currently selected room component only

`SecretArguments=AllowedWhenUntainted`

### CancelActiveEditing

```lua
C_HousingCustomizeMode.CancelActiveEditing()
```

Cancels all in-progress editing of the selected target, which will reset any unapplied customization changes and deselect the active target

### ClearDyesForSelectedDecor

```lua
C_HousingCustomizeMode.ClearDyesForSelectedDecor()
```

Clears all previewed dye changes on the selected decor; Does not clear any already saved dyes that were previously applied

### ClearTargetRoomComponent

```lua
C_HousingCustomizeMode.ClearTargetRoomComponent()
```

Deselect the currently selected room component, if there is one

### CommitDyesForSelectedDecor

```lua
C_HousingCustomizeMode.CommitDyesForSelectedDecor() -> hasChanges: bool
```

Attempt to save all previewed dye changes made to the selected decor

Returns:

| Name | Type | Notes |
|---|---|---|
| `hasChanges` | `bool` | True if there were any changes to save |

### GetHoveredDecorInfo

```lua
C_HousingCustomizeMode.GetHoveredDecorInfo() -> info: HousingDecorInstanceInfo?
```

Returns info for the placed decor instance currently being hovered, if there is one

### GetHoveredRoomComponentInfo

```lua
C_HousingCustomizeMode.GetHoveredRoomComponentInfo() -> info: HousingRoomComponentInstanceInfo?
```

Returns info for the room component currently being hovered, if there is one

### GetNumDyesToRemoveOnSelectedDecor

```lua
C_HousingCustomizeMode.GetNumDyesToRemoveOnSelectedDecor() -> numDyesToRemove: number
```

If a dyeable decor instance is selected, returns how many dye slots would be cleared on applying all currently previewed dye changes

### GetNumDyesToSpendOnSelectedDecor

```lua
C_HousingCustomizeMode.GetNumDyesToSpendOnSelectedDecor() -> numDyesToSpend: number
```

If a dyeable decor instance is selected, returns how many dye items would be spent on applying all currently previewed dye changes

### GetPreviewDyesOnSelectedDecor

```lua
C_HousingCustomizeMode.GetPreviewDyesOnSelectedDecor() -> previewDyes: PreviewDyeSlotInfo[]
```

If a dyeable decor instance is selected, returns info structs for each new/changed dye currently being previewed

### GetRecentlyUsedDyes

```lua
C_HousingCustomizeMode.GetRecentlyUsedDyes() -> recentDyes: number[]
```

Returns a list of ids for the dyes most recently applied by the player, if any

### GetRecentlyUsedThemeSets

```lua
C_HousingCustomizeMode.GetRecentlyUsedThemeSets() -> recentThemeSets: number[]
```

Returns a list of ids for the theme sets (aka styles) most recently applied by the player, if any

### GetRecentlyUsedWallpapers

```lua
C_HousingCustomizeMode.GetRecentlyUsedWallpapers() -> recentWallpapers: number[]
```

Returns a list of ids for the wallpapers most recently applied by the player, if any

### GetSelectedDecorInfo

```lua
C_HousingCustomizeMode.GetSelectedDecorInfo() -> info: HousingDecorInstanceInfo?
```

Returns info for the decor instance that's currently selected, if there is one

### GetSelectedDecorPetInfo

```lua
C_HousingCustomizeMode.GetSelectedDecorPetInfo() -> petID: WOWGUID?, petBehavior: HousingPetBehaviorType
```

If a decor is selected that supports pets, gets petID and behavior type from decor

### GetSelectedRoomComponentInfo

```lua
C_HousingCustomizeMode.GetSelectedRoomComponentInfo() -> info: HousingRoomComponentInstanceInfo?
```

Returns info for the currently selected room component, if there is one

### GetThemeSetInfo

```lua
C_HousingCustomizeMode.GetThemeSetInfo(themeSetID: number) -> name: string?
```

Returns the name of the specified theme set (aka style) if it exists

`SecretArguments=AllowedWhenUntainted`

### GetWallpapersForRoomComponentType

```lua
C_HousingCustomizeMode.GetWallpapersForRoomComponentType(type: HousingRoomComponentType) -> availableWallpapers: RoomComponentWallpaper[]
```

Get all wallpapers (aka materials/textures) available for the selected room component type, if any

`SecretArguments=AllowedWhenUntainted`

### IsDecorSelected

```lua
C_HousingCustomizeMode.IsDecorSelected() -> hasSelectedDecor: bool
```

Returns true if a decor instance is currently selected for customization

### IsHouseExteriorDoorHovered

```lua
C_HousingCustomizeMode.IsHouseExteriorDoorHovered() -> isHouseExteriorDoorHovered: bool
```

Returns true if the entry door of the house's exterior is currently being hovered

### IsHoveringDecor

```lua
C_HousingCustomizeMode.IsHoveringDecor() -> isHoveringDecor: bool
```

Returns true if a placed decor instance is currently being hovered

### IsHoveringRoomComponent

```lua
C_HousingCustomizeMode.IsHoveringRoomComponent() -> isHovering: bool
```

Returns true if a room component is currently being hovered

### IsRoomComponentSelected

```lua
C_HousingCustomizeMode.IsRoomComponentSelected() -> hasSelectedComponent: bool
```

Returns true if a room component is currently selected for customization

### RoomComponentSupportsVariant

```lua
C_HousingCustomizeMode.RoomComponentSupportsVariant(componentID: number, variant: number) -> variantSupported: bool
```

Check whether a specific room component supports a particular variant; What kind of id or enum 'variant' equates to is complicated, as it depends on the component type

`SecretArguments=AllowedWhenUntainted`

### RoomConnectionSupportsDoorType

```lua
C_HousingCustomizeMode.RoomConnectionSupportsDoorType(roomGUID: WOWGUID, componentID: number, newDoortype: HousingRoomComponentDoorType) -> doorTypeSupported: bool
```

Check whether a specific room component, within a specific room, supports a particular doorType

`SecretArguments=AllowedWhenUntainted`

### SetRoomComponentCeilingType

```lua
C_HousingCustomizeMode.SetRoomComponentCeilingType(roomGUID: WOWGUID, componentID: number, ceilingType: HousingRoomComponentCeilingType)
```

Attempt to set a specific ceiling component, within a specific room, to a specific new ceiling type

`SecretArguments=AllowedWhenUntainted`

### SetRoomComponentDoorType

```lua
C_HousingCustomizeMode.SetRoomComponentDoorType(roomGUID: WOWGUID, componentID: number, newDoortype: HousingRoomComponentDoorType)
```

Attempt to set a specific door component, within a specific room, to a specific new door type

`SecretArguments=AllowedWhenUntainted`

## Events

### HOUSING_CUSTOMIZE_MODE_HOVERED_TARGET_CHANGED

```lua
HOUSING_CUSTOMIZE_MODE_HOVERED_TARGET_CHANGED(hasHoveredTarget: bool, targetType: HousingCustomizeModeTargetType)
```

`SynchronousEvent`

### HOUSING_CUSTOMIZE_MODE_SELECTED_TARGET_CHANGED

```lua
HOUSING_CUSTOMIZE_MODE_SELECTED_TARGET_CHANGED(hasSelectedTarget: bool, targetType: HousingCustomizeModeTargetType)
```

`SynchronousEvent`

### HOUSING_DECOR_CUSTOMIZATION_CHANGED

```lua
HOUSING_DECOR_CUSTOMIZATION_CHANGED(decorGUID: WOWGUID)
```

`SynchronousEvent`

### HOUSING_DECOR_DYE_FAILURE

```lua
HOUSING_DECOR_DYE_FAILURE(decorGUID: WOWGUID, housingResult: HousingResult)
```

`SynchronousEvent`

### HOUSING_ROOM_COMPONENT_CUSTOMIZATION_CHANGED

```lua
HOUSING_ROOM_COMPONENT_CUSTOMIZATION_CHANGED(roomGUID: WOWGUID, componentID: number)
```

`SynchronousEvent`

### HOUSING_ROOM_COMPONENT_CUSTOMIZATION_CHANGE_FAILED

```lua
HOUSING_ROOM_COMPONENT_CUSTOMIZATION_CHANGE_FAILED(roomGUID: WOWGUID, componentID: number, housingResult: HousingResult)
```

`SynchronousEvent`

## Types

### HousingCustomizeModeTargetType

*Enumeration* · 4 values, 0..3

Access values as `Enum.HousingCustomizeModeTargetType.<Name>`.

Values:

| Name | Type | Notes |
|---|---|---|
| `None` | `HousingCustomizeModeTargetType` | = 0 |
| `Decor` | `HousingCustomizeModeTargetType` | = 1 |
| `RoomComponent` | `HousingCustomizeModeTargetType` | = 2 |
| `ExteriorHouse` | `HousingCustomizeModeTargetType` | = 3 |

### HousingRoomComponentInstanceInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `roomGUID` | `WOWGUID` |  |
| `type` | `HousingRoomComponentType` |  |
| `componentID` | `number` |  |
| `canBeCustomized` | `bool` |  |
| `currentThemeSet` | `number?` |  |
| `availableThemeSets` | `number[]` |  |
| `currentWallpaper` | `number?` |  |
| `currentRoomComponentTextureRecID` | `number?` |  |
| `ceilingType` | `HousingRoomComponentCeilingType` |  |
| `doorType` | `HousingRoomComponentDoorType` |  |

### PreviewDyeSlotInfo

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `dyeColorID` | `number` |  |
| `dyeSlotID` | `number` |  |

### RoomComponentWallpaper

*Structure*

Fields:

| Name | Type | Notes |
|---|---|---|
| `name` | `cstring` |  |
| `roomComponentTextureRecID` | `number` |  |
